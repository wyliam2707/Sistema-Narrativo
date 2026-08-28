# Criação de Campanha

Status: REFORMULAÇÃO / NÃO IMPLEMENTADO

Este arquivo define como uma nova campanha nasce usando `regras-basicas/`.

> **Cada passo usa o anterior como base: primeiro definir a narrativa, depois criar a temporada, depois construir as fichas para aquela história.**

## Fluxo geral

Ao receber `Nova campanha`:

```text
PASSO 01 — CAMPANHA
→ definir a identidade narrativa persistente.

PASSO 02 — TEMPORADA
→ criar o arco atual a partir dessa identidade.

PASSO 03 — FICHAS
→ construir as personagens usando campanha + temporada como contexto.

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

A temporada usa `mestre/narrativa.md` como base e cria o arco que será jogado agora.

O roteiro ativo fica em:

```text
campanhas/<nome>/mestre/roteiro.md
```

Ele deve definir somente o necessário para o arco atual, incluindo uma **condição de encerramento**.

```text
CAMPANHA
→ diz sobre o que a história é.

TEMPORADA
→ cria uma situação concreta para explorar isso agora.
```

O roteiro não determina cenas futuras nem resultados.

Quando a temporada termina, ele é arquivado, o Narrador escreve o epílogo, consolida as mudanças e pergunta **“E agora?”** antes de criar a próxima temporada.

## PASSO 03 — Criar as fichas

Somente depois de existir:

```text
mestre/narrativa.md
+
mestre/roteiro.md
```

criar ou revisar as fichas iniciais conforme:

```text
jogador/1.3-criacao-da-ficha.md
```

Isso permite que os últimos blocos da ficha sejam construídos de acordo com **o tipo de história e de decisões que realmente importam nesta campanha**.

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

> **A ficha não tenta responder tudo sobre a personagem. Ela preserva principalmente o que a IA precisará para interpretá-la com coerência nesta história.**

## 4 — Elenco inicial

Antes de revisar fichas completas, registrar todas as personagens iniciais que já precisam possuir agência.

Para cada uma, basta começar com:

```text
Nome
Importância
CONTROLE
Conceito, quando já conhecido
ESTADO DA FICHA: EM CRIAÇÃO
```

Confirmar o elenco inicial antes de avançar para a revisão detalhada.

Isso evita terminar uma ficha sem ainda saber quais outras peças centrais precisam coexistir com ela.

## 5 — Pareamento mínimo

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

## 6 — Situação inicial

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

## 7 — Mesa operacional

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

## 8 — START

Antes da primeira cena, conferir apenas se a campanha consegue funcionar corretamente:

```text
estrutura existe?
narrativa da campanha foi aprovada?
roteiro da temporada existe e possui direção suficiente?
condição de encerramento da temporada existe quando necessária?
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
→ temporada ativa.

MESTRE / temporadas/
→ roteiros de temporadas já encerradas.

OPOSITOR
→ planos, processos e informações adversariais.

LIVRO
→ histórico consolidado, capítulos e epílogos.
```

As regras completas de onde salvar cada verdade pertencem a `registro/`.

## Criação emergente depois do START

Não é necessário prever tudo antes da primeira cena.

Lacunas futuras podem ser completadas conforme `nucleo/1.7-criacao-emergente.md`, desde que não sejam inventadas retroativamente para favorecer ou impedir uma ação já apresentada.

Uma trama secundária pode crescer organicamente, mas não substitui automaticamente a narrativa da campanha nem o arco atual da temporada.

## Regra final

> **Nova campanha segue três passos dependentes: a Narrativa define que história queremos jogar; a Temporada transforma essa identidade em um arco atual com começo e fim; as Fichas usam as duas como base para registrar aquilo que realmente ajudará as personagens a decidir com coerência. Depois vêm pareamento, Estado, Mesa e START. Cada temporada termina com epílogo, consolidação e a pergunta “E agora?” antes de qualquer novo roteiro.**