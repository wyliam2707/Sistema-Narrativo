# Pendências — revisão do processo de criação de campanha

Este arquivo existe somente para permitir retomar a revisão em outro chat sem depender da conversa anterior.

Status geral: EM REVISÃO
Branch de trabalho: `revisao/personagem`

## Regra de trabalho

Revisar **um ponto por vez**.

Fluxo:

```text
apresentar 1 ponto
→ discutir até chegar a um entendimento comum
→ somente depois da aprovação, registrar nos arquivos do sistema
→ seguir para o próximo ponto
```

Não alterar vários pontos de uma vez.

## Já concluído

### Ponto 1 — checkpoint da criação

APROVADO E REGISTRADO.

A campanha usa o próprio `campanhas/<nome>/README.md` para registrar apenas onde retomar o processo de criação.

### Ponto 2 — destino exato de cada etapa

APROVADO E REGISTRADO.

Regra central:

> **Cada informação possui uma fonte principal. O README resume e orienta; não duplica o conteúdo dos arquivos concretos.**

### Ponto 3 — salvamento durante a revisão mecânica

APROVADO E REGISTRADO.

> **Durante a revisão mecânica, cada bloco passa a ser persistido imediatamente após sua aprovação. Conteúdo ainda em discussão não é salvo. Depois do salvamento, o checkpoint avança para o próximo bloco.**

### Ponto 4 — hand-off para `estado/atual.md` antes da primeira cena

APROVADO E REGISTRADO.

> **Quando todas as fichas forem aprovadas, o sistema consolida automaticamente a situação inicial em `estado/atual.md`, marca `CRIAÇÃO: CONCLUÍDA` no README da campanha e somente então o NARRADOR abre a primeira cena.**

### Ponto 5 — relação entre GERÊNCIA e CONTROLE

APROVADO E REGISTRADO.

> **GERÊNCIA é apenas o processo de decidir quem controla a personagem. O resultado dessa decisão é persistido exclusivamente no campo `CONTROLE`.**

### Ponto 6 — personagens eventuais no índice da campanha

APROVADO E REGISTRADO.

> **Cada personagem com agência é uma peça própria, deve aparecer individualmente no índice da campanha e possui sua própria ficha.**

A persona `JOGADOR IA EVENTUAL` pode ser compartilhada por vários personagens, mas cada um continua sendo uma peça própria com seu arquivo em `personagens/`.

### Ponto 7 — personagem conhecido com versões diferentes

APROVADO E REGISTRADO.

> **Personagens conhecidos usam a versão escolhida pelo jogador como base. O jogador pode modificar, combinar ou substituir elementos dessa versão durante a criação. A versão canônica serve como referência, não como limite.**

Depois de consolidada, a versão criada para a campanha passa a ser a referência canônica local daquela personagem.

### Ponto 8 — nome de campanha já existente

APROVADO E REGISTRADO.

> **A criação de uma nova campanha nunca pode sobrescrever automaticamente uma pasta de campanha existente.**

A verificação acontece antes da criação de qualquer arquivo.

### Ponto 9 — modelos determinísticos dos arquivos automáticos

APROVADO E REGISTRADO.

Regra aprovada:

> **Os arquivos operacionais da estrutura-base possuem textos iniciais obrigatórios e determinísticos. Toda nova campanha nasce com os mesmos modelos, sem improvisação entre IAs.**

Modelos definidos para:

```text
personagens/README.md
mundo/README.md
mestre/README.md
livro/README.md
estado/atual.md
```

Os textos exatos possuem uma única fonte canônica em:

- `sistema/criacao/estrutura-da-campanha.md`

O conteúdo desses arquivos pode ser atualizado depois conforme a campanha evolui; somente o modelo inicial é obrigatório e invariável.

Commit:

- `9c929d4b1461a01cc93ecec9ef414d14926f3c57`

## Ponto atual

### Ponto 10 — migrar a porta de entrada do repositório

O `README.md` da raiz e `sistema/00-LEIA-PRIMEIRO.md` ainda apontam para o fluxo legado:

- `sistema/protocolo-de-criacao.md`;
- `aventuras/`;
- estrutura antiga.

Proposta a discutir:

```text
NOVA CAMPANHA
→ sistema/criacao/README.md

CONTINUAR
→ campanhas/<nome>/README.md
```

A migração deve alinhar a entrada do sistema ao novo fluxo sem apagar nem migrar automaticamente campanhas antigas em `aventuras/`.

## Estrutura de campanha já aprovada

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

A estrutura nasce junto com o nome da campanha.

## Arquivos principais da revisão

```text
sistema/criacao/README.md
sistema/criacao/estrutura-da-campanha.md
sistema/criacao/PENDENCIAS.md
```

Antes de editar qualquer arquivo existente, buscar seu SHA atual.

## Ponto exato para retomar

Ao abrir um novo chat, continuar assim:

```text
1 - ler sistema/criacao/PENDENCIAS.md
2 - apresentar somente o Ponto 10 ao usuário
3 - não alterar a porta de entrada até o Ponto 10 ser aprovado
```
