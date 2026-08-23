# Criação de Campanha

Status: EM REVISÃO

Este arquivo é a porta de entrada para **criar uma nova campanha**.

Ele ensina outra IA ou narrador a conduzir a criação. Os dados concretos da campanha não pertencem a `sistema/criacao/`: devem ser salvos diretamente em `campanhas/<nome-da-campanha>/` conforme a estrutura definida para campanhas.

> **O sistema ensina como criar. A campanha guarda o que foi criado.**

## Princípios

> **Conceito primeiro. Mecânica depois.**

Durante a criação:

- fazer uma pergunta por vez;
- não pedir novamente informação que o jogador já forneceu;
- interpretar respostas livres normalmente;
- perguntar somente o que ainda fizer diferença real;
- parar de perguntar quando já houver informação suficiente para fechar a etapa;
- consolidar uma etapa antes de avançar para a próxima;
- salvar somente a versão consolidada, não cada tentativa intermediária.

## Exemplos e respostas numéricas

Quando uma pergunta se beneficiar de exemplos, apresentá-los numerados, uma opção por linha:

```text
1 - opção
2 - opção
3 - opção
```

O jogador pode responder de qualquer destas formas:

```text
6
```

Escolhe a opção 6.

```text
2 + 5
```

Combina as opções 2 e 5.

```text
Quero investigação sobrenatural com romance lento e humor seco.
```

Descreve uma combinação própria.

> **Os exemplos numerados são atalhos de resposta, nunca uma lista fechada.**

A IA deve aproveitar tudo que já estiver claro na resposta e não transformar os exemplos em formulário obrigatório.

## Fluxo geral

A criação segue esta ordem:

```text
Nome da campanha
→ Direção narrativa e cenário
→ Protagonista
→ Personagens com agência de jogador
→ Início da história
→ Revisão mecânica e aprovação
```

O nome abre a campanha. As etapas seguintes constroem seu conteúdo.

## Checkpoint da criação

Enquanto a campanha estiver sendo criada, o `README.md` da própria campanha deve registrar **onde o processo precisa ser retomado**.

O checkpoint não guarda o conteúdo da etapa. Ele registra somente o ponto operacional de continuação.

Forma mínima:

```text
CRIAÇÃO: EM ANDAMENTO

Etapa atual: Protagonista
```

Quando a revisão mecânica exigir mais precisão:

```text
CRIAÇÃO: EM ANDAMENTO

Etapa atual: Revisão mecânica e aprovação
Personagem atual: Ravena
Bloco atual: 3 - Poderes e capacidades
```

Ao concluir uma etapa e avançar para outra, atualizar o checkpoint para a nova etapa antes de continuar. Durante a revisão mecânica, atualizar também personagem e bloco sempre que a revisão avançar.

Quando toda a criação terminar:

```text
CRIAÇÃO: CONCLUÍDA
```

Não manter uma lista obrigatória de etapas `NÃO INICIADO`, `PENDENTE` ou semelhantes. O checkpoint deve mostrar somente **onde continuar agora**.

> **O conteúdo fica em seus arquivos próprios. O checkpoint diz somente de onde retomar a criação.**

## Destino canônico de cada etapa

Cada informação produzida durante a criação possui uma **fonte principal**. O `README.md` resume e orienta; não deve duplicar o conteúdo completo dos arquivos concretos.

```text
NOME
→ README.md
→ cria toda a estrutura-base

DIREÇÃO NARRATIVA
→ resumo em README.md

CENÁRIO
→ resumo necessário em README.md
→ detalhes estáveis, quando precisarem de desenvolvimento próprio, em mundo/

PROTAGONISTA
→ personagens/<nome>.md
→ identificação + CONTROLE no README.md

PERSONAGENS JOGADOR IA / JOGADOR IA EVENTUAL
→ personagens/<nome>.md
→ identificação + CONTROLE no README.md

INÍCIO DA HISTÓRIA
→ situação inicial concreta em estado/atual.md
→ README.md apenas aponta a retomada para estado/atual.md

CHECKPOINT DA CRIAÇÃO
→ README.md
```

