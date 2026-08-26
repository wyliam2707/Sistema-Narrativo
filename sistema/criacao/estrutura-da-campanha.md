# Estrutura Inicial da Campanha

Status: APROVADO

Este arquivo define **qual estrutura `criacao/` deve materializar quando uma nova campanha nasce**.

Ele não redefine o significado persistente de cada fonte. Depois que a estrutura existe, as regras de onde registrar cada verdade pertencem a `../persistencia/`.

> **Criação materializa a casa. Persistência define onde cada informação mora.**

## Raiz permanente

A pasta `campanhas/` é uma raiz permanente e independente das campanhas individuais.

```text
campanhas/
├── README.md
├── <campanha-a>/
└── <campanha-b>/
```

`campanhas/README.md` não pertence a nenhuma campanha específica e não deve ser removido apenas porque existe uma única campanha.

Toda nova campanha nasce como subpasta de `campanhas/`.

## Estrutura-base obrigatória

Ao aprovar um nome livre, criar:

```text
campanhas/<nome>/
├── README.md
├── personagens/
│   └── README.md
├── estado/
│   └── atual.md
├── mundo/
│   └── README.md
├── mestre/
│   └── README.md
└── livro/
    └── README.md
```

Não criar subdivisões adicionais apenas para antecipar necessidades futuras.

As personas operacionais da campanha **não exigem uma pasta paralela**. Sua composição é registrada no `README.md` da própria campanha como `Mesa operacional`, conforme `start-da-campanha.md`.

## Momento da materialização

```text
nome aprovado e livre
→ garantir campanhas/README.md
→ criar campanhas/<nome>/
→ criar estrutura-base
→ preencher modelos mínimos
→ registrar checkpoint da criação
→ continuar README.md
```

A campanha já existe fisicamente enquanto suas fichas ainda estão em revisão.

## Modelos iniciais

### `personagens/README.md`

```text
# Personagens

Esta pasta guarda as fichas dos personagens com agência da campanha.

Cada personagem possui seu próprio arquivo.

Modelo da ficha:
→ sistema/personagem/ficha.md
```

### `mundo/README.md`

```text
# Mundo

Esta pasta guarda verdades estáveis e canônicas do cenário.

O presente operacional pertence a estado/atual.md.
```

### `mestre/README.md`

```text
# Mestre

Esta pasta guarda material reservado que precisa persistir sem se tornar automaticamente conhecimento das personagens.
```

### `livro/README.md`

```text
# Livro

Esta pasta guarda capítulos já ocorridos.

O ponto atual da campanha pertence a estado/atual.md.
```

### `estado/atual.md`

```text
# Estado atual

Campanha em criação.

A situação inicial será registrada aqui quando definida.
```

Esses textos são modelos mínimos. A semântica completa de cada destino pertence a `../persistencia/`.

## README da campanha durante a criação

O `README.md` da campanha funciona como índice, checkpoint e registro da composição operacional necessária para iniciar ou retomar a mesa.

Durante a criação:

```text
CRIAÇÃO: EM ANDAMENTO

Etapa atual: ...
Personagem atual: ...     # quando aplicável
Bloco atual: ...          # quando aplicável
```

Na etapa final:

```text
CRIAÇÃO: EM ANDAMENTO
Etapa atual: CHECK DE START
```

Ao terminar:

```text
CRIAÇÃO: CONCLUÍDA
```

O checkpoint registra **onde retomar**, não replica ficha, cenário ou estado.

## Índice de personagens com agência

Cada personagem com agência aparece individualmente no índice:

```text
Nome — Importância — CONTROLE
```

Exemplo estrutural:

```text
Protagonista — Central — JOGADOR HUMANO
Aliada — Central — JOGADOR IA
Contato — Relevante — JOGADOR IA EVENTUAL
```

Persona compartilhada não cria ficha compartilhada.

As fichas concretas ficam em:

```text
campanhas/<nome>/personagens/<personagem>.md
```

O nascimento e a revisão seguem `personagem.md`.

## Mesa operacional

Antes do START, o README da campanha deve ganhar uma seção:

```text
## Mesa operacional

JOGADOR HUMANO → <personagem>
JOGADOR IA — <personagem> → <personagem>
JOGADOR IA EVENTUAL → ATIVO
OPOSITOR → ATIVO
NARRADOR → ATIVO
```

Para cada ficha com:

```text
CONTROLE: JOGADOR IA
```

incluir uma linha própria de `JOGADOR IA — <personagem>`.

Exemplo:

```text
## Mesa operacional

JOGADOR HUMANO → Kael
JOGADOR IA — Ravena → Ravena
JOGADOR IA — Wanda → Wanda
JOGADOR IA EVENTUAL → ATIVO
OPOSITOR → ATIVO
NARRADOR → ATIVO
```

Essa seção registra o arranjo de autoridade da mesa e permite reinstanciar as mesmas personas ao continuar a campanha.

Ela não substitui `CONTROLE` nas fichas e não duplica conteúdo de personagem.

A composição só é registrada como pronta depois do processo de `start-da-campanha.md`.

## Situação inicial

Durante a criação, `estado/atual.md` permanece mínimo até a etapa **Início da história**.

Depois das fichas aprovadas e do pareamento concluído, registrar o ponto inicial aprovado conforme `README.md` e `../persistencia/estado-atual.md`.

Quando não houver desgaste inicial estabelecido:

```text
Vida atual = Vida Máxima
Mana atual = Mana Máxima
```

Para a peça com `CONTROLE: JOGADOR HUMANO`:

```text
Trama [30]
```

Não usar `ENERGIA` como reserva universal.

Estado inicial pronto não significa START autorizado. A Mesa operacional ainda precisa passar pelo `CHECK DE START`.

## O que este arquivo NÃO decide

Depois de criar as pastas, este arquivo não decide:

- se uma informação pertence à ficha;
- quando atualizar `estado/atual.md`;
- onde guardar consequência causal;
- onde guardar NPC reservado;
- como consolidar Livro;
- como corrigir cânone;
- qual decisão uma persona tomará durante o jogo.

Essas decisões pertencem às áreas responsáveis.

Quem controla personagens e o que cada persona pode decidir pertence a `../personas/`.

## Material legado

Material em `aventuras/` permanece legado até migração explícita.

Não mover, apagar ou reestruturar automaticamente durante a criação de uma campanha nova.

## Regra final

> **`estrutura-da-campanha.md` define o scaffold inicial e o lugar em que a Mesa operacional é registrada. A primeira cena continua bloqueada até `start-da-campanha.md` confirmar que todas as personas necessárias estão prontas.**
