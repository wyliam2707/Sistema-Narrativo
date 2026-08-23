# Criação e Revisão de Personagens

Status: APROVADO

Este arquivo define como uma personagem nasce, é registrada e depois revisada dentro do sistema.

Ele **não substitui** o processo completo de criação de campanha. A campanha decide quando criar e em que ordem revisar suas personagens por meio de:

```text
sistema/criacao/README.md
```

## Princípio central

> **A ficha nasce completa em estrutura e mínima em conteúdo.**

Antes da revisão, a criação de qualquer ficha define somente três informações estruturais, nesta ordem:

```text
1 - NOME
2 - IMPORTÂNCIA
3 - CONTROLE
```

Essas são as primeiras três informações da ficha.

Se uma resposta do jogador já fornecer uma delas de forma explícita, registrá-la e não perguntar novamente; seguir para o próximo campo ainda indefinido.

`IMPORTÂNCIA` e `CONTROLE` são independentes. As regras de cada campo pertencem a `ficha.md`.

## Nascimento da ficha

Assim que `NOME + IMPORTÂNCIA + CONTROLE` estiverem definidos:

1. criar `personagens/<nome>.md`;
2. copiar o modelo-base completo de `ficha.md`;
3. usar `Status: PENDENTE DE REVISÃO`;
4. preencher somente Nome, Importância e CONTROLE;
5. deixar todos os demais campos e seções vazios.

Exemplo:

```text
# Ravena

Status: PENDENTE DE REVISÃO
Importância: Central
CONTROLE: JOGADOR IA

Idade:
Conceito:
Descrição:

TRAÇOS:

ATR: FIS [ ] | RES [ ] | MEN [ ] | VON [ ]
PER:
PODERES:
RECURSOS:
REL:

## Personalidade e tendências

## Desejos / objetivos atuais

## Medos / limites relevantes

## Conhecimento atual relevante

## História consolidada relevante
```

Não inventar ou preencher antecipadamente:

- idade;
- aparência;
- origem;
- conceito;
- personalidade;
- comportamento;
- história;
- objetivos;
- medos;
- atributos;
- perícias;
- poderes;
- TRAÇOS;
- RECURSOS;
- relações;
- conhecimento;
- qualquer outro conteúdo da ficha.

Tudo isso pertence à revisão.

> **Primeiro identificamos a peça e sua autoridade. Depois descobrimos quem ela é.**

## Campo desconhecido fica vazio

Campos ainda não revisados permanecem vazios.

Nunca usar `[0]` ou `[+0]` para representar pendência. Zero é um valor mecânico real.

```text
ATR: FIS [ ] | RES [ ] | MEN [ ] | VON [ ]
```

significa ainda não definido.

```text
ATR: FIS [0] | RES [0] | MEN [0] | VON [0]
```

significa valores mecanicamente definidos.

## Ordem das fichas na criação de campanha

A ordem canônica da revisão inicial pertence a `../criacao/README.md`:

```text
personagens JOGADOR IA
→ personagens JOGADOR IA EVENTUAL
→ protagonista
```

O protagonista é revisado por último para evitar que sua ficha sirva como régua inconsciente para calibrar as demais.

Cada personagem é revisado e calibrado isoladamente conforme `calibracao.md`.

> **A ordem protege o processo. Ela não cria balanceamento entre fichas.**

## Revisão em cinco blocos

Depois que as fichas estruturais estiverem criadas, cada ficha é construída **uma por vez** em cinco blocos:

```text
1 - Identidade e conceito
2 - Atributos e perícias
3 - Poderes e capacidades
4 - Traços e relações
5 - Conferência final
```

### Bloco 1 — Identidade e conceito

Nome, Importância e CONTROLE já chegam definidos e não precisam ser redescobertos.

Revisar e preencher, quando aplicáveis:

- origem;
- idade;
- aparência;
- conceito;
- personalidade;
- comportamento;
- história essencial;
- desejos e objetivos;
- medos e limites;
- conhecimento necessário para interpretação;
- demais elementos de identidade relevantes.

Se for personagem conhecido, canônico ou licenciado, a versão-base e eventuais combinações ou alterações são tratadas aqui, salvo quando o jogador já tiver fornecido essa informação.

