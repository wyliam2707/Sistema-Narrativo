# Criação de Campanha

Status: REFORMULAÇÃO / NÃO IMPLEMENTADO

Este arquivo define como uma nova campanha nasce usando `regras-basicas/`.

> **Cada passo usa o anterior como base: primeiro definir a narrativa, depois criar e fechar estruturalmente a temporada, depois construir fichas persistentes para essa campanha.**

## Fluxo geral

Ao receber `Nova campanha`:

```text
PASSO 01 — CAMPANHA
→ definir a identidade narrativa persistente.

PASSO 02 — TEMPORADA
→ receber a direção do Jogador.
→ criar o problema da temporada.
→ listar o que precisa ser resolvido.
→ responder previamente as questões estruturais.
→ registrar a Diretriz Fechada.

PASSO 03 — FICHAS
→ identificar o elenco inicial.
→ construir as personagens através da lente da campanha.
→ usar a primeira temporada apenas como contexto inicial.

DEPOIS
→ pareamento mínimo
→ situação inicial
→ Mesa operacional
→ START
```

Não pedir novamente informação já fornecida.

## 1 — Nome e estrutura

Depois que o nome for aprovado, materializar:

```text
campanhas/<nome>/
├── README.md
├── personagens/
│   └── README.md
├── estado/
│   └── atual.md
├── mundo/
│   └── README.md
├── mestre/
│   ├── README.md
│   ├── narrativa.md
│   ├── roteiro.md
│   └── temporadas/
│       └── README.md
├── opositor/
│   └── README.md
└── livro/
    └── README.md
```

Os `README.md` internos apenas identificam a função de cada área e mantêm a organização visível no repositório.

O `README.md` da campanha começa com:

```text
CRIAÇÃO: EM ANDAMENTO
Etapa atual: PASSO 01 — CAMPANHA
```

## PASSO 01 — Narrativa da campanha

O primeiro passo não cria ainda o arco da aventura. Ele define **que tipo de história esta campanha quer ser ao longo das temporadas**.

Perguntar somente o necessário:

```text
Qual é o foco principal?
Qual é o gênero?
Qual é o tom?
Que tipo de experiência queremos acompanhar?
Que temas ou relações devem receber mais espaço?
Que tipos de conflito combinam com a campanha?
O que não deve dominar a história?
Que premissas gerais já são válidas neste mundo ou nesta proposta?
```

As respostas podem ser curtas.

Exemplo:

```text
FOCO
→ romance e convivência.

GÊNERO
→ romance, comédia e aventura.

TOM
→ adulto, leve e divertido, com perigo ocasional.

EXPERIÊNCIA
→ acompanhar aproximação, vínculos e vida compartilhada.

NÃO DOMINAR
→ conspiração mundial, tragédia constante ou investigação pesada.
```

Registrar em:

```text
campanhas/<nome>/mestre/narrativa.md
```

Estrutura mínima:

```text
# Narrativa da Campanha

## Foco principal
→ sobre o que a campanha é.

## Gênero e tom
→ como essa história normalmente se apresenta.

## Experiência desejada
→ o que deve receber desenvolvimento e continuidade.

## Temas e conflitos recorrentes
→ que tipos de situação combinam com a proposta.

## Não dominar
→ o que pode existir, mas não deve tomar automaticamente o centro.

## Premissas gerais
→ elementos considerados normais ou válidos nesta campanha.
```

Preencher somente os blocos úteis.

A narrativa da campanha é **persistente entre temporadas**.

```text
NARRATIVA
→ identidade da campanha.

TEMPORADA
→ arco atual.
```

Alterar a narrativa depois exige uma mudança deliberada de proposta. Uma miniquest, um vilão interessante ou uma temporada diferente não reescrevem automaticamente o foco da campanha.

## PASSO 02 — Criar a temporada

Depois que a narrativa estiver aprovada, seguir:

```text
CRIACAO-DE-TEMPORADA.md
```

A temporada usa `mestre/narrativa.md` como base e transforma a direção do Jogador em um arco preparado antes do jogo.

O fluxo obrigatório é:

```text
DIREÇÃO DO JOGADOR
↓
PROBLEMA DA TEMPORADA
↓
LISTA DO QUE PRECISA SER RESOLVIDO
↓
RESPOSTAS CANÔNICAS
↓
DIRETRIZ FECHADA
```

O roteiro ativo fica em:

```text
campanhas/<nome>/mestre/roteiro.md
```

