# Criação de Campanha

Status: REFORMULAÇÃO / NÃO IMPLEMENTADO

Este arquivo define como uma nova campanha nasce usando `regras-basicas/`.

> **A organização nasce completa. A criação avança por etapas curtas, salva somente o aprovado e só começa a ficção quando já existe uma mesa jogável.**

## Fluxo geral

Ao receber `Nova campanha`:

```text
1. nome da campanha
2. materializar a estrutura
3. direção narrativa e cenário suficiente
4. registrar o elenco inicial
5. criar e aprovar as fichas
6. parear somente informações cruzadas essenciais
7. definir a situação inicial
8. registrar a Mesa operacional
9. conferir START
10. primeira cena
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
│   └── README.md
├── opositor/
│   └── README.md
└── livro/
    └── README.md
```

Os `README.md` internos apenas identificam a função de cada área e mantêm a organização visível no repositório.

O `README.md` da campanha começa com:

```text
CRIAÇÃO: EM ANDAMENTO
Etapa atual: ...
```

## 2 — Direção narrativa e cenário

Definir apenas o suficiente para saber que campanha está sendo criada e como ela deve ser apresentada.

Quando relevante:

```text
gênero
tom
foco
ritmo
humor
romance ou vínculos
atmosfera
premissa e cenário inicial
```

Não preencher o mundo inteiro antes de jogar.

## 3 — Elenco inicial

Antes de revisar fichas completas, registrar todas as personagens iniciais que já precisam possuir agência.

Para cada uma, basta começar com:

```text
Nome
Importância
CONTROLE
Conceito, quando já conhecido
ESTADO DA FICHA: EM CRIAÇÃO
```

Confirmar o elenco inicial antes de avançar para a revisão detalhada das fichas.

Isso evita terminar uma ficha sem ainda saber quais outras peças centrais precisam coexistir com ela.

## 4 — Criação das fichas

Criar cada ficha conforme:

```text
jogador/1.3-criacao-da-ficha.md
```

O padrão é:

```text
IA propõe quando houver base suficiente
→ jogador corrige ou aprova
→ salvar o aprovado
→ próximo bloco
```

Quando todas as fichas iniciais necessárias estiverem aprovadas, avançar.

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
direção narrativa e cenário são suficientes?
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

MESTRE
→ material reservado do Narrador.

OPOSITOR
→ planos, processos e informações adversariais.

LIVRO
→ histórico consolidado do que aconteceu.
```

As regras completas de onde salvar cada verdade pertencem a `registro/`.

## Criação emergente depois do START

Não é necessário prever tudo antes da primeira cena.

Lacunas futuras podem ser completadas conforme `nucleo/1.7-criacao-emergente.md`, desde que não sejam inventadas retroativamente para favorecer ou impedir uma ação já apresentada.

## Regra final

> **Nova campanha segue: nome, estrutura, direção narrativa, elenco, fichas, pareamento mínimo, situação inicial, Mesa operacional e START. A IA propõe quando puder, o jogador corrige ou aprova, e somente conteúdo aprovado vira cânone. Depois que a mesa estiver jogável, a história começa e o restante do mundo pode crescer durante a campanha.**