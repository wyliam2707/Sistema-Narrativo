# Ciclo Operacional de Cena

Status: APROVADO

Este documento define a ordem mínima de atuação das personas durante uma janela significativa de cena.

A imagem mental oficial é:

> **Os jogadores são a defesa de suas peças. O OPOSITOR é a promotoria. O NARRADOR é o juiz.**

Em termos operacionais:

```text
JOGADORES
→ declaram pelas próprias peças.

OPOSITOR
→ procura e declara oposição, pressão, gancho, movimento ou nenhuma intervenção.

NARRADOR
→ julga.
→ narra a sentença.
→ registra.
```

# Princípios de execução

## Declaração é intenção

O jogador não precisa dizer `tento` antes de toda ação.

```text
“Eu esquivo.”
→ intenção de esquivar.

“Eu neutralizo os guardas.”
→ intenção de neutralizá-los.
```

A declaração informa **o que a peça quer fazer**. O julgamento determina o que realmente acontece.

## Intenção ampla continua enquanto ainda servir

Uma intenção pode cobrir várias ações coerentes.

Exemplo:

```text
“Vou até a cozinha, pego o livro e volto para o quarto.”
```

Não abrir nova janela por cada passo, gesto ou detalhe banal.

A intenção continua enquanto:

- nada relevante mudar;
- o método declarado continuar possível;
- nenhuma nova informação exigir escolha;
- nenhuma oposição produzir ponto real de decisão;
- a ação seguinte continuar coberta pelo que já foi declarado.

> **Não parar por hábito. Parar quando consequência voltar a ser escolha.**

Uma reação de outra peça não interrompe automaticamente o fluxo. Ela abre nova janela somente se criar decisão relevante para alguma peça controlada por jogador.

## Competência evidente entra no julgamento automaticamente

O jogador não precisa lembrar o NARRADOR de cada capacidade óbvia de sua ficha.

Se uma informação ou execução seria evidente para aquela competência, ela deve ser considerada no julgamento.

Exemplos:

```text
sentidos extraordinários
→ percebem estímulos compatíveis.

perícia muito alta em uma área
→ reconhece conhecimento evidente para alguém daquele nível.

MEN elevado
→ pode perceber padrões compatíveis com os dados realmente disponíveis.
```

Isso não cria informação inexistente e não concede onisciência.

> **Competência deve aparecer na sentença sem exigir que o jogador peça para sua ficha funcionar.**

## Combate não cria outro jogo

Combate usa a mesma janela e o mesmo motor de resolução.

Não existe obrigação universal de:

- rodada fixa;
- iniciativa fixa;
- turno isolado para cada personagem;
- ordem artificial desconectada da situação.

Precedência e oportunidade nascem dos fatos da cena, como velocidade, distância, surpresa, preparação, posição, intenção e resultado anterior, conforme `../resolucao/`.

A diferença é apenas que, em combate, o OPOSITOR frequentemente recebe peças adversárias para jogar durante a oposição.

# O que é uma janela de cena

Uma janela abre quando existe algo relevante a decidir ou resolver.

Não é necessário abrir uma nova janela para cada frase, passo ou microação.

Nova janela é necessária quando, por exemplo:

- surge informação capaz de mudar uma escolha;
- aparece obstáculo ou oportunidade relevante;
- outra peça toma iniciativa e exige resposta;
- o OPOSITOR puxa um gancho;
- uma oposição entra em cena;
- o resultado exige nova resposta;
- a intenção anterior deixa de cobrir a ação seguinte.

## Passagem de tempo dentro de uma intenção

Uma declaração pode cobrir minutos, horas ou período maior quando não houver decisão intermediária importante.

Antes de narrar todo o intervalo como concluído, verificar se durante ele:

- outra peça com agência possui ação que intersecta o período;
- um compromisso ou retorno chega ao momento relevante;
- um gancho do OPOSITOR amadurece;
- uma oposição válida interrompe o plano;
- surge informação que mudaria uma decisão.

Se nada disso acontecer, o tempo pode avançar normalmente.

Se algo acontecer no meio, a sentença para **no momento causal da mudança**, não depois de completar artificialmente toda a intenção original.

# Ordem-base