Não criar um segundo arquivo apenas para repetir informação que já possui fonte principal.

Exemplo:

```text
README.md
Direção narrativa: romance sobrenatural adulto, cotidiano e humor.

mundo/gotham.md
→ detalhes persistentes de Gotham quando realmente precisarem de desenvolvimento próprio

estado/atual.md
→ situação inicial concreta de onde a primeira cena parte
```

> **Cada informação possui uma fonte principal. O README resume e orienta; não replica os arquivos concretos.**

## Nome da campanha

Antes das etapas conceituais, perguntar o nome da campanha.

Assim que o nome estiver definido, criar imediatamente:

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

Os READMEs internos devem explicar de forma curta para que serve cada área e quais regras do sistema precisam ser consultadas. Eles materializam as pastas no repositório e tornam a campanha autoexplicativa para outra IA.

O `README.md` da raiz da campanha já deve nascer com:

- nome da campanha;
- `CRIAÇÃO: EM ANDAMENTO`;
- `Etapa atual: Direção narrativa e cenário`;
- mapa de consulta da estrutura;
- espaços ainda não definidos claramente marcados como pendentes de criação.

`estado/atual.md` deve nascer com conteúdo mínimo indicando que a campanha ainda está em criação e que a situação inicial será registrada quando definida.

Depois disso, continuar normalmente para Direção narrativa e cenário.

> **NOME DEFINIDO → estrutura-base criada → criação continua.**

A função e o conteúdo de cada entrada estão definidos em `estrutura-da-campanha.md`.

# Etapa — Direção narrativa e cenário

Esta etapa responde a duas perguntas diferentes, mas relacionadas:

```text
Direção narrativa → Que tipo de experiência esta campanha quer produzir?
Cenário           → Que mundo existe e quais fatos básicos precisamos saber para começar?
```

## Direção narrativa

Definir somente o que realmente influencia como a campanha deve ser conduzida.

Podem importar, conforme a resposta do jogador:

- gênero;
- tom;
- foco;
- ritmo;
- presença de romance, humor, terror, investigação, ação, cotidiano ou outros elementos;
- preferências específicas de narração que realmente alterem a experiência.

Exemplo de pergunta:

> **Que tipo de história você quer viver?**

Exemplos possíveis:

```text
1 - Aventura épica
2 - Investigação sobrenatural
3 - Romance
4 - Comédia romântica
5 - Terror
6 - Romance adulto com humor
7 - Ação e aventura
8 - Cotidiano com drama
9 - Política e intriga
10 - Outro / combinação própria
```

A lista é apenas orientação. O jogador pode escolher um número, combinar opções ou descrever livremente outra proposta.

## Cenário

Definir apenas os fatos de mundo necessários para sustentar os personagens e a abertura da história.

Podem importar, conforme o caso:

- universo ou tipo de cenário;
- local principal;
- época;
- tecnologia;
- magia ou sobrenatural;
- organizações essenciais;
- regras especiais do mundo;
- grau de fidelidade ou adaptação, quando for fanfic ou cenário conhecido.

Exemplos de cenário:

```text
1 - Universo de super-heróis adaptado
2 - Fantasia medieval própria
3 - Cidade contemporânea com sobrenatural oculto
4 - Futuro cyberpunk
5 - Horror urbano
6 - Outro / combinação própria
```

## Regra de suficiência

> **Definir somente o necessário para sustentar os personagens e a abertura da história.**

Não construir uma enciclopédia antes de jogar.

Quando direção narrativa e cenário estiverem suficientemente claros:

```text
consolidar
→ atualizar Direção narrativa e Cenário no README.md
→ registrar em mundo/ somente detalhes estáveis que precisem de arquivo próprio
→ atualizar o checkpoint para Protagonista
→ seguir para Protagonista
```

# Etapa — Protagonista

