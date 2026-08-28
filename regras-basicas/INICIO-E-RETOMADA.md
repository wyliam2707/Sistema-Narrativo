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

Não é necessário reler todos os arquivos em toda resposta. Durante o jogo, consultar a regra específica somente quando ela realmente importar ou houver dúvida.

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

```text
CRIAÇÃO: CONCLUÍDA
→ reconstruir as cadeiras necessárias
→ carregar Estado Atual
→ carregar personagens relevantes
→ reconstruir intenções persistentes relevantes
→ continuar exatamente do ponto registrado
```

As cadeiras seguem `nucleo/1.0-tribunal.md` e o `CONTROLE` registrado nas fichas.

Uma única IA pode executar várias cadeiras conforme `nucleo/1.6-execucao-por-uma-unica-ia.md`, mantendo separação de conhecimento, objetivo e autoridade.

## O que precisa estar disponível antes da ficção

Basta existir o necessário para a situação atual:

```text
quem são as peças relevantes
quem controla cada uma
o que está acontecendo agora
onde estão
quais intenções continuam ativas
quais fatos estabelecidos importam
quais capacidades podem ser consultadas se necessárias
```

Não exigir preenchimento de informação que ainda não tenha utilidade real.

## Durante a sessão

Fluxo normal:

```text
estado + intenções persistentes
→ alguma cadeira possui motivo para nova iniciativa?
→ Narrador cruza as intenções relevantes
→ resolve somente se houver incerteza ou oposição
→ avança até o próximo ponto relevante
→ para se surgir nova decisão humana
→ narra a sentença
→ registra o que precisa continuar verdadeiro
```

O mundo pode continuar agindo durante uma intenção longa do Jogador Humano. Isso não autoriza a IA a escolher uma nova decisão por ele.

Consultar somente a fonte pertinente ao caso atual.

## Regra final

> **Para começar ou retomar, carregue o presente, as peças relevantes, suas autoridades e as intenções que ainda continuam válidas. Depois deixe cada cadeira agir dentro do próprio escopo, avance somente até a próxima decisão humana necessária e consulte detalhes sob demanda.**