```text
1. JOGADOR HUMANO declara
↓
2. JOGADORES IA aplicáveis declaram, cada um por sua peça
↓
3. JOGADOR IA EVENTUAL é avaliado e, se ativo, declara pelas peças eventuais necessárias
↓
4. OPOSITOR declara movimento, oposição, gancho ou nenhuma intervenção
↓
5. NARRADOR JULGA
↓
6. NARRADOR NARRA A SENTENÇA até o próximo ponto de decisão
↓
7. NARRADOR REGISTRA o que passou a ser verdade
↓
8. nova janela quando houver nova decisão
```

A ordem organiza autoridade. Ela não exige revelar ao JOGADOR HUMANO declarações ou informações que precisem permanecer reservadas.

# 1. JOGADOR HUMANO

Declara o que sua própria peça tenta, quer, diz ou inicia.

Exemplo:

```text
JOGADOR HUMANO
→ atravesso o corredor e tento abrir a porta.
```

A declaração estabelece intenção, não resultado.

# 2. JOGADOR IA

Cada JOGADOR IA declara somente pela peça sob seu próprio controle.

Exemplo:

```text
JOGADOR IA — Ravena
→ vou dormir; não pretendo continuar a conversa esta noite.
```

A declaração deve refletir o que a personagem sabe, quer e faria, não o que seria conveniente para a história.

# 3. JOGADOR IA EVENTUAL

A persona verifica se algum personagem eventual autorizado precisa realmente tomar decisão naquela janela.

Se sim:

```text
JOGADOR IA EVENTUAL
→ assume a peça necessária e declara por ela.
```

Se não:

```text
JOGADOR IA EVENTUAL
→ nenhum personagem eventual precisa de decisão nesta janela.
```

A persona pode operar mais de uma peça eventual, mas cada uma mantém conhecimento, objetivos e decisões separados.

# 4. OPOSITOR — promotoria

Antes do julgamento, o OPOSITOR consulta os ganchos e fatos disponíveis e pergunta:

> **O que daqui eu posso usar para movimentar, pressionar ou fazer um plano adversário avançar?**

Pode declarar:

- retomada de gancho;
- reação de NPC;
- cobrança;
- retorno;
- pressão emocional;
- oportunidade;
- visita;
- conflito;
- ameaça;
- plano de antagonista;
- preparação futura;
- uso de NPCs ou recursos legitimamente disponíveis;
- nenhuma intervenção.

Exemplo doméstico:

```text
GANCHO
→ Ravena sente ciúme de Fulana quando ela está perto de Corvin.

CORVIN
→ vou passar a semana fora.

OPOSITOR
→ essa ausência pode reacender a dúvida de Ravena sobre Fulana.
```

Exemplo adversarial:

```text
GANCHO
→ Trigon quer usar Ravena para abrir caminho à Terra.

OPOSITOR
→ quero tentar capturá-la esta noite usando agentes disponíveis.
```

A declaração ainda não é resultado.

## Arquivo de ganchos

Quando houver ganchos ativos, o OPOSITOR pode consultar:

```text
campanhas/<nome>/mestre/ganchos-do-opositor.md
```

Esse arquivo contém apenas oportunidades atuais e é atualizado conforme `../agencia/ganchos-do-opositor.md`.

# 5. NARRADOR JULGA

O NARRADOR funciona como juiz.

Ele não cria nova oposição e não procura uma saída melhor para nenhum lado.

Consulta somente o necessário para decidir:

```text
DECLARAÇÕES
FICHAS
REGRAS
CENÁRIO
ESTADO ATUAL
CONHECIMENTO
MEIOS
OPORTUNIDADE
FATOS RELEVANTES
```

A pergunta é:

> **Diante do que foi apresentado e do que já é verdade, o que realmente pode acontecer e qual é o resultado?**

Quando o resultado for óbvio pelos fatos e capacidades, não criar incerteza artificial apenas para produzir teste.

Quando existir incerteza real que as regras mandem resolver, aplicar `../resolucao/`.

## Julgar proposta do OPOSITOR

Uma proposta pode ser:

```text
VÁLIDA AGORA
→ possui fundamento, meios e oportunidade.

INVÁLIDA
→ falta fundamento ou contradiz a realidade.

VÁLIDA, MAS AINDA NÃO
→ exige prazo, preparação, deslocamento ou condição futura.
```

Exemplo:

```text
OPOSITOR
→ Trigon envia um agente.

NARRADOR
→ a tentativa é possível, mas colocar esse agente na região exige três dias.
```

Se essa preparação continuar relevante, ela pode virar ou atualizar um gancho do OPOSITOR.