Esta etapa constrói a **ficha conceitual** do personagem principal antes de qualquer conversão mecânica.

Pergunta-base:

> **Quem é o personagem principal que o jogador quer interpretar?**

Quando exemplos ajudarem, a IA pode apresentar conceitos como:

```text
1 - Humano comum envolvido em algo extraordinário
2 - Herói ou vigilante
3 - Mago / usuário de magia
4 - Vampiro ou criatura sobrenatural
5 - Mutante / super-humano
6 - Guerreiro / aventureiro
7 - Anti-herói
8 - Personagem já existente de outro universo
9 - Conceito próprio / combinação
```

O jogador pode responder por número, combinar opções ou descrever livremente outro conceito.

## Criação conceitual

A IA pode propor ideias para ajudar a construir a ficha, incluindo quando forem úteis:

- identidade;
- aparência e presença;
- origem;
- personalidade;
- comportamento;
- história essencial;
- relações importantes;
- desejos e objetivos;
- medos e conflitos;
- limitações narrativas;
- capacidades descritas apenas em linguagem conceitual.

Exemplos válidos de capacidade conceitual:

```text
Manipula realidade através da vontade.
Percebe fenômenos sobrenaturais.
Consegue criar portais.
Conhece rituais antigos.
```

Nesta etapa não definir atributos, perícias, patamares, valores numéricos ou qualquer outro detalhe mecânico.

> **A IA pode gerar ideias para a ficha, mas sugestões são matéria-prima. Só entram na ficha quando o jogador aceitar, modificar ou incorporar a ideia.**

## Limite de perguntas

A etapa Protagonista possui **no máximo 5 perguntas principais**.

Esse é um teto, não uma meta.

A IA deve:

- fazer menos perguntas quando já houver informação suficiente;
- aproveitar tudo que o jogador já respondeu;
- nunca perguntar apenas para preencher campos;
- não transformar a criação em biografia enciclopédica;
- deixar detalhes menores surgirem depois, quando realmente importarem.

> **O limite é de perguntas, não de informação.**

Quando o protagonista estiver conceitualmente claro o bastante para ser interpretado e revisado depois:

```text
consolidar
→ criar ou atualizar personagens/<nome>.md
→ registrar no README.md sua identificação e CONTROLE
→ atualizar o checkpoint para Personagens com agência de jogador
→ seguir para Personagens com agência de jogador
```

# Etapa — Personagens com agência de jogador

Esta etapa existe somente para definir personagens que serão controlados por `JOGADOR IA` ou `JOGADOR IA EVENTUAL`.

NPCs comuns, aliados ocasionais, figurantes e adversários não pertencem a esta etapa.

A primeira pergunta deve definir o arranjo de agência da campanha:

> **Você quer ter personagens controlados por JOGADOR IA ou JOGADOR IA EVENTUAL nesta campanha?**

Exemplos:

```text
1 - Sim, 1 JOGADOR IA dedicado
2 - Sim, 2 JOGADORES IA dedicados
3 - Sim, somente JOGADOR IA EVENTUAL
4 - Sim, JOGADOR IA dedicado + JOGADOR IA EVENTUAL
5 - Sim, 2 JOGADORES IA dedicados + JOGADOR IA EVENTUAL
6 - Não, nenhum personagem controlado por IA no início
7 - Outro arranjo dentro dos limites do sistema
```

Essa pergunta define primeiro **quantas agências próprias existirão**.

## Nome e gerência vêm primeiro

Depois de definido o arranjo, identificar os personagens **um por vez**.

Neste primeiro momento, registrar somente:

```text
NOME
GERÊNCIA
```

A gerência deve ser uma das categorias já escolhidas para a campanha:

```text
JOGADOR IA
JOGADOR IA EVENTUAL
```

Exemplo:

```text
Ravena — JOGADOR IA
Dick — JOGADOR IA EVENTUAL
Kory — JOGADOR IA EVENTUAL
```

