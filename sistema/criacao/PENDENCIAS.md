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

Exemplo:

```text
CRIAÇÃO: EM ANDAMENTO

Etapa atual: Revisão mecânica e aprovação
Personagem atual: Ravena
Bloco atual: 3 - Poderes e capacidades
```

Quando a criação termina:

```text
CRIAÇÃO: CONCLUÍDA
```

O checkpoint não guarda conteúdo da etapa; apenas o ponto operacional de retomada.

Registrado em:

- `sistema/criacao/README.md`
- `sistema/criacao/estrutura-da-campanha.md`

Commits:

- `1f37238f6c940f4283088d0c49473f1acaf5ab68`
- `11962cd5843d80cf663f6f5a9bb22d53afc2c730`

### Ponto 2 — destino exato de cada etapa

APROVADO E REGISTRADO.

Formulação aprovada:

```text
NOME
→ README.md
→ cria toda a estrutura-base

DIREÇÃO NARRATIVA
→ README.md

CENÁRIO
→ resumo necessário no README.md
→ detalhes estáveis, quando necessários, em mundo/

PROTAGONISTA
→ personagens/<nome>.md
→ identificação + CONTROLE no README.md

PERSONAGENS IA / EVENTUAIS
→ personagens/<nome>.md
→ identificação + CONTROLE no README.md

INÍCIO DA HISTÓRIA
→ estado/atual.md
→ README.md apenas aponta que a retomada está em estado/atual.md

CHECKPOINT DA CRIAÇÃO
→ README.md
```

Regra central aprovada:

> **Cada informação possui uma fonte principal. O README resume e orienta; não duplica o conteúdo dos arquivos concretos.**

Registrado em:

- `sistema/criacao/README.md`
- `sistema/criacao/estrutura-da-campanha.md`

### Ponto 3 — salvamento durante a revisão mecânica

APROVADO E REGISTRADO.

Regra aprovada:

> **Durante a revisão mecânica, cada bloco passa a ser persistido imediatamente após sua aprovação. Conteúdo ainda em discussão não é salvo. Depois do salvamento, o checkpoint avança para o próximo bloco.**

Fluxo:

```text
bloco apresentado
→ discutir e corrigir
→ jogador aprova
→ atualizar personagens/<nome>.md
→ atualizar o checkpoint para o próximo bloco
```

Tentativas intermediárias, alternativas recusadas e valores ainda não aprovados não entram na ficha.

Se a conversa for interrompida, os blocos já aprovados permanecem preservados e o checkpoint indica exatamente onde retomar.

Registrado em:

- `sistema/criacao/README.md`

Commit:

- `977986583e4a8e8cb6324f240060123b231b13cc`

## Ponto atual

### Ponto 4 — hand-off para `estado/atual.md` antes da primeira cena

Proposta ainda não discutida em detalhe:

```text
fichas aprovadas
→ consolidar estado inicial em estado/atual.md
→ marcar CRIAÇÃO: CONCLUÍDA
→ NARRADOR abre a primeira cena
```

Isso deve ser persistência automática, não uma nova etapa nem nova confirmação do jogador.

## Pontos ainda não revisados

### Ponto 5 — relação entre GERÊNCIA e CONTROLE

Durante a criação de personagens IA é usado `GERÊNCIA`, enquanto a ficha definitiva usa `CONTROLE`.

Proposta a discutir:

> **GERÊNCIA é a escolha feita durante a criação; ao criar a ficha, seu valor é registrado no campo `CONTROLE`.**

Evitar criar um campo permanente `GERÊNCIA:` na ficha.

### Ponto 6 — personagens eventuais no índice da campanha

Evitar listar um grupo genérico como se fosse uma única peça quando existem personagens distintos.

Exemplo preferido a discutir:

```text
Dick Grayson — JOGADOR IA EVENTUAL
Kory — JOGADOR IA EVENTUAL
Garfield — JOGADOR IA EVENTUAL
```

A persona `JOGADOR IA EVENTUAL` pode ser única, mas as peças continuam distintas.

### Ponto 7 — personagem conhecido com versões diferentes

Para personagens licenciados ou conhecidos, uma IA pode escolher versões incompatíveis.

Proposta a discutir:

- se o cenário já determina a versão, usar essa versão;
- se existem versões materialmente diferentes e a campanha ainda não definiu qual vale, perguntar somente essa escolha antes de gerar a ficha preliminar.

### Ponto 8 — nome de campanha já existente

Como o nome agora cria a estrutura imediatamente, falta uma proteção contra sobrescrita.

Proposta a discutir:

```text
se campanhas/<nome>/ já existir
→ NÃO sobrescrever
→ informar que a campanha já existe
→ escolher outro nome ou usar CONTINUAR
```

### Ponto 9 — modelos determinísticos dos READMEs automáticos

Os READMEs internos já são obrigatórios, mas seu texto-base ainda pode variar entre IAs.

Proposta a discutir: definir modelos curtos e exatos para:

```text
personagens/README.md
mundo/README.md
mestre/README.md
livro/README.md
estado/atual.md
```

Objetivo: qualquer IA criar a mesma estrutura conceitual sem improvisação.

### Ponto 10 — migrar a porta de entrada do repositório

Somente depois de fechar o novo processo de criação.

O `README.md` da raiz e `sistema/00-LEIA-PRIMEIRO.md` ainda apontam para o fluxo legado:

- `sistema/protocolo-de-criacao.md`;
- `aventuras/`;
- estrutura antiga.

Depois que `sistema/criacao/` estiver fechado, alinhar a entrada para o novo fluxo baseado em:

```text
NOVA CAMPANHA → sistema/criacao/README.md
CONTINUAR     → campanhas/<nome>/README.md
```

Não apagar nem migrar automaticamente campanhas antigas em `aventuras/`.

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
2 - apresentar somente o Ponto 4 ao usuário
3 - não avançar ao Ponto 5 até o Ponto 4 ser aprovado e salvo
```
