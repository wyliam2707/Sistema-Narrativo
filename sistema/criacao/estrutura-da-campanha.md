# Estrutura da campanha

Status: EM REVISÃO

Este arquivo define **onde o conteúdo concreto de uma campanha deve ser salvo**.

As regras de criação pertencem a `sistema/criacao/`. Os dados produzidos durante a criação e durante o jogo pertencem a:

```text
campanhas/<nome-da-campanha>/
```

> **O sistema ensina como operar. A campanha guarda a realidade concreta que será jogada.**

## Estrutura mínima

Toda nova campanha usa como base:

```text
campanhas/<nome-da-campanha>/
├── README.md
├── personagens/
├── estado/
├── mundo/
├── mestre/
└── livro/
```

Essas são as entradas principais. Não criar pastas adicionais apenas para antecipar necessidades futuras.

## Função de cada entrada

### `README.md`

Porta de entrada da campanha.

Deve permitir que uma IA ou narrador identifique o que é a campanha e como começar a consultá-la.

### `personagens/`

Guarda as fichas dos personagens com agência de jogador:

- protagonista;
- personagens `JOGADOR IA`;
- personagens administrados por `JOGADOR IA EVENTUAL`.

### `estado/`

Guarda a realidade dinâmica atual da campanha: aquilo que pode mudar durante o jogo e precisa ser retomado corretamente depois.

### `mundo/`

Guarda fatos estabelecidos do cenário que precisam persistir, como lugares, organizações, regras próprias daquela campanha e outros elementos de mundo relevantes.

### `mestre/`

Guarda material reservado de condução, como NPCs persistentes, adversários, planos, segredos e outros elementos que não devem ser tratados automaticamente como conhecimento dos jogadores.

### `livro/`

Guarda a narrativa já ocorrida: capítulos e registro literário da história.

## Separação central

```text
PERSONAGENS → quem são as peças
ESTADO      → como as coisas estão agora
MUNDO       → o que existe
MESTRE      → o que é reservado à condução
LIVRO       → o que aconteceu
```

> **Cada informação deve ser salva no lugar que representa sua função, não em uma pasta nova criada apenas para aquele assunto.**

## Estrutura enxuta

Não criar por padrão pastas separadas como:

```text
cronologia/
relacionamento/
progressao/
diretrizes/
```

Esses conteúdos devem ser absorvidos pelas entradas principais quando fizer sentido.

Novas subdivisões só devem existir quando surgir uma necessidade concreta durante o uso do sistema.

## Campanhas novas e material legado

O padrão para novas campanhas é `campanhas/`.

Material antigo que ainda esteja em `aventuras/` permanece preservado como legado até uma migração explícita. Não mover, apagar ou reestruturar campanhas antigas automaticamente.