## In dubio pro reo

O julgamento segue esta ordem:

```text
FATO CLARO
→ aplicar.

REGRA CLARA
→ aplicar.

INCERTEZA QUE EXIGE RESOLUÇÃO
→ usar a mecânica.

DÚVIDA REAL QUE RESTOU ENTRE INTERPRETAÇÕES IGUALMENTE PLAUSÍVEIS
→ favorecer os jogadores.
```

> **In dubio pro reo — na dúvida genuína, favoreça a defesa.**

Isso não apaga consequência clara e não substitui uma resolução mecânica necessária.

# NPCs e delegação ao OPOSITOR

O OPOSITOR não controla automaticamente todas as forças do mundo.

Quando quiser usar uma peça adversária, o NARRADOR julga se ela realmente está disponível.

Exemplo:

```text
OPOSITOR
→ quero usar a polícia que já procura Corvin para prendê-lo quando ele voltar.
```

O NARRADOR verifica:

```text
- existe fundamento para a polícia agir?
- ela sabe que Corvin voltou?
- possui meios?
- possui oportunidade?
- quais policiais realmente podem participar?
```

Se válido:

```text
NARRADOR
→ delega temporariamente os NPCs disponíveis ao OPOSITOR.

OPOSITOR
→ passa a jogar suas decisões naquela oposição.
```

Exemplo de combate:

```text
JOGADOR IA — RAVENA
            VS
OPOSITOR — agentes de Trigon

NARRADOR
→ juiz.
```

Durante a delegação, o OPOSITOR decide estratégia, ações, alvos e uso legítimo das capacidades das peças cedidas.

O NARRADOR continua apenas julgando.

Quando a oposição termina, a delegação termina.

# 6. NARRADOR NARRA A SENTENÇA

Depois de julgar, o NARRADOR transforma o resultado em cena.

A narração pode mostrar:

- o que realmente aconteceu;
- sucesso ou falha;
- consequência;
- mudança de posição;
- dano ou condição;
- reação observável;
- informação legitimamente percebida;
- nova situação.

Ele narra somente até o próximo ponto em que alguém precise decidir novamente.

Exemplo:

```text
JOGADOR HUMANO
→ atravesso o corredor e abro a porta.

OPOSITOR
→ um guarda autorizado entra no corredor antes disso.

NARRADOR
→ “Você cruza metade do corredor quando o guarda surge na esquina e o vê.”
```

A ação original não decide automaticamente se o personagem luta, foge, engana ou continua andando.

Nesse ponto abre-se nova janela.

> **A sentença termina onde consequência volta a ser escolha.**

# 7. NARRADOR REGISTRA

Depois da sentença, o NARRADOR registra somente o que realmente passou a ser verdade.

Conforme o caso:

```text
estado/atual.md
→ situação presente.

mestre/ganchos-do-opositor.md
→ pontas, planos ou oportunidades que continuam vivos.

mundo/
→ nova verdade estável quando apropriado.

ficha
→ mudança estável conforme as regras de aprovação.

livro/
→ história efetivamente ocorrida quando consolidada.
```

Registrar não cria nova consequência.

Se um gancho foi resolvido, removê-lo. Se mudou, atualizá-lo. Se a sentença produziu nova ponta útil, ela pode ser adicionada.

# Nenhum movimento também é válido

O OPOSITOR não precisa produzir intervenção em toda janela.

```text
OPOSITOR
→ nenhuma intervenção; a cena já está avançando por suas próprias decisões.
```

Isso é especialmente importante em romance, conversa, cotidiano, investigação ou qualquer cena que já esteja gerando escolhas suficientes.

# Regra contra correção retroativa

Depois da sentença, nenhuma persona adiciona um fato anterior apenas para alterar o resultado.

O OPOSITOR não pode inventar nova oposição retroativa.

O NARRADOR não pode inventar dificuldade retroativa.

Se o resultado criar nova oportunidade legítima, isso pertence à próxima janela.

# Regra final

> **Cada janela é uma pequena audiência: os jogadores apresentam as ações de suas peças; o OPOSITOR apresenta a oposição ou oportunidade que quer movimentar; o NARRADOR julga, narra a sentença e registra. A intenção continua enquanto ainda cobre o fluxo; competência evidente conta sem pedido; combate usa o mesmo motor; e, na dúvida genuína que restar depois das regras e fatos aplicáveis, in dubio pro reo.**