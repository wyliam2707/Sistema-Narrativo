# Persistência

Status: APROVADO

Esta pasta responde:

> **O que precisa continuar verdadeiro depois da cena e em qual fonte isso deve ser registrado?**

Persistência não cria fatos, não calcula resultados e não decide ações. Ela registra verdades já estabelecidas na fonte correta.

## Estrutura

```text
persistencia/
├── README.md
├── estado-atual.md
├── salvar-estado.md
├── status.md
├── progressao.md
├── relevancia-da-ficha.md
├── atualizacao-de-ficha.md
├── material-reservado.md
├── livro.md
├── fechamento-de-capitulo.md
└── correcao-de-canone.md
```

## Identidades internas

### `estado-atual.md`

Define o retrato concreto de retomada:

```text
campanhas/<nome>/estado/atual.md
```

Guarda o presente necessário para continuar corretamente.

### `salvar-estado.md`

Preserva o ponto atual sem fechar capítulo nem criar nova ficção.

### `status.md`

Define **STATUS persistente**: como a peça está agora — Vida, Mana, Trama quando aplicável, condições mecânicas, efeitos ativos, Barreiras, alterações temporárias e posição relevante.

A mecânica dos Status pertence a `../resolucao/status/`.

### `progressao.md`

Registra consequências já estabelecidas que continuam causalmente vivas.

Não significa XP, evolução de poder ou crescimento mecânico.

### `relevancia-da-ficha.md`

Define **o que merece ser consolidado numa ficha** e evita guardar meta-informação ou redundância sem utilidade futura.

A estrutura e significado dos campos continuam em `../personagem/ficha.md`.

### `atualizacao-de-ficha.md`

Define quando uma mudança deixa de ser apenas estado e passa a integrar de forma estável quem a personagem é.

Mudança permanente segue a aprovação prevista nesse arquivo.

### `material-reservado.md`

Define o uso de:

```text
campanhas/<nome>/mestre/
```

para NPCs persistentes sem agência de jogador, segredos, planos, preparações e outras fontes reservadas.

### `livro.md`

Define o registro histórico literário do que realmente aconteceu.

### `fechamento-de-capitulo.md`

Consolida uma unidade narrativa encerrada e atualiza somente as fontes que precisam continuar válidas.

### `correcao-de-canone.md`

Define como uma correção aprovada substitui a versão anterior sem manter duas realidades concorrentes.

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
→ quem as peças são

ESTADO
→ como continuar agora

MUNDO
→ verdades estáveis do cenário

MESTRE
→ material reservado

LIVRO
→ o que aconteceu
```

## Regra contra duplicação

Um conceito do sistema não exige automaticamente um arquivo homônimo dentro da campanha.

Não criar por padrão arquivos paralelos de STATUS, Progressão, cronologia ou intenções quando a mesma informação já possui fonte canônica suficiente.

> **Cada verdade deve ter uma fonte principal.**

## Fronteiras

```text
como construir inicialmente?      → ../criacao/
quem a personagem é?              → ../personagem/
quem decide?                       → ../personas/
quais fios podem voltar a agir?    → ../agencia/
como calcular consequência?        → ../resolucao/
quando registrar?                  → ../operacao/
como apresentar?                   → ../narracao/
onde a verdade permanece?          → persistencia/
```

## Regra final

> **`persistencia/` é a memória canônica do sistema. Ela não cria a verdade: guarda cada verdade já estabelecida uma única vez, na fonte correta.**
