# Transição do Novo Motor para `sistema/`

Status: **PRONTO PARA INICIAR A TRANSIÇÃO**

Este arquivo é o ponto de continuidade para um novo chat.

O objetivo da próxima etapa é migrar as regras aprovadas em `novo-motor/` para a arquitetura operacional já existente em `sistema/`, preservando a organização útil de `sistema/` e substituindo as mecânicas antigas que entrarem em conflito com o Novo Motor.

> **Durante a transição, `novo-motor/` é a fonte de verdade para as regras mecânicas novas.**

> **Não apagar `novo-motor/` até o JOGADOR HUMANO declarar explicitamente que a migração terminou.**

---

# Regra de prioridade durante a migração

Quando houver conflito entre documentos:

1. correção explícita mais recente do JOGADOR HUMANO;
2. regra aprovada em `novo-motor/`;
3. arquitetura atual de `sistema/`, quando não contradizer o Novo Motor;
4. formulações mecânicas antigas de `sistema/` apenas como material legado a ser substituído.

A arquitetura em `sistema/` continua útil como destino organizacional:

```text
sistema/
├── criacao/
├── personagem/
├── personas/
├── resolucao/
├── agencia/
├── narracao/
├── persistencia/
└── operacao/
```

O arquivo `sistema/MIGRACAO-ESTRUTURAL.md` registra uma migração estrutural anterior e contém mecânicas antigas. Ele é histórico e não deve ser usado para desfazer o Novo Motor.

---

# Estado do projeto

Os sete pontos de fechamento do Novo Motor foram resolvidos:

1. **Criação: Atributos e Perícias** — FECHADO.
2. **Atributos temporários e acúmulo** — FECHADO.
3. **Piso da Mana** — FECHADO; não existe piso artificial necessário.
4. **Quem possui Trama** — FECHADO; somente JOGADOR HUMANO.
5. **Definição de Poder mundano/sobrenatural** — FECHADO.
6. **Modelo Mínimo de ficha** — FECHADO.
7. **CONTROLE e papéis das IAs** — FECHADO.

Depois desses sete pontos, a regra de **Pontos de Trama** foi refinada e também está FECHADA para a transição.

---

# Princípio central de resolução

> **Sempre resolva uma ação ou uso de Poder com o menor número possível de rolagens.**

A ficção vem primeiro:

- ação óbvia não exige teste;
- ação impossível não se torna possível por brecha mecânica;
- teste existe quando há incerteza, oposição ou risco relevante;
- o Narrador não escolhe a ação voluntária de um personagem controlado por jogador.

---

# Resolução universal

Base:

> **4d6 + Atributo**

Bônus:

```text
+1d → rola 5d6 e mantém os 4 maiores
+2d → rola 6d6 e mantém os 4 maiores
```

Penalidades:

```text
-1d → rola 5d6 e mantém os 4 menores
-2d → rola 6d6 e mantém os 4 menores
```

Bônus e penalidades se cancelam.

Limite universal:

> **±2d**

Perícia relevante concede **+1d**. Várias Perícias aplicáveis continuam concedendo no máximo **+1d**.

Não existe Perícia genérica de combate.

Empates em oposição favorecem quem iniciou a ação. Contra uma CD, igualdade é sucesso. Para uma defesa superar um ataque, a defesa precisa obter resultado maior.

---

# Atributos

Corpo:

- Potência
- Controle
- Resistência

Mente:

- Intelecto
- Presença
- Vontade

Escala permanente normal:

> **[-2] a [7]**, com `[0]` como referência comum.

Efeitos temporários podem ultrapassar esses limites.

O Atributo é escolhido pela finalidade e pela forma real da ação, não pelo nome de um movimento nem simplesmente pelo maior valor disponível.

## Criação

Pontos de Atributo:

> **Patamar × 4**

Máximo de criação por Atributo:

> **Patamar + 2**, respeitando o máximo permanente absoluto `[7]`.

