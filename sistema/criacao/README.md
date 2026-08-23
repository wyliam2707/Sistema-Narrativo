# Criação de Campanha

Status: EM REVISÃO

Este arquivo é a porta de entrada para **criar uma nova campanha**.

Ele ensina outra IA ou narrador a conduzir a criação. Os dados concretos da campanha pertencem a `campanhas/<nome-da-campanha>/` conforme `estrutura-da-campanha.md`.

> **O sistema ensina como criar. A campanha guarda o que foi criado.**

## Princípios

Durante a criação:

- fazer uma pergunta por vez;
- não pedir novamente informação que o jogador já forneceu;
- interpretar respostas livres normalmente;
- perguntar somente o que ainda fizer diferença real;
- consolidar uma etapa antes de avançar;
- salvar somente conteúdo aprovado;
- não preencher campos de ficha antes do momento definido para sua revisão.

> **Primeiro identificamos as peças. Depois construímos suas fichas. Só então definimos a abertura da história.**

## Exemplos e respostas numéricas

Quando uma pergunta se beneficiar de exemplos, apresentá-los numerados, uma opção por linha.

O jogador pode escolher um número, combinar opções ou responder livremente.

> **Exemplos numerados são atalhos, nunca lista fechada.**

## Fluxo geral

A criação segue esta ordem:

```text
Nome da campanha
→ Direção narrativa e cenário
→ Registrar protagonista
→ Registrar outros personagens com agência
→ Revisão das fichas
→ Início da história
→ Consolidar estado inicial
→ CRIAÇÃO: CONCLUÍDA
→ primeira cena
```

## Checkpoint da criação

Enquanto a campanha estiver sendo criada, o `README.md` da própria campanha registra somente **onde retomar**.

Exemplo:

```text
CRIAÇÃO: EM ANDAMENTO

Etapa atual: Revisão das fichas
Personagem atual: Ravena
Bloco atual: 3 - Poderes e capacidades
```

Quando a criação terminar:

```text
CRIAÇÃO: CONCLUÍDA
```

O checkpoint não guarda o conteúdo da etapa.

> **O conteúdo fica nos arquivos próprios. O checkpoint diz somente de onde continuar.**

## Destino canônico de cada etapa

```text
NOME DA CAMPANHA
→ README.md
→ cria toda a estrutura-base

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
→ cada bloco aprovado é persistido na própria ficha

INÍCIO DA HISTÓRIA
→ estado/atual.md
→ README.md apenas aponta Situação de entrada para estado/atual.md

CHECKPOINT
→ README.md
```

> **Cada informação possui uma fonte principal. O README resume e orienta; não replica os arquivos concretos.**

# Etapa — Nome da campanha

Perguntar o nome da campanha.

Antes de criar qualquer arquivo, verificar se `campanhas/<nome-da-campanha>/` já existe.

Se já existir:

```text
NÃO sobrescrever
→ informar que a campanha já existe
→ oferecer continuar essa campanha ou escolher outro nome
```

A criação de uma nova campanha nunca substitui automaticamente uma campanha existente.

Se o nome estiver disponível, criar imediatamente a estrutura-base definida em `estrutura-da-campanha.md`.

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

> **NOME DISPONÍVEL → estrutura-base criada → criação continua.**

# Etapa — Direção narrativa e cenário

Esta etapa responde apenas ao necessário para sustentar a campanha.

```text
Direção narrativa → que experiência queremos produzir?
Cenário           → em que mundo e condições básicas isso acontece?
```

Podem importar, conforme o caso:

- gênero;
- tom;
- foco;
- ritmo;
- romance, humor, terror, investigação, ação, cotidiano ou outros elementos;
- universo;
- local principal;
- época;
- tecnologia;
- magia ou sobrenatural;
- organizações essenciais;
- regras especiais do mundo;
- grau de fidelidade ou adaptação em cenário conhecido.

Não construir uma enciclopédia antes de jogar.

Quando estiver suficientemente claro:

```text
consolidar Direção narrativa e Cenário no README.md
→ registrar em mundo/ somente detalhes estáveis que precisem de arquivo próprio
→ checkpoint: Registrar protagonista
```

# Regra universal — nascimento de qualquer ficha

A primeira estrutura de **qualquer personagem apresentável ao jogador** é sempre:

```text
1 - NOME
2 - IMPORTÂNCIA
3 - CONTROLE
```

Fazer uma pergunta por vez.

Se o jogador já tiver fornecido um desses campos de forma explícita, não perguntar novamente; registrar e seguir para o próximo ainda indefinido.

Assim que os três estiverem definidos:

```text
NOME + IMPORTÂNCIA + CONTROLE
→ criar personagens/<nome>.md
→ copiar o modelo-base completo de sistema/personagem/ficha.md
→ Status: PENDENTE DE REVISÃO
→ preencher somente Nome, Importância e CONTROLE
→ deixar todo o restante em branco
```

Não preencher antecipadamente conceito, aparência, idade, história, personalidade, atributos, perícias, poderes, TRAÇOS, RECURSOS, relações ou qualquer outro campo.

> **A ficha nasce completa em estrutura e mínima em conteúdo. Todo o restante pertence à revisão.**

# Etapa — Registrar protagonista

Registrar o personagem do jogador humano usando exatamente a regra universal:

```text
NOME
→ IMPORTÂNCIA
→ CONTROLE
→ ficha completa em branco
```

