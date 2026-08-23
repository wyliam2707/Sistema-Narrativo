# Persistência

Status: REFERÊNCIA PRINCIPAL

Esta pasta reúne as regras que respondem à pergunta:

> **O que precisa permanecer verdadeiro depois que a cena, sessão ou capítulo termina, e em qual fonte concreta da campanha isso deve ser registrado?**

## Princípio

Persistência não serve para repetir tudo que aconteceu.

Cada conceito do sistema guarda uma função diferente, mas isso **não significa que cada conceito precise virar um arquivo separado dentro da campanha**.

> **Conceito do sistema ≠ arquivo obrigatório da campanha.**

A estrutura concreta das campanhas atuais é definida por:

```text
sistema/criacao/estrutura-da-campanha.md
```

## Estrutura concreta atual

```text
campanhas/<nome>/
├── README.md
├── personagens/
├── estado/
│   └── atual.md
├── mundo/
├── mestre/
└── livro/
```

A persistência deve distribuir cada fato conforme sua função:

```text
FICHA / PERSONAGENS
→ quem a peça é e o que se consolidou nela

ESTADO / atual.md
→ como as coisas estão agora e quais fios operacionais continuam ativos

MUNDO
→ verdades estáveis do cenário

MESTRE
→ NPCs, fatos, planos, preparações e material reservado de condução

LIVRO
→ o que realmente aconteceu
```

## STATUS

`status.md` continua sendo a regra do sistema para **como um personagem está agora**.

STATUS pode incluir, quando relevantes:

- Vida atual;
- Dano acumulado;
- Energia atual;
- condições;
- efeitos ativos;
- localização;
- outras informações circunstanciais necessárias para resolução e continuidade.

Na campanha atual, esses dados não exigem um `status.md` próprio.

Quando precisam sobreviver à conversa, são registrados no retrato presente de:

```text
campanhas/<nome>/estado/atual.md
```

> **STATUS é um conceito operacional. `estado/atual.md` é sua fonte concreta de persistência na campanha.**

## Progressão

`progressao.md` continua definindo **consequências estabelecidas que ainda possuem potencial causal futuro**.

Favores, promessas, investigações abertas, ameaças, acessos, dívidas, intenções ainda ativas e fios causais semelhantes podem continuar sendo tratados conceitualmente como Progressão.

Na estrutura atual, Progressão não exige uma pasta nem um arquivo próprio.

Quando o fato ainda é necessário para continuar corretamente do presente, ele pertence a:

```text
estado/atual.md
```

Quando sua natureza muda:

```text
vira parte estável do personagem → personagens/<nome>.md
vira verdade estável do cenário  → mundo/
vira informação reservada        → mestre/
deixa de estar causalmente vivo   → permanece apenas no livro/
```

> **Progressão descreve a função causal do fato; a estrutura da campanha determina onde ele é persistido.**

## Livro

`livro.md` define a história realmente ocorrida.

Capítulos consolidados ficam em:

```text
campanhas/<nome>/livro/001.md
campanhas/<nome>/livro/002.md
...
```

O Livro é histórico. Não é o ponto operacional padrão de retomada da campanha.

## Material reservado

`material-reservado.md` define como fatos e agentes reservados são preservados sem se tornarem automaticamente conhecimento das personagens.

Seu destino concreto é:

```text
campanhas/<nome>/mestre/
```

NPCs persistentes sem agência de jogador também pertencem a essa área quando precisam de ficha ou continuidade própria.

## Atualização de ficha

`atualizacao-de-ficha.md` define quando uma consequência deixa de ser apenas estado e passa a integrar quem o personagem é.

Toda alteração permanente continua exigindo a autoridade prevista nessa regra.

Quando aprovada, atualizar a ficha canônica em:

```text
campanhas/<nome>/personagens/<personagem>.md
```

quando se tratar de personagem com agência de jogador.

NPCs persistentes continuam em `mestre/` enquanto permanecerem NPCs.

## Fechamento de capítulo

`fechamento-de-capitulo.md` define como consolidar a história e atualizar continuidade.

Quando ele manda atualizar `STATUS` ou `Progressão`, isso significa atualizar os fatos correspondentes dentro de `estado/atual.md` na estrutura atual, salvo quando a própria natureza do fato exigir outra fonte.

Fluxo prático:

```text
fechar capítulo
→ consolidar livro/<número>.md
→ atualizar estado/atual.md
→ atualizar fichas somente se algo mudou de forma estável
→ atualizar mundo/ somente se surgiu nova verdade estável
→ atualizar mestre/ somente se material reservado mudou
```

## Correção de cânone

`correcao-de-canone.md` continua definindo substituição de fatos incorretos ou contraditórios.

Correção não cria uma camada paralela: alinhar diretamente as fontes canônicas afetadas.

## Arquivos aprovados nesta área

- `status.md` — regra de estado circunstancial atual;
- `progressao.md` — regra de consequência causal ainda viva;
- `atualizacao-de-ficha.md` — mudança estável do personagem;
- `livro.md` — registro histórico canônico;
- `fechamento-de-capitulo.md` — salvamento de capítulo e continuidade;
- `material-reservado.md` — fatos, NPCs, planos e preparações reservados;
- `correcao-de-canone.md` — substituição explícita de cânone incorreto.

## Material legado

Arquivos antigos diretamente em `sistema/` permanecem preservados como fontes históricas de migração.

Quando contradisserem esta arquitetura ou `sistema/criacao/estrutura-da-campanha.md`, prevalece a estrutura atual explicitamente aprovada.

Não reintroduzir como obrigatórias camadas antigas como:

```text
status.md da campanha
progressao.md da campanha
cronologia.md
intencoes.md
```

A estrutura pode ser ampliada futuramente quando surgir necessidade concreta, mas não por antecipação nem para duplicar conteúdo já persistido.

> **Salvar corretamente é preservar a função do fato na fonte canônica certa, não criar um arquivo para cada conceito do sistema.**