Um Atributo abaixo de `[0]` devolve pontos para redistribuição na criação.

## Ampliações temporárias

No máximo **2 Atributos diferentes** podem estar ampliados temporariamente ao mesmo tempo.

Reduções temporárias não possuem limite equivalente de quantidade de Atributos afetados.

Mudanças temporárias não recalculam Vida Máxima nem Mana Máxima.

---

# Perícias

Lista atual:

- Animais
- Campestre
- Ciência
- Condução
- Crime
- Engenharia
- Esportes
- Explorar
- Expressão
- Idiomas
- Investigar
- Manipulação
- Medicina
- Ocultismo
- Ofícios
- Sociedade

Quantidade na criação:

```text
personagem simples → 1 Perícia
personagem relevante → 2 Perícias
vilão ou personagem jogador → 3 Perícias
```

Perícias são amplas e não possuem Atributo fixo.

---

# Patamar

Escala:

> **[1] a [7]**

`[X]` representa o Patamar quando usado nas regras dos Poderes.

Na criação:

- pontos positivos de Traço = `Patamar + 1`;
- quantidade base de Poderes = `Patamar + 1`.

Cada ponto obtido por Vício/Corrupção pode ser gasto em **1 ponto de Traço positivo OU +1 Poder**, nunca nos dois ao mesmo tempo.

---

# Vida

Fórmula:

> **Vida = 10 + (Resistência × 4) + (Potência × 2) + (Controle × 2) + Intelecto + Presença + Vontade**

Para o cálculo de Vida, Atributos negativos contam como `0`.

Alteração permanente de Atributo recalcula Vida. Alteração temporária não recalcula.

Em `0` de Vida o personagem fica **Incapacitado**; isso não significa automaticamente morto ou inconsciente.

Recuperação natural por dia de descanso:

> **Resistência × 2**, mínimo `2`.

Medicina:

```text
5  → +1
10 → +2
15 → +3
20 → +4
25+ → +5
```

Frações de Dano são arredondadas para baixo. Se uma aplicação de Dano existir, o Dano final mínimo é `1`, salvo regra que o anule completamente.

Ordem de Dano:

> **Defesa → redução pela Defesa → RD → Barreira → Vida**

Múltiplas RDs não somam; usa-se apenas a maior aplicável.

---

# Mana

Definição:

> **Mana é a reserva técnica abstrata utilizada para alimentar o uso dos Poderes.**

> **A mecânica é sempre Mana; a ficção determina o que essa reserva significa para cada personagem.**

Pode representar magia, munição, bateria, equipamentos preparados, esforço, fôlego ou outro recurso coerente.

Fórmula:

> **Mana = 10 + 2 × soma dos seis Atributos**

Atributos negativos reduzem a Mana normalmente.

Não é necessário piso artificial de Mana na criação, porque a redistribuição dos pontos de Atributo preserva a soma total.

Recuperação:

> **Vontade de Mana por hora**, mínimo `1`.

Após 8 horas reais de descanso, toda a Mana é restaurada.

---

# Poderes

Definição aprovada:

> **Poder é o arsenal funcional do personagem.**

Um Poder define ações e efeitos configuráveis que o personagem possui e pode produzir.

O termo **Poder** é mecânico, não significa necessariamente sobrenatural.

A origem pode ser:

- mundana;
- física;
- técnica;
- tecnológica;
- equipamento;
- mística;
- sobrenatural;
- outra origem coerente com o conceito.

Alguns Poderes possuem custo operacional começando em `0+`; outros começam em `1+`, conforme a estrutura específica do Poder.

O Hub configura **como** o arsenal é usado; o Poder define **o que é possível produzir**.

Ações comuns continuam possíveis mesmo sem um Poder correspondente.

Exemplo: um personagem sem `[Golpe]` ainda pode dar um soco.

Ataque comum sem Poder ofensivo:

> **Dano = valor do Atributo usado na ação, sem rolagem de Dano.**

