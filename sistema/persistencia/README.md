# Persistência

Status: APROVADO

Esta pasta responde:

> **O que precisa continuar verdadeiro depois da cena e em qual fonte da campanha isso deve ser registrado?**

Persistência não cria fatos. Ela registra fatos já estabelecidos na fonte correta.

## Estrutura canônica

```text
persistencia/
├── README.md
├── estado-atual.md
├── salvar-estado.md
├── status.md
├── progressao.md
├── atualizacao-de-ficha.md
├── material-reservado.md
├── livro.md
├── fechamento-de-capitulo.md
└── correcao-de-canone.md
```

## Arquivos

### `estado-atual.md`

Define a fonte concreta de retomada:

```text
campanhas/<nome>/estado/atual.md
```

Guarda somente o presente necessário para continuar corretamente.

### `salvar-estado.md`

Define como preservar o ponto atual sem fechar capítulo nem criar nova ficção.

### `status.md`

Define o conceito de STATUS: como uma peça está agora — Vida, Dano acumulado, Energia, Condições, Efeitos Ativos, Local e outros estados temporários relevantes.

Na campanha, STATUS persistente fica dentro de `estado/atual.md`; não exige arquivo próprio.

### `progressao.md`

Define consequências estabelecidas que continuam causalmente vivas.

Na campanha atual, esses fios ficam em `estado/atual.md`, ou em `mestre/` quando forem reservados. Não existe obrigação de criar `progressao.md` dentro da campanha.

### `atualizacao-de-ficha.md`

Define quando uma mudança deixa de ser apenas estado e passa a integrar de forma estável quem a personagem é.

Alteração permanente de ficha exige a aprovação prevista nesse arquivo.

### `material-reservado.md`

Define a função de:

```text
campanhas/<nome>/mestre/
```

Ali ficam NPCs persistentes sem agência de jogador, segredos, planos, preparações e outras fontes reservadas.

### `livro.md`

Define o registro histórico literário do que realmente aconteceu.

Capítulos pertencem a:

```text
campanhas/<nome>/livro/
```

O Livro não é a fonte operacional padrão de retomada.

### `fechamento-de-capitulo.md`

Define a consolidação de uma unidade narrativa encerrada no Livro e a atualização das fontes necessárias para continuar.

### `correcao-de-canone.md`

Define como uma correção explicitamente aprovada substitui a versão anterior de um fato sem manter duas realidades concorrentes.

## Estrutura concreta da campanha

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

Distribuição básica:

```text
PERSONAGENS
→ quem as peças com agência são.

ESTADO / atual.md
→ como continuar agora.

MUNDO
→ verdades estáveis do cenário.

MESTRE
→ NPCs e material reservado.

LIVRO
→ o que aconteceu.
```

## Regra contra duplicação

Um conceito do sistema não exige automaticamente um arquivo homônimo na campanha.

Não criar por padrão:

```text
status.md da campanha
progressao.md da campanha
cronologia.md
intencoes.md
```

Se a mesma informação já possui fonte canônica suficiente, não duplicá-la em outra camada.

## Relação com as outras áreas

```text
personagem/
→ define quem a peça é.

resolucao/
→ estabelece consequências mecânicas.

agencia/ e personas/
→ definem quem decide e quais fios podem se mover.

operacao/
→ define quando julgar, narrar e registrar.

narracao/
→ apresenta a sentença.

persistencia/
→ preserva somente o que passou a ser verdade.
```

## Regra final

> **README roteia. `estado-atual.md` guarda o presente; `mestre/` guarda o reservado; `livro/` guarda a história; fichas guardam mudanças estáveis. Persistir corretamente é registrar cada verdade uma única vez na fonte certa.**