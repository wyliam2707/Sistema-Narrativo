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
→ Personagens relevantes
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
