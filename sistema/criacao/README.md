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

```text
Nome da campanha
→ Direção narrativa e cenário
→ Registrar protagonista humano
→ Registrar TODOS os demais personagens iniciais com agência
→ Confirmar elenco inicial com agência
→ Revisão das fichas
→ Pareamento das informações
→ Início da história
→ Consolidar estado inicial
→ CRIAÇÃO: CONCLUÍDA
→ primeira cena
```

Nenhuma ficha entra em revisão enquanto ainda houver personagem inicial com agência a registrar.

A situação inicial não é definida enquanto o pareamento das fichas relevantes ainda possuir lacunas cruzadas a resolver.

---

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

> **O conteúdo fica nos arquivos próprios. O checkpoint diz somente de onde continuar.**

---

## Destino canônico de cada etapa

```text
NOME DA CAMPANHA
→ README.md

DIREÇÃO NARRATIVA / CENÁRIO
→ resumo necessário em README.md
→ verdades estáveis adicionais em mundo/

PERSONAGEM COM AGÊNCIA
→ personagens/<nome>.md
→ Nome + Importância + CONTROLE no índice

REVISÃO DA FICHA
→ personagens/<nome>.md
→ cada bloco aprovado é persistido

PAREAMENTO
→ compara fichas relacionadas
→ pergunta uma questão por vez
→ consolida em lote as respostas aprovadas

INÍCIO DA HISTÓRIA
→ estado/atual.md

CHECKPOINT
→ README.md
```

> **Cada informação possui uma fonte principal. O README resume e orienta; não replica os arquivos concretos.**

---

# Etapa — Nome da campanha

Perguntar o nome da campanha.

Antes de criar qualquer arquivo, verificar se `campanhas/<nome-da-campanha>/` já existe.

Se já existir:

```text
NÃO sobrescrever
→ informar que a campanha já existe
→ oferecer continuar essa campanha ou escolher outro nome
```

Quando o nome estiver livre:

```text
garantir campanhas/README.md
→ criar campanhas/<nome>/
→ aplicar estrutura-da-campanha.md
→ registrar CRIAÇÃO: EM ANDAMENTO
→ checkpoint: Direção narrativa e cenário
```

---

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

---

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

- Patamar;
- Conceito;
- aparência;
- idade;
- história;
- personalidade;
- Atributos;
- Perícias;
- Poderes;
- Traços;
- Vida/Mana derivadas;
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

---

# Etapa — Registrar outros personagens com agência

Depois do protagonista humano, identificar e registrar **todos os demais personagens iniciais com agência** antes de revisar qualquer ficha.

Para cada personagem:

```text
1 - NOME
2 - IMPORTÂNCIA
3 - CONTROLE
```

Valores disponíveis nesta etapa:

```text
JOGADOR IA
JOGADOR IA EVENTUAL
```

`JOGADOR HUMANO` não é oferecido novamente.

Cada personagem recebe seu próprio arquivo, mesmo quando vários usam a mesma persona `JOGADOR IA EVENTUAL`.

Continuar até o jogador humano declarar que o elenco inicial com agência está completo.

Somente então:

```text
checkpoint
→ Revisão das fichas
```

---

# Etapa — Revisão das fichas

A revisão só começa depois da confirmação de que todas as peças iniciais com agência já foram registradas.

A revisão ocorre por personagem, em cinco blocos:

```text
1 - Identidade e Conceito
2 - Patamar, Atributos e Perícias
3 - Poderes e capacidades
4 - Traços, Recursos e relações
5 - Conferência final
```

As regras detalhadas pertencem a `../personagem/criacao.md`.

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

Conteúdo ainda em discussão não é persistido como definitivo.

Não preencher campo vazio com zero. `[0]` é valor mecânico real.

Depois do Bloco 5 aprovado:

```text
Status da ficha: APROVADO
```

Depois que todas as fichas iniciais estiverem aprovadas:

