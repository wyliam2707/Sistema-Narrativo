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

Porta de entrada e **índice operacional** da campanha.

Deve permitir que uma IA ou narrador identifique rapidamente o que é a campanha, quais peças com agência existem e onde consultar cada tipo de informação.

O `README.md` deve conter somente o necessário para orientação inicial:

```text
1 - Nome da campanha
2 - Direção narrativa
3 - Cenário
4 - Personagens com agência
5 - Situação de entrada
6 - Mapa de consulta
```

#### Nome da campanha

Identifica a campanha.

#### Direção narrativa

Resumo curto do tom, foco e proposta narrativa já aprovados.

Não repetir toda a discussão de criação.

#### Cenário

Resumo curto do universo e das premissas necessárias para compreender onde a campanha acontece.

Detalhes persistentes de mundo pertencem a `mundo/`.

#### Personagens com agência

Registrar somente identificação e gerência suficientes para localizar as peças principais.

Exemplo:

```text
Wyliam — JOGADOR HUMANO
Ravena — JOGADOR IA
Titãs — JOGADOR IA EVENTUAL
```

As fichas completas pertencem a `personagens/`.

#### Situação de entrada

Indica de onde a campanha deve ser retomada.

No início da campanha, aponta para o resumo inicial aprovado. Durante o jogo, deve orientar para o estado atual sem duplicá-lo no `README.md`.

#### Mapa de consulta

Deve indicar de forma curta onde cada categoria de informação está armazenada:

```text
personagens/ → fichas
estado/      → situação atual
mundo/       → cenário persistente
mestre/      → material reservado
livro/       → história ocorrida
```

> **O README orienta. Ele não replica os arquivos da campanha.**

Não guardar nele ficha completa, STATUS detalhado, cronologia extensa, capítulos, planos secretos ou material reservado do mestre.

### `personagens/`

Guarda as fichas dos personagens com agência de jogador:

- protagonista;
- personagens `JOGADOR IA`;
- personagens administrados por `JOGADOR IA EVENTUAL`.

Cada personagem com agência possui **um arquivo próprio**, independentemente do tipo de controle.

Exemplo:

```text
personagens/
├── wyliam.md
├── ravena.md
├── dick-grayson.md
└── kory.md
```

Não separar por padrão em subpastas como:

```text
humanos/
jogadores-ia/
eventuais/
```

O tipo de controle pertence à própria ficha, por meio do campo `CONTROLE`, e não precisa ser duplicado no caminho do arquivo.

NPCs comuns, aliados ocasionais, figurantes e adversários não pertencem a `personagens/`; quando precisarem de persistência, ficam sob a estrutura reservada de `mestre/`.

> **Cada personagem com agência possui sua própria ficha. O tipo de controle pertence à ficha, não à pasta.**

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