Poderes ofensivos fornecem sua própria estrutura de Dano, alcance, efeitos e configurações.

Estrutura ofensiva geral:

> **Defesa → Dano → Resistência → Efeito**

Um único uso contra vários alvos usa o menor número possível de rolagens: uma rolagem de Acerto quando necessária e uma rolagem de Dano quando necessária; defesas e resistências individuais permanecem separadas quando precisam produzir resultados individuais.

---

# Tempo, turno, movimento e distância

Tempo:

> **Instante → Turno → Cena → Hora → Dia**

Um Turno representa aproximadamente **10 segundos**.

Cada personagem possui uma ação em seu Turno e movimento normal, podendo mover-se antes, durante ou depois da ação quando a ficção permitir.

Pequenas interações coerentes podem fazer parte da ação.

Uma ação termina sua resolução antes do próximo participante agir.

Defender-se não consome automaticamente a ação seguinte.

Iniciativa:

> **4d6 + Controle + Intelecto**

Empates de iniciativa são desempatados com `1d6`.

Distâncias:

```text
Si Mesmo
Toque
Próximo ≈ 3 m
Curto ≈ 20 m
Médio ≈ 45 m
Longo ≈ 90 m
```

Além de Longo normalmente exige capacidade própria.

`Andar [Curto]` aparece como referência de movimento em exemplos e fichas. A frase central definitiva de movimento padrão ainda deve ser conferida durante a limpeza/migração para evitar duplicação ou formulação antiga.

---

# Traços

Traços são passivos e descrevem características relevantes do personagem.

Traços positivos normalmente usam valores `[1]` a `[3]`.

Vícios são `[-1]`.

Corrupções podem ser `[-1]` ou `[-2]`.

Traços podem interagir com Trama quando criam complicações reais.

---

# Status

Famílias atuais:

- Sentidos
- Contenção
- Terror
- Exaustão
- Perturbação
- Aflição
- Posição
- Influência
- Ruína
- Debilitação

Cada família é controlada separadamente.

Dentro da mesma família, apenas o efeito mais forte fica ativo. Efeitos de famílias diferentes podem coexistir.

Para mesmo efeito/fonte:

- o mais forte fica ativo;
- em igualdade de força, permanece o de maior duração;
- durações não se somam;
- efeito mais fraco ainda pode continuar com seu tempo correndo e voltar a ficar ativo quando o mais forte terminar.

---

# Fichas

## Ficha Completa

Obrigatória para:

- JOGADOR HUMANO;
- JOGADOR IA;
- JOGADOR IA EVENTUAL.

Blocos:

1. Descrição
2. Atributos e Perícias
3. Traços e Poderes
4. Recursos e Movimento
5. Personalidade
6. Relacionamentos
7. Histórico

## Ficha Rápida

Usada para NPCs relevantes quando uma ficha completa não é necessária.

Inclui os seis Atributos, Perícias efetivas, Traços/Poderes relevantes, Vida/Mana, Movimento e uma Conduta curta.

## Ficha Mínima

Usada para figurantes, criaturas simples e peças de resolução pontual.

Estrutura:

- Nome
- Conceito
- Patamar
- apenas capacidades relevantes
- Vida/Mana somente quando acompanhados
- Movimento apenas quando diferente do normal

Informação ausente **não significa `[0]` ou inexistência**; significa apenas que ainda não precisou ser registrada.

Status temporários não fazem parte da ficha-base mínima.

---

# CONTROLE

Regra central:

> **CONTROLE determina quem possui autoridade para decidir as ações voluntárias do personagem. O Narrador descreve o mundo e as consequências; o controlador decide o que o personagem escolhe fazer.**

## JOGADOR HUMANO

O humano decide ações voluntárias, falas e escolhas.

É o único tipo de personagem que possui **Pontos de Trama**.

## JOGADOR IA

Uma IA atua como jogador daquele personagem e decide ações, falas e escolhas usando sua ficha, Personalidade, Tendências, Desejos, Relacionamentos e Histórico.