Ele deve possuir direção suficiente, uma **condição de encerramento** e a **Diretriz Fechada** necessária para impedir que o Narrador invente continuamente a estrutura da temporada durante a sessão.

```text
CAMPANHA
→ diz sobre o que a história é.

JOGADOR
→ indica o que deseja explorar agora.

TEMPORADA
→ cria um problema concreto e estabelece previamente seu espaço estrutural.
```

O roteiro não determina cenas futuras nem resultados voluntários das personagens. Entretanto, problemas estruturais que exigem solução devem possuir respostas canônicas e pelo menos uma resolução possível antes do START.

Quando a temporada termina, ele é arquivado, o Narrador escreve o epílogo, consolida as mudanças e pergunta **“E agora?”** antes de criar a próxima temporada.

## PASSO 03 — Criar as fichas

Somente depois de existir:

```text
mestre/narrativa.md
+
mestre/roteiro.md
```

começar a construção das personagens.

A **Narrativa da Campanha** é a lente principal da ficha. O roteiro da primeira temporada ajuda a revelar necessidades imediatas, mas não limita a personagem à situação daquele arco.

```text
CAMPANHA
→ define quais aspectos da personagem tendem a importar ao longo da história.

PRIMEIRA TEMPORADA
→ ajuda a perceber o que já precisa estar claro no começo.

FICHA
→ permanece válida além da temporada atual.
```

### 3.1 — Elenco inicial

Primeiro identificar todas as personagens iniciais que já precisam possuir agência.

Para cada uma, basta começar com:

```text
Nome
Importância
CONTROLE
Conceito, quando já conhecido
ESTADO DA FICHA: EM CRIAÇÃO
```

Confirmar o elenco inicial antes da revisão detalhada das fichas.

Isso não exige conhecer toda a personagem antes da temporada. O elenco pode existir inicialmente apenas como conceito suficiente para saber **quem precisa ser construído**.

### 3.2 — Construção das fichas

Depois do elenco, criar ou revisar cada ficha conforme:

```text
jogador/1.3-criacao-da-ficha.md
```

Os últimos blocos da ficha são guiados principalmente pelo **tipo de história e de decisões que provavelmente importarão ao longo da campanha**.

```text
ROMANCE
→ vínculos, atração, compromisso, iniciativa, ciúme, modelos de relação, limites.

TERROR
→ medo, confiança, reação sob pressão, sinais de ameaça, proteção, perdas.

INVESTIGAÇÃO
→ conhecimento, suspeitas, métodos, padrões, contatos, fatos confirmados.

AÇÃO
→ risco, proteção, iniciativa, liderança, recuo, prioridades em perigo.
```

A mesma informação pode ser central numa campanha e quase irrelevante em outra.

> **A ficha não tenta responder tudo sobre a personagem. Ela preserva principalmente o que a IA precisará para interpretá-la com coerência nesta campanha.**

## 4 — Pareamento mínimo

Comparar apenas personagens cujas fichas possuam informações cruzadas relevantes.

Verificar somente o necessário para evitar contradições antes da primeira cena, como:

```text
se já se conhecem
natureza atual da relação
fatos compartilhados importantes
conhecimento que uma possui sobre a outra
obrigações, acessos ou vínculos recorrentes
```

Se houver lacuna importante, perguntar uma coisa por vez e atualizar somente as fichas afetadas.

```text
pode surgir normalmente em cena sem contradição
→ deixar para a história
```

Pareamento busca coerência, não biografia completa nem simetria.

## 5 — Situação inicial

Depois das fichas e do pareamento, registrar em:

```text
campanhas/<nome>/estado/atual.md
```

somente o presente necessário para abrir a primeira cena.

Quando relevante:

```text
local
momento ou período
personagens presentes
situação imediata
Vida / Mente / Mana atuais
condições ou efeitos ativos
processos ou prazos já em andamento
```

Estado Atual não é histórico.

## 6 — Mesa operacional

Registrar no `README.md` da campanha quem ocupa cada cadeira necessária.

Exemplo:

```text
## Mesa operacional

JOGADOR HUMANO → <personagem>
JOGADOR IA — <personagem> → <personagem>
JOGADOR IA EVENTUAL → ATIVO, quando necessário
OPOSITOR → ATIVO
NARRADOR → ATIVO
```

Cada personagem com `CONTROLE: JOGADOR IA` possui sua própria cadeira dedicada.