A versão escolhida serve como referência inicial. O jogador pode alterar, combinar ou substituir aparência, idade, história, poderes, relações, personalidade ou qualquer outro elemento.

Depois de consolidada, a versão da campanha passa a ser a referência canônica local daquela personagem.

> **A pergunta relevante é: “qual é a versão desta campanha?”**

### Bloco 2 — Atributos e perícias

Converter e revisar o que foi estabelecido no conceito em:

```text
FIS | RES | MEN | VON
```

e nas perícias realmente relevantes.

Aplicar `calibracao.md` sem usar outra ficha como molde automático.

### Bloco 3 — Poderes e capacidades

Converter e revisar:

- poderes;
- equipamentos tratados como Poder quando aplicável;
- capacidades especiais;
- repertórios;
- limites conceituais relevantes.

Usar as regras atuais de `poderes.md`, `escala.md`, `calibracao.md` e `../resolucao/` quando necessário.

### Bloco 4 — Traços e relações

Revisar e preencher:

- TRAÇOS;
- fraquezas;
- características especiais qualitativas;
- RECURSOS recorrentes relevantes;
- relações que realmente pertençam à ficha.

### Bloco 5 — Conferência final

Verificar se o conjunto representa o conceito aprovado, corrigir incoerências, remover excessos e confirmar que não restou campo importante esquecido apenas porque estava fora da conversa.

Campos comprovadamente inúteis para aquela personagem podem ser removidos somente depois dessa conferência.

## Salvamento durante a revisão

Cada bloco aprovado é persistido imediatamente antes de avançar.

```text
bloco apresentado
→ discutir e corrigir
→ jogador aprova
→ atualizar personagens/<nome>.md
→ atualizar o checkpoint para o próximo bloco
```

Conteúdo ainda em discussão, alternativas recusadas e tentativas intermediárias não entram na ficha definitiva.

> **Bloco aprovado vira estado persistente. Conteúdo em discussão permanece apenas na conversa.**

## Organização dos arquivos na campanha

Personagens com agência de jogador possuem ficha própria em:

```text
campanhas/<nome>/personagens/<personagem>.md
```

Isso inclui qualquer personagem com:

```text
CONTROLE: JOGADOR HUMANO
CONTROLE: JOGADOR IA
CONTROLE: JOGADOR IA EVENTUAL
```

Vários personagens `JOGADOR IA EVENTUAL` podem compartilhar a mesma persona operacional, mas cada um continua sendo uma peça distinta e possui seu próprio arquivo.

NPCs comuns não pertencem por padrão a `personagens/`.

Quando um NPC precisa de persistência reservada para continuidade, sua ficha ou material operacional pertence a:

```text
campanhas/<nome>/mestre/
```

Quando houver volume suficiente, pode existir:

```text
campanhas/<nome>/mestre/npcs/
```

Não usar `mundo/npcs/` como destino padrão.

## Antagonistas reservados

Antagonistas importantes podem receber ficha completa em `mestre/` sem revisão aberta quando a apresentação revelaria informação que precisa permanecer reservada.

Isso não altera as regras de calibração.

Sempre que for prático, capacidades ocultas relevantes devem existir antes de serem usadas diretamente contra outra peça.

Depois de estabelecidas, não podem ser alteradas apenas para contrariar uma solução válida ou recuperar dificuldade.

## Estado de aprovação

Uma ficha apresentável ao jogador permanece:

```text
Status: PENDENTE DE REVISÃO
```

até a conferência final ser aprovada.

Depois da aprovação explícita:

```text
Status: APROVADO
```

A versão final não deve carregar tentativas descartadas, explicações de conversa ou versões intermediárias.

## Progressão não é criação repetida

Concluir missão, capítulo ou arco não concede automaticamente atributo, perícia, poder ou capacidade nova.

A ficha só muda posteriormente quando a própria ficção muda de forma estável o personagem.

O procedimento de atualização pertence a `../persistencia/`.

> **Criação identifica a peça e constrói sua ficha inicial. Persistência acompanha mudanças reais posteriores.**
