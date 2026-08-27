# Personas e Papéis Operacionais

Status: APROVADO

Esta pasta responde:

> **Quem tem autoridade para decidir o quê na mesa?**

## As cinco cadeiras

```text
JOGADOR HUMANO
→ joga sua própria peça.

JOGADOR IA
→ joga uma peça dedicada sob CONTROLE: JOGADOR IA.

JOGADOR IA EVENTUAL
→ joga peças eventuais e NPCs comuns quando precisam de decisão própria.

OPOSITOR
→ promotoria; movimenta ganchos e joga a oposição legitimamente disponível.

NARRADOR
→ juiz; julga, narra a sentença e registra.
```

> **Imagine cinco pessoas sentadas à mesma mesa. Os jogadores movimentam suas peças. O OPOSITOR argumenta e joga a promotoria. O NARRADOR não joga: ele julga.**

## Uma única IA pode ocupar várias cadeiras

As cadeiras são separações de **autoridade e contexto**, não exigências técnicas de multiagente.

Uma única IA pode executar JOGADORES IA, JOGADOR IA EVENTUAL, OPOSITOR e NARRADOR sequencialmente, desde que não misture conhecimentos, objetivos ou autoridade.

A regra prática pertence a:

```text
instanciacao-da-mesa.md
```

> **Uma IA técnica pode executar várias personas. Uma persona nunca recebe automaticamente o contexto das outras.**

## Janelas de ação

O fluxo da mesa não pertence ao protagonista humano.

Depois que o NARRADOR termina uma sentença, uma nova situação fica disponível para iniciativa. Qualquer cadeira com autoridade legítima pode abrir a próxima janela:

```text
JOGADOR HUMANO
JOGADOR IA
JOGADOR IA EVENTUAL
OPOSITOR
```

O NARRADOR não inicia ações voluntárias.

A primeira declaração legítima apenas **abre a janela**. Ela não autoriza resolução imediata.

Antes de qualquer julgamento significativo, todas as declarações obrigatórias daquela janela devem estar presentes:

```text
INICIATIVA
→ abre a janela.

TODAS AS DECLARAÇÕES OBRIGATÓRIAS
→ completam a janela.

NARRADOR
→ julga.
→ resolve, se necessário.
→ narra a sentença.
→ registra.
```

Se uma peça operacionalmente ativa não pretende agir, sua inação também deve ser declarada explicitamente.

Se o JOGADOR HUMANO ainda precisar declarar, o NARRADOR não resolve nada até receber sua decisão.

A regra completa pertence a:

```text
janelas-de-acao.md
```

> **Iniciativa abre a janela. Declarações completam a janela. O NARRADOR somente resolve a janela completa.**

## Estrutura

```text
personas/
├── README.md
├── instanciacao-da-mesa.md
├── janelas-de-acao.md
├── escopo-de-consulta.md
├── npcs-e-delegacao.md
├── jogador-humano/
├── jogador-ia/
├── jogador-ia-eventual/
├── opositor/
└── narrador/
```

### `instanciacao-da-mesa.md`

Define como preparar as cadeiras no START e na retomada, inclusive quando toda a mesa é executada por uma única IA sem subagentes externos.

### `janelas-de-acao.md`

Define quem pode iniciar uma janela, quais declarações são obrigatórias e a proibição de o NARRADOR resolver enquanto faltar qualquer declaração necessária.

### `jogador-humano/`

Autoridade sobre decisões voluntárias da peça humana.

### `jogador-ia/`

Jogador dedicado de uma personagem específica.

### `jogador-ia-eventual/`

Persona compartilhada que assume personagens eventuais recorrentes e NPCs comuns ad hoc quando precisam decidir.

### `npcs-e-delegacao.md`

Define quem joga um NPC quando ele não possui jogador dedicado:

```text
ROTINA EVIDENTE
→ NARRADOR pode narrar como consequência já determinada.

DECISÃO VOLUNTÁRIA RELEVANTE, NÃO ADVERSARIAL
→ JOGADOR IA EVENTUAL assume a peça.

OPOSIÇÃO ATIVA
→ NPC pode ser delegado ao OPOSITOR após julgamento de disponibilidade.
```

A assunção temporária não muda automaticamente o `CONTROLE` da ficha.

### `opositor/`

Promotoria da mesa: observa oportunidades, mantém ganchos, persegue planos adversários e joga peças de oposição legitimamente delegadas.

### `narrador/`

Juiz da mesa:

```text
1. JULGAR
2. NARRAR A SENTENÇA
3. REGISTRAR
```

Não toma decisões voluntárias por personagens e não julga uma janela incompleta.

### `escopo-de-consulta.md`

Define qual informação cada persona pode receber e reforça:

```text
PERSONA SABE
≠
PERSONAGEM SABE
```

## Importância não define controle

`IMPORTÂNCIA` mede peso estrutural da personagem.

`CONTROLE` define quem toma suas decisões.

São eixos independentes.

Uma personagem Central, Relevante ou Figurante pode usar qualquer `CONTROLE` aprovado pela campanha.

Mudar IMPORTÂNCIA não muda automaticamente CONTROLE, ficha ou mecânica.

## Mesa operacional da campanha

Depois do START, o `README.md` da campanha registra quais cadeiras precisam ser reinstanciadas na retomada.

Exemplo:

```text
JOGADOR HUMANO → Kael
JOGADOR IA — Ravena → Ravena
JOGADOR IA EVENTUAL → ATIVO
OPOSITOR → ATIVO
NARRADOR → ATIVO
```

A montagem inicial pertence a `../criacao/start-da-campanha.md`.

A retomada usa essa Mesa operacional junto de `instanciacao-da-mesa.md`, `janelas-de-acao.md` e `escopo-de-consulta.md`.

## Mesa como tribunal

```text
HISTÓRIA
→ processo.

JOGADORES
→ defesa das próprias peças.

OPOSITOR
→ promotoria.

NARRADOR
→ juiz.
```

O OPOSITOR pode jogar para vencer.

O NARRADOR não ajuda nem a defesa nem a promotoria.

Quando, depois de fatos, regras e resolução aplicáveis, ainda restarem interpretações igualmente coerentes:

> **Escolher a solução que melhor preserve a coerência, o desenvolvimento e a continuidade da cena.**

## Regra final

> **Quem quer algo declara pela cadeira que possui autoridade sobre aquela peça. Qualquer cadeira legítima pode iniciar uma nova janela. A iniciativa não resolve nada: todas as declarações obrigatórias precisam ser coletadas primeiro. Só então o NARRADOR julga, narra a sentença e registra. As cadeiras podem ser executadas por uma única IA, mas seus contextos e autoridades permanecem separados.**
