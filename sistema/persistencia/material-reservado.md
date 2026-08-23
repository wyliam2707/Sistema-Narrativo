# Material Reservado e Escopo Operacional

Status: APROVADO

A pasta `mestre/` de uma campanha guarda **fatos, NPCs, preparações, planos e outras informações operacionais que não devem entrar automaticamente no contexto de todas as personas**.

Ela não é um mecanismo técnico de privacidade e não representa a mente completa do NARRADOR.

> **`mestre/` é uma fonte reservada da campanha. Cada persona recebe dela somente o recorte necessário à própria função.**

## Destino concreto atual

Nas campanhas do fluxo atual, material reservado pertence a:

```text
campanhas/<nome>/mestre/
```

A estrutura interna é flexível. Criar subdivisões apenas quando houver conteúdo suficiente para justificar.

Exemplo possível:

```text
campanhas/<nome>/
└── mestre/
    ├── README.md
    ├── notas.md
    ├── npcs/
    ├── segredos/
    └── preparacoes/
```

Essas subpastas são opcionais.

Não usar `aventuras/<campanha>/` para novas campanhas e não usar `mundo/npcs/` como destino padrão de NPC persistente.

## Acesso técnico não é acesso de persona

O JOGADOR HUMANO pode tecnicamente abrir qualquer arquivo do repositório se quiser.

A separação relevante é operacional entre as personas da IA:

```text
JOGADOR IA
→ recebe somente aquilo que seu personagem legitimamente sabe

JOGADOR IA EVENTUAL
→ recebe somente aquilo que sua peça legitimamente sabe

OPOSITOR
→ recebe fios, NPCs, planos e preparações necessários para mover o cenário

NARRADOR
→ consulta fatos, fichas, regras e preparações necessários para organizar e julgar
```

> **Separação de persona é separação de contexto e autoridade, não segurança técnica do repositório.**

As regras gerais de compartimentação estão em `../personas/escopo-de-consulta.md`.

## Função de `mestre/`

A pasta pode guardar, quando houver conteúdo real que justifique:

- fichas e informações operacionais de NPCs;
- identidades ocultas;
- conhecimentos secretos de NPCs;
- objetivos ainda desconhecidos;
- armadilhas e preparações já existentes;
- verdades ocultas do cenário;
- planos ainda não executados;
- sementes futuras validadas;
- possibilidades ainda não transformadas em fato;
- outras informações reservadas necessárias à continuidade.

`mestre/` não deve duplicar fichas completas de personagens que já possuem agência própria em `personagens/`.

Se uma peça com agência tiver informação reservada que não possa ficar na ficha aberta, registrar apenas o segredo necessário em `mestre/`, mantendo uma única ficha canônica em `personagens/`.

## `mestre/` não pertence exclusivamente ao NARRADOR

O nome da pasta é organizacional.

O NARRADOR não deve carregar todo o conteúdo dela por padrão.

O OPOSITOR também não deve vasculhá-la inteira apenas para procurar uma complicação.

Cada persona consulta somente o material pertinente à função do momento.

## Natureza da informação

Quando houver risco de confusão, distinguir claramente o estado do conteúdo.

### FATO

Já é verdade na campanha.

```text
FATO:
- Trigon conhece a localização do santuário.
```

### CONHECIMENTO DE NPC

Algo que determinado NPC realmente sabe.

```text
CONHECIMENTO:
- Trigon sabe que Corvin procura o grimório.
```

Isso não concede o mesmo conhecimento a outra personagem.

### PREPARAÇÃO

Algo que já foi colocado, organizado ou iniciado no mundo.

```text
PREPARAÇÃO:
- duas câmeras cobrem a entrada principal do galpão.
```

Uma preparação pode ser descoberta, evitada, neutralizada, atrasada ou tornar-se irrelevante.

### PLANO

Intenção de alguém dentro da ficção que ainda não foi executada.

```text
PLANO:
- Trigon pretende capturar Dick se surgir oportunidade.
```

Plano não é acontecimento consumado.

### POSSIBILIDADE

Ideia ainda não transformada em verdade da ficção.

```text
POSSIBILIDADE:
- Trigon pode tentar negociar com Ravena em algum momento.
```

Possibilidade não fundamenta resolução como se já fosse fato.

## Proposto, validado e acontecido

