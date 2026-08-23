# Pendências — revisão do processo de criação de campanha

Este arquivo permite retomar a revisão em outro chat sem depender da conversa anterior.

Status geral: CICLO 1–10 CONCLUÍDO
Branch de trabalho: `revisao/personagem`

## Regra de trabalho

Revisar **um ponto por vez**.

```text
apresentar 1 ponto
→ discutir até chegar a um entendimento comum
→ somente depois da aprovação, registrar nos arquivos do sistema
→ seguir para o próximo ponto
```

Não alterar vários pontos de uma vez.

## Pontos concluídos

### Ponto 1 — checkpoint da criação

APROVADO E REGISTRADO.

> **O README da própria campanha guarda somente o ponto operacional de retomada da criação.**

### Ponto 2 — destino exato de cada etapa

APROVADO E REGISTRADO.

> **Cada informação possui uma fonte principal. O README resume e orienta; não duplica o conteúdo dos arquivos concretos.**

### Ponto 3 — salvamento durante a revisão mecânica

APROVADO E REGISTRADO.

> **Cada bloco mecânico aprovado é persistido imediatamente. Conteúdo ainda em discussão não é salvo. Depois do salvamento, o checkpoint avança.**

### Ponto 4 — hand-off para `estado/atual.md`

APROVADO E REGISTRADO.

> **Quando todas as fichas forem aprovadas, o sistema consolida automaticamente a situação inicial em `estado/atual.md`, marca `CRIAÇÃO: CONCLUÍDA` e somente então o NARRADOR abre a primeira cena.**

### Ponto 5 — GERÊNCIA e CONTROLE

APROVADO E REGISTRADO.

> **GERÊNCIA é o processo de decidir quem controla a personagem. O resultado é persistido exclusivamente no campo `CONTROLE`.**

### Ponto 6 — personagens eventuais

APROVADO E REGISTRADO.

> **Cada personagem com agência é uma peça própria, aparece individualmente no índice e possui sua própria ficha.**

A persona `JOGADOR IA EVENTUAL` pode ser compartilhada por várias peças sem criar ficha compartilhada.

### Ponto 7 — personagens conhecidos e versões

APROVADO E REGISTRADO.

> **Personagens conhecidos usam a versão escolhida pelo jogador como base. O jogador pode modificar, combinar ou substituir elementos. A versão consolidada torna-se a referência canônica local da campanha.**

### Ponto 8 — nome de campanha já existente

APROVADO E REGISTRADO.

> **Nova criação nunca sobrescreve automaticamente uma campanha existente.**

A verificação acontece antes de criar qualquer arquivo.

### Ponto 9 — modelos determinísticos dos arquivos automáticos

APROVADO E REGISTRADO.

> **Os arquivos operacionais da estrutura-base possuem textos iniciais obrigatórios e determinísticos.**

Modelos definidos para:

```text
personagens/README.md
mundo/README.md
mestre/README.md
livro/README.md
estado/atual.md
```

Fonte canônica única dos textos:

```text
sistema/criacao/estrutura-da-campanha.md
```

Commit principal:

- `9c929d4b1461a01cc93ecec9ef414d14926f3c57`

### Ponto 10 — porta de entrada do repositório

APROVADO E REGISTRADO POR ORA.

Fluxo atual:

```text
NOVA CAMPANHA
→ sistema/criacao/README.md

CONTINUAR
→ campanhas/<nome>/README.md
```

O `README.md` da raiz e `sistema/00-LEIA-PRIMEIRO.md` foram alinhados ao novo fluxo.

Material antigo em `aventuras/` e `sistema/protocolo-de-criacao.md` permanece preservado como legado. Não apagar, mover ou migrar automaticamente.

Commits:

- `c9482040744d46d160e7d62a729e3a2c87c26f50` — `README.md`
- `43985d655981bf3de2aa41eddbe6280def34279c` — `sistema/00-LEIA-PRIMEIRO.md`

## Estrutura de campanha aprovada

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

Separação central:

```text
PERSONAGENS → quem são as peças
ESTADO      → como as coisas estão agora
MUNDO       → o que existe
MESTRE      → o que é reservado à condução
LIVRO       → o que aconteceu
```

## Arquivos principais desta revisão

```text
sistema/criacao/README.md
sistema/criacao/estrutura-da-campanha.md
sistema/criacao/PENDENCIAS.md
README.md
sistema/00-LEIA-PRIMEIRO.md
```

Antes de editar qualquer arquivo existente, buscar seu SHA atual.

## Ponto exato para retomar

O ciclo planejado de 10 pontos foi concluído.

Ao retomar esta revisão em outro chat:

```text
1 - ler sistema/criacao/PENDENCIAS.md
2 - considerar os Pontos 1–10 como aprovados e registrados
3 - não reabrir um ponto já fechado sem nova correção explícita do jogador
4 - iniciar nova revisão somente a partir de uma nova necessidade concreta
```
