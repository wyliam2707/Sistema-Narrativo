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
mestre/roteiro.md
+ estado/atual.md
+ fichas das personagens atualmente relevantes
```

Essas três fontes possuem funções diferentes:

```text
ROTEIRO DA CAMPANHA
→ foco, tom, premissa, trama de fundo e limites de direção.

FICHA DA PERSONAGEM
→ principal fonte de interpretação, capacidades, relações e conhecimento consolidado.

ESTADO ATUAL
→ situação temporária, marcas, Mana, posição e processos atuais.

LIVROS / MUNDO / OUTROS ARQUIVOS
→ contexto externo consultado quando necessário.
```

O roteiro não determina resultados nem substitui o julgamento. Ele impede que a campanha perca sua direção por causa de uma trama secundária, improvisação ou mudança automática de tom.

Conhecimento registrado na ficha já faz parte da personagem. Não apresentar novamente como descoberta, nem reiniciar automaticamente um conflito de aceitação ou aprendizado que já esteja consolidado.

Consultar outros arquivos de `mundo/`, `mestre/`, `opositor/`, conhecimento ou Livro somente quando forem necessários para a cena ou para resolver dúvida real.

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
→ carregar Roteiro da Campanha
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
sobre o que esta campanha é
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
roteiro + estado + intenções persistentes
→ alguma cadeira possui motivo para nova iniciativa?
→ interpretar cada personagem a partir da própria ficha
→ Narrador cruza as intenções relevantes
→ resolve somente se houver incerteza ou oposição
→ avança até o próximo ponto relevante
→ para se surgir nova decisão humana
→ narra a sentença dentro da direção da campanha
→ registra o que precisa continuar verdadeiro
```

O mundo pode continuar agindo durante uma intenção longa do Jogador Humano. Isso não autoriza a IA a escolher uma nova decisão por ele.

Uma miniquest, investigação, combate ou outro desvio local pode ocupar a cena quando fizer sentido, mas não substitui automaticamente o foco principal registrado no roteiro.

Consultar somente a fonte pertinente ao caso atual.

## Regra final

> **Para começar ou retomar, carregue o roteiro, o presente e as fichas das peças relevantes. O roteiro preserva a direção da campanha; a ficha é a principal fonte de interpretação da personagem; Estado Atual registra o temporário e livros ou outros arquivos fornecem contexto externo sob demanda. Conhecimento já consolidado não deve ser redescoberto sem fato novo.**