## JOGADOR IA EVENTUAL

Funciona normalmente como NPC, mas pode receber temporariamente uma IA dedicada como jogador. Enquanto estiver sob esse controle, possui a mesma agência de um JOGADOR IA.

## NARRADOR

Controla mundo, ambiente, consequências e NPCs sem controlador próprio.

Não escolhe ações voluntárias de personagens controlados por jogador.

## OPOSITOR

Cria pressão, conflitos e aplica complicações/regras.

Não toma decisões voluntárias pelo personagem de jogador.

---

# Pontos de Trama

Arquivo canônico atual:

> `novo-motor/trama.md`

Conceito:

> **Trama é o privilégio narrativo do protagonista.**

Ela representa a margem de roteiro que permite ao protagonista sobreviver, encontrar uma abertura improvável, corrigir uma consequência recém-acontecida ou fazer a história admitir uma possibilidade que normalmente seria improvável.

Trama não é simplesmente sorte. É **protagonismo**.

Somente `CONTROLE: JOGADOR HUMANO` possui Trama.

Reserva inicial:

> **30 Pontos de Trama**

Recuperação:

- +5 por novo dia;
- até +5 adicionais por dia ao aceitar complicações relevantes de seus próprios Traços.

## Usos mecânicos

```text
1 Trama  → reduz 1 de Dano
1 Trama  → substitui 1 Mana faltante para pagar um Poder
5 Trama  → +1d
10 Trama → +2d
5 Trama  → reduz penalidade de -1d
10 Trama → reduz penalidade de -2d
5 Trama  → recebe uma dica do Narrador
```

O limite universal `±2d` continua valendo.

## Uso narrativo — 5 Trama

> **5 Trama suaviza em um grau uma consequência narrativa imediata, desde que exista uma versão menos grave e plausível.**

Exemplo:

```text
"O aliado morreu."
→ 5 Trama
→ volta ao instante
→ "O aliado está incapacitado, gravemente ferido, mas vivo."
```

A consequência continua existindo, porém deixa de ser tão definitiva.

## Uso narrativo — 10 Trama

> **10 Trama pode abrir uma possibilidade narrativa forte que antes seria extremamente improvável, inesperada ou praticamente impensável.**

Isso pode transformar rejeição absoluta em:

- considerar;
- avaliar;
- hesitar;
- sentir curiosidade;
- admitir a hipótese;
- aceitar conversar sobre aquilo.

**Abrir uma possibilidade é diferente de forçar uma possibilidade.**

A Trama não obriga outro personagem a aceitar, amar, concordar, perdoar ou tomar a decisão desejada.

Ela apenas muda o espaço de possibilidades da história.

Exemplo social:

```text
Antes: "Não. Isso é absurdo. Nunca."
→ 10 Trama, usado imediatamente
Depois: "Não agora... mas a ideia deixa de ser inimaginável."
```

O personagem ainda pode responder não. A diferença é que agora existe uma possibilidade narrativa real para desenvolvimento futuro.

## Correção retroativa imediata

Trama pode ser usada **depois de o jogador conhecer a consequência**, desde que a narrativa ainda não tenha avançado para outro evento relevante decorrente dela.

O Narrador volta ao instante necessário e narra novamente a cena considerando o gasto.

A versão corrigida passa a ser o acontecimento canônico.

Exemplo de Dano:

```text
Ataque causa 12 de Dano.
Protagonista chegaria a 0 de Vida.
Jogador gasta 12 Trama.
Dano final → 0.
```

A cena é renarrada: o tiro desviou, atingiu a proteção, passou por pouco ou outra explicação coerente ocorreu.

Na versão definitiva, o protagonista nunca sofreu aqueles 12 pontos.

A correção retroativa não é limitada a combate. Pode ser usada em consequências sociais, descobertas, coincidências, oportunidades perdidas e outros resultados imediatos quando um uso válido de Trama se aplicar.

