# Material Reservado e Escopo Operacional

Status: APROVADO

A pasta `mestre/` guarda fatos, NPCs, preparações, planos e outras informações operacionais que não devem entrar automaticamente no contexto de todas as personas.

Ela não é um mecanismo técnico de privacidade.

> **`mestre/` é uma fonte reservada da campanha. Cada persona recebe dela somente o recorte necessário à própria função.**

## Destino concreto

```text
campanhas/<nome>/mestre/
```

Subdivisões são opcionais e só devem existir quando houver conteúdo suficiente para justificar.

Exemplo:

```text
mestre/
├── README.md
├── npcs/
├── segredos/
└── preparacoes/
```

NPC persistente sem agência de jogador pertence a `mestre/`, não a `mundo/npcs/`.

## Acesso técnico não é conhecimento de personagem

O fato de uma informação existir no repositório não significa que uma personagem a conhece.

```text
JOGADOR IA
→ recebe somente o que sua peça legitimamente sabe.

JOGADOR IA EVENTUAL
→ recebe somente o que a peça assumida legitimamente sabe.

OPOSITOR
→ pode consultar fios e recursos necessários para apresentar movimentos e oposição.

NARRADOR
→ consulta somente o que precisa para julgar, narrar a sentença e registrar corretamente.
```

A compartimentação geral segue `../personas/escopo-de-consulta.md`.

## O que pode existir em `mestre/`

Quando necessário:

- fichas e informações operacionais de NPCs;
- identidades ocultas;
- conhecimento secreto de um agente;
- objetivos desconhecidos;
- armadilhas e preparações já existentes;
- verdades ocultas do cenário;
- planos ainda não executados;
- possibilidades reservadas ainda não transformadas em fato;
- outras informações necessárias à continuidade.

Não duplicar ficha completa de personagem que já possui agência própria em `personagens/`.

## Estados da informação

Quando houver risco de confusão, distinguir:

### FATO

Já é verdade.

```text
FATO:
- Trigon conhece a localização do santuário.
```

### CONHECIMENTO

Algo que determinado agente sabe.

```text
CONHECIMENTO — Trigon:
- Corvin procura o grimório.
```

Conhecimento de um agente não se transfere automaticamente a outro.

### PREPARAÇÃO

Algo que já foi colocado, iniciado ou organizado no mundo.

```text
PREPARAÇÃO:
- duas câmeras cobrem a entrada principal.
```

### PLANO

Intenção ainda não executada.

```text
PLANO:
- Trigon pretende capturar Ravena se surgir oportunidade.
```

### POSSIBILIDADE

Ideia ainda não estabelecida na ficção.

```text
POSSIBILIDADE:
- Trigon pode tentar negociar em algum momento.
```

Possibilidade não pode ser usada como se fosse fato anterior.

## Proposto, julgado e acontecido

```text
PROPOSTO
→ jogador, JOGADOR IA, JOGADOR IA EVENTUAL ou OPOSITOR apresenta uma intenção ou movimento.

JULGADO
→ NARRADOR verifica fatos, conhecimento, meios, oportunidade e regras.

ACONTECIDO
→ a resolução/sentença estabelece o que efetivamente passou a ser verdade.
```

Proposta não é fato. Plano não é acontecimento. Preparação existente pode produzir consequência somente quando a situação realmente a aciona.

## NPCs persistentes

NPCs que precisam de continuidade própria podem ficar em:

```text
campanhas/<nome>/mestre/npcs/
```

Enquanto forem NPCs:

```text
CONTROLE: NPC
```

Se passarem formalmente a possuir agência de jogador aprovada, sua ficha canônica passa para `personagens/` conforme as regras de criação/personagem. Segredos separados podem permanecer em `mestre/`.

## OPOSITOR

O OPOSITOR pode usar material reservado para apresentar movimento a partir de fatos reais.

Pode consultar, quando pertinente:

- ganchos;
- consequências vivas;
- planos;
- preparações;
- NPCs disponíveis;
- recursos legítimos;
- oportunidades;
- ameaças;
- passagem de tempo relevante.

Ele não pode inventar retroativamente uma preparação apenas porque isso melhoraria a oposição.

> **O OPOSITOR argumenta e movimenta. O NARRADOR julga.**

## NARRADOR

O NARRADOR consulta `mestre/` quando isso for necessário para:

- validar uma proposta;
- verificar conhecimento ou capacidade;
- confirmar preparação existente;
- julgar uma resolução;
- narrar corretamente a sentença;
- registrar o resultado já estabelecido.

O NARRADOR não vasculha material reservado para procurar uma complicação nova. Essa iniciativa pertence ao OPOSITOR.

## Relação com `estado/atual.md`

```text
mestre/
→ detalhe reservado.

estado/atual.md
→ retrato necessário para continuar agora.
```

Um plano secreto pode ficar apenas em `mestre/`.

Quando a retomada exige saber que existe uma fonte reservada relevante, `estado/atual.md` pode apontar para ela sem duplicar o conteúdo.

## Relação com ganchos do OPOSITOR

O arquivo:

```text
campanhas/<nome>/mestre/ganchos-do-opositor.md
```

é uma lista simples de oportunidades atuais, conforme `../agencia/ganchos-do-opositor.md`.

Ele não substitui todo `mestre/` e não precisa repetir fichas, planos completos ou segredos já armazenados em outra fonte.

## Relação com o Livro

```text
mestre/
→ guarda fatos, planos e preparações reservadas ainda úteis.

livro/
→ registra aquilo que efetivamente aconteceu.
```

Plano não executado não entra no Livro como fato.

Ação secreta efetivamente ocorrida pode entrar no Livro conforme `livro.md`, sem conceder esse conhecimento às personagens.

## Proibição de criação retroativa

Não criar retroativamente, apenas para alterar um resultado já encaminhado:

- imunidade;
- poder;
- recurso;
- guarda;
- armadilha;
- conhecimento;
- passagem secreta;
- aliança;
- preparação;
- regra local;
- qualquer outro fato anterior inexistente.

> **Semente futura pode nascer agora. Defesa retroativa não.**

## Regra final

> **`mestre/` preserva informação reservada. OPOSITOR pode usá-la para apresentar movimentos legítimos. NARRADOR consulta somente para julgar, narrar a sentença e registrar. Conhecimento operacional da IA nunca vira automaticamente conhecimento de personagem.**