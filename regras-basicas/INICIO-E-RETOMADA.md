# Início e Retomada

Status: REFORMULAÇÃO / NÃO IMPLEMENTADO

Este arquivo define como uma IA começa ou retoma uma campanha usando `regras-basicas/` sem depender de `sistema/`.

> **Carregar somente o necessário para jogar corretamente. Não transformar preparação em uma segunda sessão.**

## Entrada

No primeiro contato:

```text
ler regras-basicas/README.md
→ compreender Núcleo, Jogador, Mestre, Opositor e Registro
→ Nova campanha ou Continuar?
```

Não é necessário reler todos os arquivos em toda resposta. Durante o jogo, consultar a regra específica quando ela realmente importar ou houver dúvida.

## Nova campanha

Seguir:

```text
CRIACAO-DE-CAMPANHA.md
```

A ficção só começa quando existir informação suficiente para apresentar a primeira cena sem inventar escolhas ou fatos estruturais essenciais.

## Continuar campanha

Abrir:

```text
campanhas/<nome>/README.md
```

Depois carregar, no mínimo:

```text
estado/atual.md
+ fichas das personagens atualmente relevantes
```

Consultar `mundo/`, `mestre/`, `opositor/`, conhecimento ou Livro somente quando forem necessários para a cena ou para resolver dúvida real.

Não pedir novamente informação que já esteja registrada em fonte canônica da campanha.

## Campanha em criação

```text
CRIAÇÃO: EM ANDAMENTO
→ retomar do ponto registrado
→ não iniciar ficção ainda
```

## Campanha pronta

Quando a campanha estiver pronta:

```text
CRIAÇÃO: CONCLUÍDA
→ reconstruir as cadeiras necessárias
→ carregar Estado Atual
→ carregar personagens relevantes
→ continuar exatamente do ponto registrado
```

As cadeiras seguem o Tribunal em `nucleo/1.0-tribunal.md` e o `CONTROLE` registrado nas fichas.

Uma única IA pode executar várias cadeiras conforme `nucleo/1.6-execucao-por-uma-unica-ia.md`, mantendo separação de conhecimento, objetivo e autoridade.

## O que precisa estar disponível antes da ficção

Basta existir o necessário para a situação atual:

```text
quem são as peças relevantes
quem controla cada uma
o que está acontecendo agora
onde estão
quais fatos já estabelecidos importam
quais capacidades podem ser consultadas se necessárias
```

Não exigir preenchimento de informação que ainda não tenha utilidade real.

## Durante a sessão

Fluxo normal:

```text
situação aberta
→ cadeiras declaram
→ Narrador julga
→ resolve somente se houver incerteza
→ narra a sentença
→ registra o que precisa continuar verdadeiro
```

Consultar somente a fonte pertinente ao caso atual.

## Regra final

> **Para começar ou retomar, carregue a campanha até compreender o presente, as peças relevantes e suas autoridades. Depois jogue normalmente. Consulte detalhes sob demanda e nunca peça ao jogador algo que a campanha já sabe.**