## Conveniência de roteiro

Trama também explica mecanicamente situações comuns em filmes e romances:

- o protagonista não recebe justamente o tiro fatal em uma área vulnerável;
- o vilão hesita ou fala demais;
- surge uma coincidência útil;
- alguém toma uma decisão questionável, mas ainda narrativamente explicável;
- uma oportunidade improvável aparece;
- uma consequência fatal revela-se menos definitiva.

> **A Trama transforma "armadura de roteiro" e "conveniência de roteiro" em recursos limitados e gastáveis do protagonista.**

Ela nunca elimina a necessidade de uma explicação narrativa coerente.

---

# Pontos conhecidos para limpeza durante a transição

Estes não são novas dúvidas mecânicas; são documentos que podem conter formulações anteriores e precisam ser alinhados ao migrar:

- `novo-motor/README.md` pode ainda listar Vida/Mana como não fechadas;
- `novo-motor/regras-gerais.md` pode conter observações antigas sobre Hub, RD, Vida, Mana ou Atributos temporários;
- `novo-motor/status/vida.md` pode conter observações antigas sobre Atributos temporários;
- `novo-motor/tracos/README.md` pode conter formulação antiga da economia de criação;
- `novo-motor/atributos.md` ainda pode descrever Poder como necessário apenas para algo "extraordinário"; isso deve ser substituído pelo conceito de **arsenal funcional**;
- `novo-motor/poderes/README.md` ainda pode usar a definição antiga de "ação extraordinária"; o conceito fechado está em `novo-motor/poderes/conceito.md`;
- `novo-motor/ficha/modelo-completo.md` deve ser conferido para que **Trama apareça apenas em JOGADOR HUMANO**;
- a frase central de movimento padrão deve ser conferida para garantir consistência com `Andar [Curto]` e com o Traço Velocidade.

Durante a migração, corrigir essas divergências com base nas regras fechadas acima, sem reabrir as decisões já aprovadas.

---

# Processo recomendado para o próximo chat

Não migrar tudo de uma vez.

Para cada área:

1. ler os arquivos correspondentes de `novo-motor/`;
2. ler a área de destino em `sistema/`;
3. identificar o que é arquitetura aproveitável e o que é mecânica antiga;
4. apresentar ao JOGADOR HUMANO uma proposta curta de substituição;
5. após aprovação, salvar a alteração;
6. continuar para a próxima área.

Uma ordem segura de transição é:

```text
1. resolucao   → regra universal, combate, dano, tempo e status
2. personagem  → Atributos, Perícias, Vida, Mana, Traços, Poderes e fichas
3. criacao     → Patamar, distribuição e quantidade de recursos iniciais
4. personas    → CONTROLE, JOGADOR HUMANO/IA/EVENTUAL, NARRADOR e OPOSITOR
5. agencia     → continuidade de vontade e interação com Trama/Traços
6. operacao    → sequência prática de aplicação das novas regras
7. narracao    → garantir que a apresentação respeite ficção primeiro e correção por Trama
8. persistencia→ adequar salvamento ao novo estado mecânico
```

Essa ordem é recomendação de trabalho, não nova regra do sistema.

---

# Instrução curta para abrir o próximo chat

Use algo equivalente a:

> **"Vamos iniciar a transição do Novo Motor para a estrutura `sistema/` do repositório `wyliam2707/Sistema-Narrativo`. Leia primeiro `novo-motor/TRANSICAO-PARA-SISTEMA.md`. O Novo Motor é a fonte mecânica atual; preserve a arquitetura útil de `sistema/` e migre uma área por vez, pedindo minha aprovação antes de cada mudança conceitual."**

---

# Regra final da transição

> **Não redesenhar o sistema durante a migração. Primeiro transferir fielmente as regras já aprovadas. Refinamentos novos só entram quando o JOGADOR HUMANO explicitamente abrir uma nova decisão de design.**