`CONTROLE` deve representar a autoridade realmente definida para essa peça; não inferir Importância a partir do Controle nem Controle a partir da Importância.

Depois de criar a ficha estrutural do protagonista:

```text
registrar Nome + Importância + CONTROLE no índice da campanha
→ checkpoint: Registrar outros personagens com agência
```

Nenhum outro conteúdo da ficha é criado nesta etapa.

# Etapa — Registrar outros personagens com agência

Perguntar se a campanha terá outros personagens com agência própria de jogador no início.

Quando houver, registrar **cada personagem individualmente** pela mesma sequência:

```text
NOME
→ IMPORTÂNCIA
→ CONTROLE
→ ficha completa em branco
```

Controles possíveis incluem, conforme a campanha:

```text
JOGADOR IA
JOGADOR IA EVENTUAL
```

Cada personagem possui seu próprio arquivo mesmo quando vários compartilham a persona `JOGADOR IA EVENTUAL`.

Não criar grupo, equipe ou organização como uma única ficha quando seus integrantes são peças distintas.

## Personagens conhecidos

Se o personagem for conhecido, canônico ou licenciado, **não desenvolver sua versão nesta etapa**.

Aqui continuam sendo preenchidos apenas:

```text
NOME
IMPORTÂNCIA
CONTROLE
```

A versão-base, combinações e alterações entram no Bloco 1 da revisão, salvo quando o jogador já tiver fornecido essa informação antes.

Quando todos os personagens com agência inicial estiverem registrados:

```text
checkpoint: Revisão das fichas
```

# Etapa — Revisão das fichas

A revisão acontece **uma ficha por vez**.

Ordem inicial:

```text
personagens JOGADOR IA
→ personagens JOGADOR IA EVENTUAL
→ protagonista
```

O protagonista é revisado por último para evitar que sua ficha sirva como régua automática para calibrar as demais.

Cada personagem é calibrado pelo que ele é, usando `sistema/personagem/` e `sistema/resolucao/` quando necessário.

## Cinco blocos

```text
1 - Identidade e conceito
2 - Atributos e perícias
3 - Poderes e capacidades
4 - Traços e relações
5 - Conferência final
```

### Bloco 1 — Identidade e conceito

Nome, Importância e CONTROLE já estão definidos.

Revisar e preencher o restante da identidade, quando aplicável:

- versão-base de personagem conhecido;
- origem;
- idade;
- aparência;
- conceito;
- personalidade;
- comportamento;
- história essencial;
- desejos e objetivos;
- medos e limites;
- conhecimento necessário para interpretação.

Para personagem conhecido, o jogador pode alterar, combinar ou substituir qualquer elemento da versão-base. Depois de consolidada, a versão da campanha passa a ser sua referência canônica local.

> **A pergunta relevante é “qual é a versão desta campanha?”, não “qual é a versão oficial?”.**

### Bloco 2 — Atributos e perícias

Converter e revisar:

```text
FIS | RES | MEN | VON
```

e as perícias realmente relevantes.

### Bloco 3 — Poderes e capacidades

Converter e revisar poderes, equipamentos tratados como Poder quando aplicável, capacidades especiais e seus limites.

### Bloco 4 — Traços e relações

Revisar TRAÇOS, fraquezas, características qualitativas, RECURSOS recorrentes e relações que pertençam à ficha.

### Bloco 5 — Conferência final

Verificar o conjunto completo, corrigir incoerências, remover excessos e confirmar que o modelo não deixou campo importante esquecido.

Campos comprovadamente inúteis podem ser removidos somente depois dessa conferência.

## Salvamento por bloco

Conteúdo ainda em discussão não é persistido como definitivo.

```text
bloco apresentado
→ discutir e corrigir
→ jogador aprova
→ atualizar personagens/<nome>.md
→ atualizar checkpoint para o próximo bloco
```

Se a conversa for interrompida, os blocos aprovados permanecem salvos e o checkpoint mostra o ponto exato de retomada.

Quando uma ficha concluir o Bloco 5:

```text
Status: APROVADO
```

Depois que todas as fichas iniciais estiverem aprovadas:

```text
checkpoint: Início da história
```

# Etapa — Início da história

Somente depois das fichas aprovadas definir **de onde a primeira cena parte**.

Pergunta-base:

> **Como você quer que a história comece?**

Exemplos podem incluir:

```text
1 - cotidiano antes de algo acontecer
2 - já no meio de um acontecimento
3 - encontro com personagem importante
4 - chegada a um novo lugar
5 - missão ou objetivo já em andamento
6 - problema ou ameaça aparece
7 - NARRADOR escolhe uma abertura coerente
8 - outro / combinação própria
```

A etapa possui no máximo 5 perguntas principais, mas esse é apenas um teto. Perguntar menos quando já houver informação suficiente.

Não planejar capítulos futuros, arcos completos ou acontecimentos que ainda devem nascer durante o jogo.

Quando a abertura estiver clara:

```text
consolidar resumo do início
→ registrar situação inicial concreta em estado/atual.md
→ README.md aponta Situação de entrada para estado/atual.md
→ CRIAÇÃO: CONCLUÍDA
→ NARRADOR abre a primeira cena
```

A consolidação usa somente fatos já aprovados e necessários para a entrada. Não copia fichas completas para `estado/atual.md` e não inventa acontecimentos futuros.

> **Fichas aprovadas primeiro. Abertura depois. A primeira cena nasce do estado já consolidado.**