Não definir ainda função narrativa, personalidade, relação com o protagonista, história, capacidades ou mecânica.

> **Primeiro o sistema estabelece quais peças existem e quem gerencia cada uma.**

## Personagens conhecidos e versões

Quando um personagem conhecido, canônico ou licenciado possuir versões diferentes, o jogador escolhe a versão-base que será usada na campanha.

Essa versão é somente a referência inicial. O jogador pode alterar, combinar ou substituir elementos como aparência, idade, história, poderes, relações, personalidade ou qualquer outro aspecto durante a criação.

Se o jogador já tiver indicado uma versão ou combinação suficiente para identificar a personagem da campanha, não perguntar novamente qual versão usar.

Depois que a versão da campanha estiver consolidada, ela passa a ser a referência canônica local para aquela personagem. O cânone externo continua servindo como fonte de apoio, não como limite obrigatório.

> **A pergunta relevante não é “qual é a versão oficial?”, mas “qual é a versão desta campanha?”.**

## Ficha conceitual preliminar

Depois de registrar `NOME + GERÊNCIA`, não fazer perguntas adicionais por padrão.

A IA deve usar o cenário, o nome do personagem e tudo que já estiver definido na campanha para montar uma **ficha conceitual preliminar** compatível com o material existente.

Essa ficha é uma proposta, não uma definição final. Ela deve ser marcada como:

```text
PENDENTE DE REVISÃO
```

O jogador poderá aceitar, corrigir, remover, acrescentar ou pedir novas ideias durante a revisão.

Nesta etapa não fechar atributos, perícias, patamares, valores numéricos ou outros detalhes mecânicos.

> **NOME + GERÊNCIA → ficha conceitual preliminar → PENDENTE DE REVISÃO.**

Para cada personagem identificado, criar ou atualizar `personagens/<nome>.md` e registrar sua identificação + controle no `README.md` da campanha.

Quando os personagens com agência de jogador estiverem registrados e suas fichas preliminares preparadas:

```text
atualizar o checkpoint para Início da história
→ seguir para Início da história
```

# Etapa — Início da história

Esta etapa define somente **de onde a primeira cena parte**. Ela não cria a trama inteira nem determina antecipadamente o que acontecerá depois.

Pergunta-base:

> **Como você quer que a história comece?**

Exemplos:

```text
1 - Cotidiano do protagonista antes de algo acontecer
2 - Já no meio de um acontecimento
3 - Encontro com outro personagem importante
4 - Chegada a um novo lugar
5 - Missão, trabalho ou objetivo já em andamento
6 - Problema ou ameaça aparece
7 - Quero que o NARRADOR escolha uma abertura coerente
8 - Outro / combinação própria
```

O jogador pode responder por número, combinar opções ou descrever livremente uma situação inicial.

## Limite de perguntas

A etapa possui **no máximo 5 perguntas principais**.

Esse é um teto, não uma meta. A IA deve aproveitar tudo que já estiver definido na campanha e fazer menos perguntas sempre que possível.

As perguntas servem apenas para esclarecer elementos que realmente alterem a abertura, como lugar, momento, situação imediata ou presença inicial de personagens.

Não usar essa etapa para planejar capítulos futuros, arcos completos, antagonistas ocultos ou acontecimentos que ainda devem nascer durante o jogo.

> **Definir somente a situação inicial. O que acontece depois pertence ao jogo, não à criação da campanha.**

## Resumo do início

Quando a abertura estiver suficientemente clara, produzir um **resumo curto do início da história**.

Esse resumo deve registrar apenas os fatos necessários para o NARRADOR abrir a primeira cena de forma reproduzível, sem narrar antecipadamente a cena e sem decidir ações dos jogadores.

Depois:

```text
consolidar o resumo do início
→ registrar a situação inicial concreta em estado/atual.md
→ fazer README.md apontar Situação de entrada para estado/atual.md
→ atualizar o checkpoint para Revisão mecânica e aprovação
→ seguir para Revisão mecânica e aprovação
```

