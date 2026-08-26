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

# Fronteira protegida da migração

A transição do Novo Motor para `sistema/` é uma **migração mecânica**, não uma reconstrução da arquitetura de condução.

O Novo Motor pode substituir ou atualizar:

- testes e oposição;
- Atributos e Perícias;
- Patamar;
- Vida, Mana, Dano, Defesa, RD e Barreira;
- Poderes e seus Hubs;
- Status e efeitos mecânicos;
- Traços quando possuírem função mecânica;
- campos e cálculos mecânicos das fichas;
- regras mecânicas utilizadas durante a criação de personagens.

As seguintes áreas ficam protegidas como arquitetura de `sistema/`:

- `personas/` — autoridade, cadeiras e delegação;
- `agencia/` — continuidade de vontade e agência;
- `narracao/` — forma de apresentar e dramatizar a ficção;
- `operacao/` — fluxo da mesa, janelas, interrupções e funcionamento dos turnos;
- `persistencia/` — arquitetura de registro e continuidade;
- `criacao/` — fluxo de criação da campanha, perguntas, checkpoints e aprovações.

Essas áreas podem receber apenas correções de **nomes, referências ou campos mecânicos** necessárias para apontar para as novas regras. Seu comportamento estrutural não deve ser substituído pelo Novo Motor.

Em especial:

> **O combate continua usando os turnos simultâneos de até 10 segundos definidos em `sistema/operacao/turnos-de-combate.md`.**

O Novo Motor não cria uma ordem fixa de iniciativa nem uma economia de "uma ação por turno" dentro dessa arquitetura.

Quando uma regra mecânica do Novo Motor conflitar com uma regra operacional, de agência, persona ou narração já consolidada em `sistema/`, aplicar a mecânica nova somente até a fronteira de resolução e preservar a arquitetura de `sistema/`.

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

A fronteira da migração também está FECHADA:

> **migrar mecânicas de resolução sem substituir personas, agência, narração ou o comportamento operacional de `sistema/`.**

A antiga fórmula própria de Iniciativa também foi descartada para a migração. Precedência incerta dentro de um turno simultâneo passa a usar a própria resolução universal de oposição.

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

# Tempo, turno, movimento, precedência e distância

Tempo mecânico:

> **Instante → Turno → Cena → Hora → Dia**

A operação concreta dos turnos pertence a `sistema/operacao/`.

Durante combate, preservar a regra já consolidada em `sistema/operacao/turnos-de-combate.md`:

> **um Turno é um intervalo simultâneo de até aproximadamente 10 segundos compartilhado pelas peças envolvidas.**

Não existe, por causa do Novo Motor:

- ordem fixa de iniciativa por personagem;
- rodada sequencial obrigatória;
- regra universal de uma única ação por personagem;
- direito de agir primeiro apenas por ter declarado primeiro.

Ações que não interferem entre si podem acontecer normalmente dentro do mesmo intervalo.

## Precedência dentro do turno

Quando duas ou mais ações competirem pelo mesmo instante, usar primeiro a ficção:

```text
PRECEDÊNCIA EVIDENTE
→ estabelecer diretamente qual acontece primeiro.

AÇÕES SEM INTERFERÊNCIA REAL
→ podem ocorrer dentro do mesmo intervalo sem disputa de precedência.

PRECEDÊNCIA REALMENTE INCERTA
→ resolver como oposição comum.
```

Não existe uma fórmula especial de Iniciativa.

Quando a precedência for realmente incerta:

> **4 dados mantidos + Atributo × 4 dados mantidos + Atributo**

Cada lado utiliza o Atributo coerente com a maneira pela qual tenta agir primeiro.

Exemplos possíveis:

- rapidez e coordenação corporal → **Controle**;
- antecipação e leitura da situação → **Intelecto**;
- segurar ou bloquear alguém antes que passe → **Potência**;
- outra abordagem → Atributo correspondente à ação concreta.

Os Atributos dos dois lados não precisam ser iguais.

Uma Perícia relevante pode conceder `+1d` normalmente quando seu treinamento realmente contribuir para aquela disputa de precedência.

Empates seguem a regra universal de oposição: favorecem quem iniciou a ação concorrente.

