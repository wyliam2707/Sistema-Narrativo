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

Essas são as entradas principais. Não criar pastas adicionais apenas para antecipar necessidades futuras.

## Materialização no momento do nome

Assim que o nome da campanha for definido e estiver disponível:

```text
nome definido
→ criar campanhas/<nome>/
→ criar estrutura-base
→ criar arquivos operacionais obrigatórios
→ continuar a criação
```

A campanha já deve existir fisicamente mesmo antes de suas fichas estarem revisadas.

## Modelos obrigatórios da estrutura-base

Ao criar uma nova campanha, usar **exatamente** estes textos iniciais. Não improvisar versões diferentes entre campanhas.

### `personagens/README.md`

```text
# Personagens

Esta pasta guarda as fichas dos personagens com agência da campanha.

Cada personagem possui seu próprio arquivo.

Modelo e regras:
→ sistema/personagem/ficha.md
```

### `mundo/README.md`

```text
# Mundo

Esta pasta guarda fatos estáveis e canônicos do cenário.

Situações momentâneas pertencem a estado/atual.md.

Regras de estrutura:
→ sistema/criacao/estrutura-da-campanha.md
```

### `mestre/README.md`

```text
# Mestre

Esta pasta guarda material reservado de condução.

Acesso a este conteúdo não cria conhecimento automático para as personagens.

Regras de estrutura:
→ sistema/criacao/estrutura-da-campanha.md
```

### `livro/README.md`

```text
# Livro

Esta pasta guarda apenas capítulos já ocorridos, em numeração sequencial.

O ponto atual da campanha pertence a estado/atual.md.

Regras de estrutura:
→ sistema/criacao/estrutura-da-campanha.md
```

### `estado/atual.md`

```text
# Estado atual

Campanha em criação.

A situação inicial será registrada aqui quando definida.
```

> **Mesma estrutura-base → mesmos arquivos iniciais → nenhuma variação de texto entre IAs.**

# Função de cada entrada

## `README.md`

É a porta de entrada e o **índice operacional** da campanha.

Deve conter somente o necessário para identificar a campanha, localizar suas peças e saber onde continuar.

Estrutura lógica:

```text
Checkpoint da criação
1 - Nome da campanha
2 - Direção narrativa
3 - Cenário
4 - Personagens com agência
5 - Situação de entrada
6 - Mapa de consulta
```

### Checkpoint da criação

Enquanto a criação estiver em andamento, registrar somente o ponto operacional atual.

Exemplo:

```text
CRIAÇÃO: EM ANDAMENTO

Etapa atual: Revisão das fichas
Personagem atual: Ravena
Bloco atual: 3 - Poderes e capacidades
```

Ao terminar:

```text
CRIAÇÃO: CONCLUÍDA
```

O checkpoint não replica ficha, cenário ou estado.

> **O conteúdo pertence aos arquivos concretos. O checkpoint diz somente onde continuar.**

### Fonte principal de cada informação

```text
NOME DA CAMPANHA
→ README.md

DIREÇÃO NARRATIVA
→ resumo em README.md

CENÁRIO
→ resumo necessário em README.md
→ detalhes estáveis, quando necessários, em mundo/

PERSONAGEM COM AGÊNCIA
→ personagens/<nome>.md
→ Nome + Importância + CONTROLE no índice do README.md

REVISÃO DA FICHA
→ personagens/<nome>.md

INÍCIO DA HISTÓRIA
→ situação inicial concreta em estado/atual.md
→ README.md apenas aponta Situação de entrada para estado/atual.md

CHECKPOINT
→ README.md
```

> **Cada informação possui uma fonte principal. O README resume e orienta; não replica os arquivos concretos.**

### Personagens com agência

Cada personagem deve aparecer **individualmente** no índice.

Registrar:

```text
Nome — Importância — CONTROLE
```

Exemplo:

```text
Wyliam — Central — JOGADOR HUMANO
Ravena — Central — JOGADOR IA
Dick Grayson — Relevante — JOGADOR IA EVENTUAL
Kory — Central — JOGADOR IA EVENTUAL
```

A persona `JOGADOR IA EVENTUAL` pode operar mais de um personagem, mas isso não cria ficha ou identidade coletiva.

> **Persona compartilhada não cria ficha compartilhada.**

### Situação de entrada

Só é definida **depois que as fichas iniciais estiverem aprovadas**.

O README aponta para:

```text
estado/atual.md
```

Não duplicar o conteúdo da situação inicial no índice.

### Mapa de consulta

```text
personagens/ → fichas
estado/      → situação atual
mundo/       → cenário persistente
mestre/      → material reservado
livro/       → história ocorrida
```

# `personagens/`

