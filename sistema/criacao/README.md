# Criação de Campanha

Status: APROVADO

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

Quando o nome estiver livre:

```text
criar campanhas/<nome>/
→ aplicar a estrutura obrigatória de estrutura-da-campanha.md
→ registrar CRIAÇÃO: EM ANDAMENTO no README.md
→ checkpoint: Direção narrativa e cenário
```

# Etapa — Direção narrativa e cenário

Construir primeiro o suficiente para saber **que tipo de campanha está sendo criada**.

A direção narrativa pode incluir, conforme relevante:

- gênero;
- tom;
- foco;
- ritmo;
- humor;
- romance/intimidade;
- atmosfera;
- outras prioridades de apresentação.

O cenário deve registrar somente o necessário para começar de forma coerente. Detalhes adicionais podem surgir durante a campanha e ser persistidos depois em `mundo/` quando se tornarem verdades estáveis.

Depois da aprovação:

```text
README.md
→ registrar resumo de Direção narrativa
→ registrar resumo de Cenário
→ checkpoint: Registrar protagonista
```

# Etapa — Registrar protagonista

A ficha nasce completa em **estrutura** e mínima em **conteúdo**.

As três perguntas universais de nascimento são:

```text
1 - NOME
2 - IMPORTÂNCIA
3 - CONTROLE
```

Para o protagonista, normalmente:

```text
CONTROLE: JOGADOR HUMANO
```

Depois de obter essas três informações:

```text
criar personagens/<nome>.md
→ copiar integralmente o modelo de ../personagem/ficha.md
→ Status: PENDENTE DE REVISÃO
→ preencher somente Nome, Importância e CONTROLE
→ deixar todo o restante em branco
```

Não preencher antes da revisão:

- conceito;
- aparência;
- idade;
- história;
- personalidade;
- atributos;
- perícias;
- poderes;
- traços;
- recursos;
- relações;
- outros campos não fornecidos e aprovados.

Depois:

```text
personagens/README.md
→ adicionar Nome + Importância + CONTROLE

README.md da campanha
→ checkpoint: Registrar outros personagens com agência
```

> **Antes da revisão, somente NOME, IMPORTÂNCIA e CONTROLE são preenchidos.**

# Etapa — Registrar outros personagens com agência

Perguntar quais outros personagens terão agência de jogador na campanha.

Para cada personagem:

```text
1 - NOME
2 - IMPORTÂNCIA
3 - CONTROLE
```

Valores de `CONTROLE` com agência própria:

```text
JOGADOR IA
JOGADOR IA EVENTUAL
```

Cada personagem recebe **seu próprio arquivo**.

Mesmo quando vários personagens usam a mesma persona `JOGADOR IA EVENTUAL`, não existe ficha compartilhada.

Quando o jogador terminar de registrar personagens:

```text
checkpoint
→ Revisão das fichas
```

## Personagens conhecidos

Se o personagem vier de obra conhecida, sua versão-base é tratada somente durante o **Bloco 1 — Identidade e conceito**, salvo quando o jogador já forneceu explicitamente essa informação antes.

Não preencher antecipadamente cânone, poderes, história ou personalidade só porque o nome é conhecido.

A versão escolhida e consolidada pelo jogador torna-se a referência canônica local da campanha.

# Etapa — Revisão das fichas

A revisão ocorre por personagem, em cinco blocos:

```text
1 - Identidade e conceito
2 - Atributos e perícias
3 - Poderes e capacidades
4 - Traços e relações
5 - Conferência final
```

Ordem geral:

```text
JOGADORES IA
→ JOGADORES IA EVENTUAIS
→ protagonista
```

Dentro de cada bloco:

```text
apresentar proposta
→ discutir
→ ajustar
→ receber aprovação
→ salvar imediatamente somente o bloco aprovado
→ avançar checkpoint
```

Conteúdo ainda em discussão **não é persistido como definitivo**.

Não preencher campo vazio com zero. `[0]` é valor mecânico real e só deve ser usado quando realmente estabelecido.

Depois do Bloco 5 aprovado:

```text
Status da ficha: APROVADO
```

Então seguir para a próxima ficha.

# Etapa — Início da história

Somente depois de todas as fichas aprovadas, definir a situação concreta em que a campanha começará.

O início pertence a:

```text
estado/atual.md
```

O README da campanha apenas aponta para essa fonte.

Consolidar em `estado/atual.md` o que for necessário para abrir corretamente a primeira cena, por exemplo:

- quem está presente;
- onde estão;
- situação imediata;
- STATUS relevante;
- efeitos ativos;
- fios causais já estabelecidos;
- informação operacional necessária.

Depois:

```text
README.md
→ CRIAÇÃO: CONCLUÍDA
→ remover checkpoint de criação
→ apontar Situação de entrada para estado/atual.md
```

Somente então começar a primeira cena.

# Importância e CONTROLE

`IMPORTÂNCIA` mede peso estrutural.

`CONTROLE` define quem decide.

São independentes.

Não existe limite universal obrigatório de personagens Centrais.

Mudar `IMPORTÂNCIA` não muda automaticamente `CONTROLE`, ficha ou mecânica.

Toda proposta de alteração de Importância exige aprovação do JOGADOR HUMANO antes de persistir.

# Regra contra duplicação

Cada informação deve possuir uma fonte principal.

```text
README da campanha
→ resumo e checkpoint

personagens/
→ fichas

estado/atual.md
→ presente operacional

mundo/
→ verdades estáveis do cenário

mestre/
→ material reservado e NPCs persistentes

livro/
→ história ocorrida
```

Não criar arquivos paralelos de STATUS, Progressão, cronologia, intenções ou gerência apenas para repetir conteúdo já coberto por essa estrutura.

## Regra final

> **A ficha nasce completa em estrutura e mínima em conteúdo. Antes da revisão, somente NOME, IMPORTÂNCIA e CONTROLE são preenchidos; os demais campos permanecem vazios até seu bloco. Cada bloco aprovado é salvo imediatamente. Depois de todas as fichas aprovadas, o estado inicial é consolidado e a campanha começa.**