Uma única IA técnica pode executar várias cadeiras conforme `nucleo/1.6-execucao-por-uma-unica-ia.md`, mantendo conhecimento, objetivo e autoridade separados.

## 7 — START

Antes da primeira cena, conferir apenas se a campanha consegue funcionar corretamente:

```text
estrutura existe?
narrativa da campanha foi aprovada?
direção do Jogador para a temporada está clara?
problema da temporada foi criado?
lista do que precisa ser resolvido existe?
respostas canônicas necessárias foram definidas?
resoluções possíveis existem onde forem necessárias?
riscos, obstáculos e processos necessários possuem fundamento prévio?
Diretriz Fechada está registrada no roteiro?
condição de encerramento da temporada existe?
elenco inicial foi confirmado?
fichas necessárias estão aprovadas?
pareamento essencial foi resolvido?
estado inicial está definido?
CONTROLE das peças está claro?
Mesa operacional está registrada?
```

Se algo essencial estiver faltando:

```text
CRIAÇÃO: EM ANDAMENTO
→ registrar a etapa atual
→ não iniciar ficção
```

Se estiver pronto:

```text
CRIAÇÃO: CONCLUÍDA
→ seguir INICIO-E-RETOMADA.md
→ abrir a primeira cena
```

START é apenas a passagem da criação para o jogo. Não é uma cena nem um acontecimento ficcional.

## Ciclo depois da primeira temporada

Os três passos completos são necessários para **criar a campanha pela primeira vez**.

Depois disso, a campanha e as fichas continuam existindo.

Quando uma temporada termina:

```text
RESOLUÇÃO DA TEMPORADA
→ Epílogo
→ consolidar mudanças
→ “E agora?”
→ voltar ao PASSO 02 — TEMPORADA
```

Não voltar automaticamente ao Passo 01 e não repetir o Passo 03 como rotina.

```text
CAMPANHA
→ persistente.

FICHAS
→ persistentes.

TEMPORADA
→ renovável.
```

Uma nova temporada pode tornar uma informação antes secundária muito importante. Nesse caso, complementar uma ficha somente quando a ausência dessa informação tiver **alta chance de causar interpretação ou decisão incoerente** no novo arco.

```text
NOVA TEMPORADA
≠ revisar todas as fichas.

LACUNA REALMENTE CRÍTICA
→ complementar apenas o necessário.
```

## Função das áreas da campanha

```text
README
→ porta de entrada, checkpoint e Mesa operacional.

PERSONAGENS
→ fichas reais.

ESTADO
→ presente necessário para continuar.

MUNDO
→ verdades estáveis do cenário.

MESTRE / narrativa.md
→ identidade persistente da campanha.

MESTRE / roteiro.md
→ temporada ativa e sua Diretriz Fechada.

MESTRE / temporadas/
→ roteiros de temporadas já encerradas.

OPOSITOR
→ planos, processos e informações adversariais.

LIVRO
→ histórico consolidado, capítulos e epílogos.
```

As regras completas de onde salvar cada verdade pertencem a `registro/`.

## Criação emergente depois do START

Não é necessário prever todos os detalhes antes da primeira cena.

Lacunas menores podem ser completadas conforme `nucleo/1.7-criacao-emergente.md`, desde que não sejam inventadas retroativamente para favorecer ou impedir uma ação já apresentada.

A criação emergente não pode alterar a Diretriz Fechada, introduzir um novo problema estrutural ou ampliar a temporada além dos limites preparados apenas porque o Jogador demonstrou interesse em um elemento.

```text
IMPROVISAR DETALHES, CAMINHOS E CENAS
→ permitido.

IMPROVISAR UMA NOVA VERDADE ESTRUTURAL DA TEMPORADA
→ não permitido por padrão.
```

Uma trama secundária pode receber desenvolvimento dentro dos limites preparados, mas não substitui automaticamente a narrativa da campanha nem o arco atual da temporada.

## Regra final

> **Nova campanha segue três passos dependentes: a Narrativa define que história queremos jogar; na primeira Temporada o Jogador fornece a direção e o Narrador cria o problema, lista o que precisa ser resolvido, responde previamente as questões estruturais e registra uma Diretriz Fechada; as Fichas são então construídas através da lente da campanha, usando a primeira temporada como contexto inicial. Depois do START, a IA improvisa dentro do tabuleiro preparado, não a verdade estrutural da temporada. Cada temporada termina com resolução, epílogo, consolidação e “E agora?”, e o ciclo retorna ao Passo 02.**