```text
checkpoint
→ Pareamento das informações
```

Não definir ainda a situação de entrada.

---

# Etapa — Pareamento das informações

Depois que todas as fichas individuais estiverem `APROVADO`, comparar as fichas que possuem vínculos narrativamente relevantes.

A regra detalhada pertence a:

```text
../personagem/pareamento.md
```

O pareamento pode procurar, por exemplo:

- há quanto tempo duas pessoas se conhecem;
- como se conheceram;
- o que uma sabe sobre a outra;
- segredos e assimetrias de conhecimento;
- fatos recorrentes compartilhados;
- acesso, confiança, obrigações e rotinas;
- conhecimento sobre terceiros adquirido através da relação.

Quando houver lacunas relevantes:

```text
identificar perguntas necessárias
→ fazer UMA pergunta ao JOGADOR HUMANO
→ guardar a resposta
→ fazer a próxima pergunta
→ repetir até esclarecer o conjunto
→ consolidar consequências
→ ajustar em lote todas as fichas afetadas
→ persistir
```

As fichas continuam `APROVADO`; não é necessário reiniciar os cinco blocos.

Depois de concluir o pareamento:

```text
checkpoint
→ Início da história
```

---

# Etapa — Início da história

Somente depois de todas as fichas aprovadas e do pareamento concluído, definir a situação concreta em que a campanha começará.

O início pertence a:

```text
estado/atual.md
```

Consolidar o necessário para abrir corretamente a primeira cena:

- quem está presente;
- onde estão;
- situação imediata;
- STATUS relevante;
- fios causais já estabelecidos;
- informação operacional necessária.

### Estado mecânico inicial

Quando uma personagem começar sem desgaste ou efeito previamente estabelecido:

```text
Vida atual
→ Vida Máxima

Mana atual
→ Mana Máxima
```

Para a única personagem com:

```text
CONTROLE: JOGADOR HUMANO
```

inicializar também:

```text
Trama [30]
```

conforme `../personagem/trama.md`.

Não criar Trama para JOGADOR IA, JOGADOR IA EVENTUAL ou NPC por regra geral.

Se a abertura da campanha já estabelecer ferimento, gasto, Status ou outra condição, registrar o valor realmente aprovado em vez de restaurar automaticamente.

Depois:

```text
README.md
→ CRIAÇÃO: CONCLUÍDA
→ remover checkpoint
→ apontar Situação de entrada para estado/atual.md
```

Somente então começar a primeira cena.

---

# Importância e CONTROLE

`IMPORTÂNCIA` mede peso estrutural.

`CONTROLE` define quem decide.

São independentes.

Não existe limite universal obrigatório de personagens Centrais.

Existe apenas **uma peça com `CONTROLE: JOGADOR HUMANO` por campanha**.

Mudar `IMPORTÂNCIA` não muda automaticamente `CONTROLE`, ficha ou mecânica.

Toda proposta de alteração de Importância exige aprovação do JOGADOR HUMANO antes de persistir.

---

# Regra contra duplicação

Cada informação deve possuir uma fonte principal.

```text
README da campanha
→ resumo e checkpoint

personagens/
→ fichas consolidadas

estado/atual.md
→ presente operacional, incluindo reservas atuais

mundo/
→ verdades estáveis do cenário

mestre/
→ material reservado e NPCs persistentes

livro/
→ história ocorrida
```

Não criar arquivos paralelos de STATUS, Progressão, cronologia, intenções ou gerência apenas para repetir conteúdo já coberto por essa estrutura.

## Regra final

> **A ficha nasce completa em estrutura e mínima em conteúdo. Antes da revisão, somente NOME, IMPORTÂNCIA e CONTROLE são preenchidos. A revisão inclui Patamar, seis Atributos, Perícias, Poderes e Traços; depois do pareamento, o estado inicial recebe Vida/Mana atuais e Trama 30 para o protagonista humano. Só então a campanha começa.**
