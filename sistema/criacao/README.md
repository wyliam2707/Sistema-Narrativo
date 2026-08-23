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

> **Primeiro identificamos todas as peças iniciais. Depois construímos suas fichas. Em seguida pareamos as informações entre personagens relacionados. Só então definimos a abertura da história.**

## Exemplos e respostas numéricas

Quando uma pergunta se beneficiar de exemplos, apresentá-los numerados, uma opção por linha.

O jogador pode escolher um número, combinar opções ou responder livremente.

> **Exemplos numerados são atalhos, nunca lista fechada.**

## Fluxo geral

A criação segue esta ordem:

```text
Nome da campanha
→ Direção narrativa e cenário
→ Registrar protagonista humano
→ Registrar TODOS os demais personagens iniciais com agência
→ Confirmar que o elenco inicial com agência está completo
→ Revisão das fichas
→ Pareamento das informações entre fichas
→ Início da história
→ Consolidar estado inicial
→ CRIAÇÃO: CONCLUÍDA
→ primeira cena
```

Nenhuma ficha entra em revisão enquanto ainda houver personagem inicial com agência a registrar.

A situação inicial não é definida enquanto o pareamento das fichas relevantes ainda possuir lacunas cruzadas a resolver.

## Checkpoint da criação

Enquanto a campanha estiver sendo criada, o `README.md` da própria campanha registra somente **onde retomar**.

Exemplo durante revisão:

```text
CRIAÇÃO: EM ANDAMENTO

Etapa atual: Revisão das fichas
Personagem atual: Ravena
Bloco atual: 3 - Poderes e capacidades
```

Exemplo durante pareamento:

```text
CRIAÇÃO: EM ANDAMENTO

Etapa atual: Pareamento das informações
Par atual: Nick Fury ↔ Corvin Blackwood
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

PAREAMENTO DAS INFORMAÇÕES
→ compara fichas relacionadas
→ pergunta ao JOGADOR HUMANO quando houver lacuna relevante
→ ajusta imediatamente as fichas afetadas

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
garantir campanhas/README.md
→ criar campanhas/<nome>/
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

O protagonista humano usa:

```text
CONTROLE: JOGADOR HUMANO
```

Cada campanha possui **um único personagem com `CONTROLE: JOGADOR HUMANO`**.

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

Depois do protagonista humano, identificar e registrar **todos os demais personagens iniciais com agência** antes de revisar qualquer ficha.

Para cada personagem:

```text
1 - NOME
2 - IMPORTÂNCIA
3 - CONTROLE
```

Valores de `CONTROLE` com agência própria disponíveis nesta etapa:

```text
JOGADOR IA
JOGADOR IA EVENTUAL
```

`JOGADOR HUMANO` não é oferecido novamente: a única peça humana já foi definida no protagonista.

Cada personagem recebe **seu próprio arquivo**.

Mesmo quando vários personagens usam a mesma persona `JOGADOR IA EVENTUAL`, não existe ficha compartilhada.

O narrador deve continuar perguntando e registrando personagens até o jogador humano declarar que o **elenco inicial com agência está completo**.

Somente então:

```text
checkpoint
→ Revisão das fichas
```

> **Primeiro todos os personagens iniciais com agência. Depois qualquer revisão de ficha.**

NPCs comuns que surgirão durante o jogo não precisam ser antecipados nesta etapa. Personagens que já forem definidos como peças iniciais com agência, porém, devem ser registrados antes da revisão.

## Personagens conhecidos

Se o personagem vier de obra conhecida, sua versão-base é tratada somente durante o **Bloco 1 — Identidade e conceito**, salvo quando o jogador já forneceu explicitamente essa informação antes.

Não preencher antecipadamente cânone, poderes, história ou personalidade só porque o nome é conhecido.

A versão escolhida e consolidada pelo jogador torna-se a referência canônica local da campanha.

# Etapa — Revisão das fichas

A revisão só começa depois da confirmação de que todos os personagens iniciais com agência já foram registrados.

A revisão ocorre por personagem, em cinco blocos:

```text
1 - Identidade e conceito
2 - Atributos e perícias
3 - Poderes e capacidades
4 - Traços e relações
5 - Conferência final
```

O **Bloco 1 — Identidade e conceito** não deve terminar com uma descrição apenas abstrata. Antes de avançar, a personagem precisa estar suficientemente definida para ser **reconhecida e descrita em cena**.

Quando aplicável, isso inclui:

- nome de uso ou codinome;
- nome real/civil quando diferente;
- idade;
- aparência física;
- estilo visual e apresentação habitual;
- origem, natureza e conceito essenciais.

Personagens conhecidos não podem depender apenas do conhecimento externo do leitor. A versão desta campanha deve registrar concretamente os sinais de identidade necessários à interpretação. Detalhes e organização dessa revisão pertencem a `../personagem/criacao.md`.

Ordem geral:

```text
JOGADORES IA
→ JOGADORES IA EVENTUAIS
→ protagonista humano
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

Depois que **todas** as fichas iniciais estiverem aprovadas:

```text
checkpoint
→ Pareamento das informações
```

Não definir ainda a situação de entrada.

# Etapa — Pareamento das informações

Depois que todas as fichas individuais estiverem `APROVADO`, comparar as fichas que possuem vínculos narrativamente relevantes.

A regra detalhada pertence a:

```text
../personagem/pareamento.md
```

O pareamento procura fatos que a revisão individual pode não ter definido, por exemplo:

- há quanto tempo duas pessoas se conhecem;
- como se conheceram;
- o que uma sabe sobre a outra;
- segredos e assimetrias de conhecimento;
- fatos recorrentes compartilhados;
- acesso, confiança, obrigações e rotinas;
- conhecimento sobre terceiros adquirido através da relação.

Quando a comparação revelar uma lacuna relevante:

```text
fazer UMA pergunta ao JOGADOR HUMANO
→ receber resposta
→ consolidar a consequência
→ ajustar imediatamente todas as fichas afetadas
→ persistir
→ fazer a próxima pergunta necessária
```

As fichas continuam `APROVADO`; não é necessário reiniciar os cinco blocos.

O pareamento não cria arquivo paralelo de campanha apenas para repetir essas informações. As respostas são gravadas diretamente nas fichas ou, quando estabelecerem uma verdade geral do cenário, no destino canônico apropriado.

Depois de verificar todos os pares e grupos relevantes e confirmar que não restam lacunas cruzadas importantes:

```text
checkpoint
→ Início da história
```

> **A comparação revela perguntas. O JOGADOR HUMANO fornece as respostas. As respostas ajustam as fichas antes da primeira cena.**

# Etapa — Início da história

Somente depois de todas as fichas aprovadas **e do pareamento concluído**, definir a situação concreta em que a campanha começará.

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

Existe, porém, apenas **uma peça com `CONTROLE: JOGADOR HUMANO` por campanha**.

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

> **A ficha nasce completa em estrutura e mínima em conteúdo. Antes da revisão, somente NOME, IMPORTÂNCIA e CONTROLE são preenchidos; os demais campos permanecem vazios até seu bloco. Todos os personagens iniciais com agência são registrados antes de qualquer revisão. Cada bloco aprovado é salvo imediatamente. Depois que todas as fichas estiverem aprovadas, elas são pareadas por relações relevantes; o narrador faz uma pergunta por vez e ajusta as fichas conforme as respostas. Só depois do pareamento concluído o estado inicial é consolidado e a campanha começa.**