A resolução de precedência vale apenas para aquela interferência concreta. Ela **não cria uma ordem permanente** para o restante do turno, da rodada, da cena ou do combate.

## Distâncias

```text
Si Mesmo
Toque
Próximo ≈ 3 m
Curto ≈ 20 m
Médio ≈ 45 m
Longo ≈ 90 m
```

Além de Longo normalmente exige capacidade própria.

`Andar [Curto]` aparece como referência de movimento em exemplos e fichas. A frase central definitiva de movimento padrão ainda deve ser conferida durante a limpeza/migração para evitar duplicação ou formulação antiga, sem substituir o funcionamento operacional dos turnos de `sistema/`.

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

Durante a migração, esta seção serve apenas como referência de compatibilidade. A implementação operacional de CONTROLE continua pertencendo a `sistema/personas/` e não deve ser substituída.

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

Durante a migração mecânica inicial, os usos de Trama que alteram diretamente narração ou cânone não devem ser usados como justificativa para reescrever `sistema/narracao/` ou `sistema/personas/`. Sua integração com a arquitetura existente deve ser tratada separadamente quando necessário.

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
- referências à antiga Iniciativa `4d6 + Controle + Intelecto` devem ser removidas ou reinterpretadas: precedência incerta usa oposição comum de Atributos;
- referências a "uma ação por Turno" ou resolução sequencial obrigatória não devem substituir os turnos simultâneos de `sistema/operacao/`;
- a frase central de movimento padrão deve ser conferida para garantir consistência com `Andar [Curto]` e com o Traço Velocidade sem alterar a estrutura operacional dos turnos.

Durante a migração, corrigir essas divergências com base nas regras fechadas acima, sem reabrir as decisões já aprovadas.

---

# Processo recomendado para a transição

Não migrar tudo de uma vez.

Para cada área mecânica:

1. ler os arquivos correspondentes de `novo-motor/`;
2. ler a área de destino em `sistema/`;
3. identificar o que é arquitetura aproveitável e o que é mecânica antiga;
4. apresentar ao JOGADOR HUMANO uma proposta curta de substituição;
5. esclarecer dúvidas reais antes de alterar;
6. após aprovação, salvar a alteração;
7. conferir o resultado antes de continuar para a próxima área.

A ordem atual aprovada para a transição é:

```text
1. resolucao
   → princípio universal, 4d6, CDs, oposição e precedência
   → depois combate, dano e resistências

2. personagem mecânico
   → Atributos, Perícias, Patamar e campos mecânicos de ficha

3. recursos
   → Vida, Mana, recuperação, RD e Barreira

4. poderes e status
   → conceito mecânico, Hubs, efeitos, famílias e aplicações

5. criacao mecânica
   → distribuição, quantidades e custos iniciais
   → preservar o fluxo de criação de campanha já existente

6. compatibilidade estrutural
   → corrigir somente nomes, links e campos mecânicos em `operacao/` e `persistencia/`
   → não mudar o funcionamento dessas áreas

7. auditoria final
   → localizar e remover referências mecânicas antigas que ainda concorram com o Novo Motor
```

Não são etapas de migração mecânica:

```text
personas
agencia
narracao
```

Essas áreas permanecem como estão, salvo correção pontual de referência explicitamente necessária e aprovada.

`operacao/` também não é redesenhada. Ela apenas recebe compatibilidade mecânica quando necessário.

---

# Instrução curta para abrir o próximo chat

Use algo equivalente a:

> **"Vamos continuar a transição do Novo Motor para a estrutura `sistema/` do repositório `wyliam2707/Sistema-Narrativo`. Leia primeiro `novo-motor/TRANSICAO-PARA-SISTEMA.md`. O Novo Motor é a fonte mecânica atual; preserve `personas/`, `agencia/`, `narracao/` e o funcionamento de `operacao/`. Migre uma área mecânica por vez, explique a proposta, esclareça dúvidas e peça minha aprovação antes de cada mudança conceitual."**

---

# Regra final da transição

> **Não redesenhar a arquitetura de `sistema/` durante a migração. Transferir as mecânicas aprovadas do Novo Motor para os lugares já existentes em `sistema/`, preservando personas, agência, narração e operação. Refinamentos novos só entram quando o JOGADOR HUMANO explicitamente abrir uma nova decisão de design.**