Guarda as fichas dos personagens com agência de jogador.

Cada personagem possui um arquivo próprio:

```text
personagens/
├── README.md
├── wyliam.md
├── ravena.md
├── dick-grayson.md
└── kory.md
```

Não separar por padrão em subpastas de tipo de controle.

## Nascimento obrigatório da ficha

Toda ficha apresentável ao jogador usa desde o primeiro momento o modelo completo de:

```text
sistema/personagem/ficha.md
```

Antes da revisão, somente três informações recebem conteúdo:

```text
NOME
IMPORTÂNCIA
CONTROLE
```

O arquivo nasce como:

```text
Status: PENDENTE DE REVISÃO
```

Os demais campos e seções do modelo já existem, mas permanecem vazios até o bloco correspondente da revisão.

```text
NOME + IMPORTÂNCIA + CONTROLE
→ criar arquivo individual
→ copiar modelo-base completo
→ deixar o restante em branco
→ revisão posterior
```

> **A ficha nasce completa em estrutura e mínima em conteúdo.**

VIDA atual, ENERGIA atual, localização, condições, efeitos ativos e outros estados circunstanciais pertencem a `estado/atual.md`, não à ficha apenas por estarem ativos agora.

NPCs comuns não pertencem por padrão a `personagens/`; quando precisarem de persistência reservada, pertencem a `mestre/`.

# `estado/`

Guarda a realidade dinâmica atual da campanha.

Por padrão:

```text
estado/
└── atual.md
```

Durante a criação, o arquivo permanece com o modelo mínimo até a etapa **Início da história**, que ocorre somente depois da aprovação das fichas iniciais.

Quando a abertura for definida, `atual.md` passa a registrar somente o necessário para continuar corretamente daquele ponto.

Pode conter, quando existirem:

- momento atual;
- localização atual;
- VIDA e ENERGIA atuais;
- STATUS, condições e efeitos ativos;
- situações em andamento;
- intenções futuras ainda ativas;
- fios causais pendentes;
- outras informações operacionais necessárias para retomada.

Não criar por padrão arquivos separados como:

```text
status.md
progressao.md
cronologia.md
intencoes.md
```

`atual.md` substitui o retrato anterior pelo presente. Não é diário da sessão.

> **`estado/atual.md` responde: “Se outra IA assumir agora, o que precisa saber para continuar corretamente?”**

# `mundo/`

Guarda a memória canônica estável do cenário.

Criar arquivos além do README apenas quando houver conteúdo concreto suficiente.

Podem pertencer a `mundo/`:

- lugares;
- organizações;
- sociedades;
- regras próprias do cenário;
- fatos históricos necessários;
- estruturas e instalações estabelecidas;
- fenômenos persistentes;
- outras verdades estáveis do mundo.

`mundo/` não registra o estado momentâneo desses elementos.

> **`mundo/` guarda o que existe de forma estabelecida. `estado/` guarda como isso está agora.**

# `mestre/`

Guarda material reservado de condução que precisa persistir sem se tornar automaticamente conhecimento das personagens.

Podem pertencer a `mestre/`:

- NPCs persistentes sem agência de jogador;
- adversários;
- intenções e planos de NPCs;
- segredos estabelecidos;
- ameaças em preparação;
- informações reservadas necessárias à continuidade.

Quando a quantidade justificar:

```text
mestre/npcs/
```

Acesso da persona ao conteúdo de `mestre/` não concede esse conhecimento às peças que ela movimenta.

> **`mestre/` guarda verdades e intenções reservadas de condução. Acesso ao arquivo não cria metaconhecimento.**

# `livro/`

Guarda apenas a história que realmente aconteceu, consolidada em capítulos.

Depois que capítulos existirem:

```text
livro/
├── README.md
├── 001.md
├── 002.md
└── ...
```

Não guardar planos, possibilidades futuras ou acontecimentos ainda dependentes de decisão.

```text
livro/002.md    → o que aconteceu
estado/atual.md → de onde continuar
mestre/         → o que permanece reservado
```

> **`livro/` registra o que aconteceu. Nunca determina antecipadamente o que ainda deve acontecer.**

# Separação central

```text
PERSONAGENS → quem são as peças
ESTADO      → como as coisas estão agora
MUNDO       → o que existe
MESTRE      → o que é reservado à condução
LIVRO       → o que aconteceu
```

Não criar por padrão pastas como:

```text
cronologia/
relacionamento/
progressao/
diretrizes/
```

Novas subdivisões só surgem por necessidade concreta.

## Campanhas novas e material legado

O padrão atual é:

```text
campanhas/<nome>/
```

Material antigo em `aventuras/` permanece legado até migração explícita. Não mover, apagar ou reestruturar automaticamente.
