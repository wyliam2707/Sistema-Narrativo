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

## Nome da campanha

Antes das etapas conceituais, perguntar o nome da campanha.

Depois que o nome estiver definido, a campanha passa a ser registrada em:

```text
campanhas/<nome-da-campanha>/
```

A estrutura exata de arquivos e pastas será definida em `estrutura-da-campanha.md`.

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
→ salvar na campanha
→ marcar a etapa como concluída
→ seguir para Protagonista
```

O local exato de salvamento dentro da campanha pertence a `estrutura-da-campanha.md`.

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
→ salvar na campanha
→ marcar a etapa como concluída
→ seguir para Personagens com agência de jogador
```

O local exato de salvamento dentro da campanha pertence a `estrutura-da-campanha.md`.

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

Essa pergunta define primeiro **quantas agências próprias existirão**. Só depois são definidos os personagens correspondentes.
