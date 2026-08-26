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

O `README.md` da campanha funciona como índice e checkpoint.

Durante a criação:

```text
CRIAÇÃO: EM ANDAMENTO

Etapa atual: ...
Personagem atual: ...     # quando aplicável
Bloco atual: ...          # quando aplicável
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

## O que este arquivo NÃO decide

Depois de criar as pastas, este arquivo não decide:

- se uma informação pertence à ficha;
- quando atualizar `estado/atual.md`;
- onde guardar consequência causal;
- onde guardar NPC reservado;
- como consolidar Livro;
- como corrigir cânone.

Essas decisões pertencem a `../persistencia/`.

Também não decide quem controla personagens; isso pertence a `../personas/`.

## Material legado

Material em `aventuras/` permanece legado até migração explícita.

Não mover, apagar ou reestruturar automaticamente durante a criação de uma campanha nova.

## Regra final

> **`estrutura-da-campanha.md` define apenas o scaffold inicial que `criacao/` cria. A vida posterior desses arquivos é governada por `persistencia/`.**