# Etapa — Revisão mecânica e aprovação

Nenhuma ficha conceitual vira ficha final automaticamente.

A revisão deve acontecer **uma ficha por vez**.

A ordem é:

```text
personagens JOGADOR IA
→ personagens JOGADOR IA EVENTUAL
→ protagonista
```

O protagonista deve ser revisado **por último**, para evitar que sua ficha contamine a construção ou calibração das demais fichas.

Cada ficha deve ser convertida e revisada a partir do próprio conceito, do cenário e das regras do sistema, sem usar outra ficha como molde automático.

> **Cada personagem é calibrado pelo que ele é. O protagonista não serve como régua para os demais.**

## Revisão em blocos

Cada ficha deve ser apresentada e revisada em **5 blocos**, um por vez.

```text
1 - Identidade e conceito
2 - Atributos e perícias
3 - Poderes e capacidades
4 - Traços e relações
5 - Conferência final
```

### Bloco 1 — Identidade e conceito

Revisar nome, gerência, origem, aparência, personalidade, comportamento, história essencial e papel narrativo quando aplicáveis.

### Bloco 2 — Atributos e perícias

Converter e revisar o conceito nos atributos `FIS | RES | MEN | VON` e nas perícias realmente relevantes para o personagem.

### Bloco 3 — Poderes e capacidades

Converter e revisar poderes, equipamentos tratados como Poder quando aplicável, capacidades relevantes e seus limites conceituais segundo as regras do sistema.

### Bloco 4 — Traços e relações

Revisar traços permanentes, fraquezas, características especiais e relações iniciais que realmente pertençam à ficha.

### Bloco 5 — Conferência final

Verificar se o conjunto mecânico representa o conceito aprovado, corrigir incoerências, remover excessos e somente então considerar a ficha pronta para aprovação.

> **Apresentar um bloco por vez. Só avançar para o próximo depois da revisão do jogador.**

## Salvamento por bloco

Durante a revisão mecânica, conteúdo ainda em discussão não deve ser persistido como definitivo.

Cada bloco aprovado deve ser consolidado **imediatamente** na ficha do personagem antes de avançar para o próximo bloco.

```text
bloco apresentado
→ discutir e corrigir
→ jogador aprova
→ atualizar personagens/<nome>.md
→ atualizar o checkpoint para o próximo bloco
```

Não salvar tentativas intermediárias, alternativas recusadas ou valores ainda não aprovados.

Se a conversa for interrompida, os blocos já aprovados permanecem preservados na ficha e o checkpoint indica exatamente qual bloco deve ser retomado.

> **Bloco aprovado vira estado persistente da ficha. Conteúdo em discussão continua apenas na conversa.**

Se um bloco for alterado de forma que afete outro já revisado, corrigir somente o que tiver sido realmente impactado antes da aprovação final.

## Início do jogo

Quando todas as fichas tiverem concluído a revisão e forem aprovadas, a criação termina sem etapa intermediária adicional.

Antes de abrir a primeira cena, o sistema deve **consolidar automaticamente** em `estado/atual.md` a situação inicial exata da campanha usando apenas fatos já aprovados e necessários para o ponto de entrada. Essa consolidação não cria uma nova etapa, não exige nova confirmação do jogador e não deve copiar fichas completas para o estado.

Depois, atualizar o `README.md` da campanha para:

```text
CRIAÇÃO: CONCLUÍDA
```

Somente então o NARRADOR abre a primeira cena a partir de `estado/atual.md`.

```text
fichas aprovadas
→ consolidar estado inicial em estado/atual.md
→ marcar CRIAÇÃO: CONCLUÍDA
→ NARRADOR abre a primeira cena
```

Não criar uma fase separada de preparação, não exigir nova confirmação de prontidão e não antecipar acontecimentos além do que já estiver estabelecido para a abertura.

> **A criação termina em persistência automática. A primeira cena começa a partir do estado já consolidado.**