Durante o jogo:

```text
PROPOSTO
→ uma persona sugere um movimento possível

VALIDADO
→ o NARRADOR confirma fundamento, meios, condições e tempo necessários

ACONTECIDO
→ a ação foi efetivamente estabelecida na ficção
```

Uma proposta não se torna automaticamente fato.

Uma preparação validada pode existir antes de produzir acontecimento. Quando o acontecimento ocorrer, o Livro registra o que realmente aconteceu.

## NPCs persistentes

NPCs persistentes ou com informação operacional relevante podem ser registrados em:

```text
campanhas/<nome>/mestre/npcs/
```

quando essa subdivisão for útil.

Suas fichas seguem as mesmas regras gerais de personagem.

Enquanto forem NPCs:

```text
CONTROLE: NPC
```

Se uma personagem passar formalmente a possuir `CONTROLE: JOGADOR IA EVENTUAL`, sua ficha canônica passa para:

```text
campanhas/<nome>/personagens/<personagem>.md
```

Material secreto separado pode continuar em `mestre/` quando necessário.

## Relação com o OPOSITOR

O OPOSITOR usa material reservado para mover o cenário a partir de fatos reais, não para fabricar uma resposta sob medida depois que o jogador encontrou uma solução.

Pode receber, conforme necessário:

- gancho antigo;
- consequência parada;
- plano de NPC;
- preparação futura;
- NPC disponível;
- oportunidade;
- ameaça;
- visita possível;
- informação de passagem de tempo;
- outro fio capaz de gerar movimento.

Sua pergunta típica é:

> **Isso aqui pode se mover agora?**

O NARRADOR julga a proposta.

## Relação com o NARRADOR

O NARRADOR consulta `mestre/` somente quando algum conteúdo for necessário para:

- validar uma proposta;
- verificar capacidade ou conhecimento de NPC;
- confirmar preparação;
- julgar uma resolução;
- registrar novo estado operacional.

> **O NARRADOR organiza, julga e registra. O OPOSITOR movimenta fios disponíveis.**

## Relação com o estado atual

`mestre/` e `estado/atual.md` cumprem funções diferentes.

```text
mestre/
→ verdade ou intenção reservada de condução

estado/atual.md
→ retrato operacional necessário para continuar agora
```

Um plano secreto pode permanecer somente em `mestre/`.

Se uma consequência reservada já está ativa e precisa ser conhecida pelo NARRADOR para retomar corretamente o momento presente, o estado pode apontar de forma operacional para a fonte reservada sem revelar ao jogador o conteúdo que sua personagem não conhece.

Não duplicar automaticamente todo material reservado em `estado/atual.md`.

## Relação com o Livro

```text
mestre/
→ guarda realidade operacional, planos e preparações reservadas ainda úteis

livro/
→ registra aquilo que efetivamente aconteceu
```

Plano não executado não entra no Livro como fato.

Ação secreta efetivamente acontecida pode entrar no Livro como parte da realidade completa da campanha, conforme `livro.md`, sem conceder metaconhecimento às personagens.

## Relação com Progressão

Progressão descreve consequências estabelecidas que continuam causalmente vivas.

Na estrutura atual, um fio causal presente pode ser persistido em `estado/atual.md`; quando sua natureza precisar permanecer reservada, a fonte detalhada pode ficar em `mestre/`.

Não duplicar automaticamente a mesma informação em várias fontes.

## Proibição de criação retroativa

`mestre/` não é uma caixa-preta para justificar qualquer coisa depois que o jogador encontrou uma solução eficaz.

Não criar retroativamente, apenas por conveniência:

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
- outro fato destinado a alterar um resultado já encaminhado.

O OPOSITOR pode propor movimento novo para o futuro. Não pode inventar que esse movimento já existia no passado.

> **Semente futura pode nascer agora. Defesa retroativa não.**

## Regra final

```text
JOGADORES
→ recebem a visão legítima de suas peças

OPOSITOR
→ recebe fios suficientes para mover o cenário

NARRADOR
→ recebe o necessário para organizar, julgar e registrar

mestre/
→ preserva a fonte operacional reservada da campanha
```

> **O arquivo pode existir tecnicamente no mesmo repositório. O conhecimento pertence somente a quem o adquiriu legitimamente na ficção.**
