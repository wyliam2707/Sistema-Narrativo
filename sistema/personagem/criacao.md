# Criação e Revisão de Personagens

Status: APROVADO

Este arquivo define a criação de um personagem como entidade do sistema.

Ele **não substitui** o processo completo de criação de campanha. A campanha decide quando criar e em que ordem revisar suas personagens por meio de:

```text
sistema/criacao/README.md
```

Este arquivo define como um personagem deve ser concebido e convertido para ficha.

## Princípio central

> **Conceito primeiro. Mecânica depois.**

A criação deve começar por quem o personagem é, não por distribuir números.

## Etapa conceitual

Antes de calibrar a ficha mecânica, definir somente o que for realmente necessário para compreender o personagem.

Podem importar:

- nome;
- natureza ou origem;
- aparência;
- idade real e aparente, quando diferentes;
- conceito;
- personalidade;
- comportamento social;
- história essencial;
- ocupações ou trajetória importante;
- desejos e objetivos;
- medos e limites;
- TRAÇOS permanentes;
- `CONTROLE`, quando já definido pela estrutura da campanha.

Não é obrigatório preencher todos esses campos.

> **Perguntar e registrar apenas aquilo que realmente ajuda a definir o personagem.**

Estado circunstancial da cena não deve ser confundido com conceito estável da ficha.

## Estrutura de ficha desde o começo

O arquivo do personagem pode usar desde a criação a estrutura final descrita em `ficha.md`.

Preencher apenas os campos já conhecidos.

Campos ainda desconhecidos ficam vazios.

> **Nunca usar `[0]` ou `[+0]` para representar pendência. Zero é um valor mecânico real.**

## O que não calibrar na etapa conceitual

Enquanto o conceito ainda está sendo construído, não atribuir automaticamente:

- FIS;
- RES;
- MEN;
- VON;
- graus de perícia;
- graus de poderes;
- especializações numéricas;
- relações numéricas ainda não estabelecidas.

Esses elementos entram na conversão mecânica.

## Criação mínima

Qualquer personagem pode nascer com uma ficha mínima.

Pode ser suficiente inicialmente registrar:

- nome;
- `CONTROLE`, quando já decidido;
- importância, quando realmente necessária;
- conceito já estabelecido.

Importância não determina tamanho, formato ou quantidade de detalhe da ficha.

Não inventar aparência, personalidade, história, capacidades ou recursos apenas para completar visualmente a ficha.

Se o jogador delegar explicitamente a criação, uma proposta pode ser construída, mas continua sujeita à revisão normal quando for apresentável ao jogador.

## Conversão mecânica

Quando o conceito estiver suficientemente claro:

1. reconstruir as capacidades do personagem em linguagem natural;
2. identificar o que é atributo natural;
3. identificar perícias reais;
4. identificar poderes e repertórios;
5. identificar TRAÇOS qualitativos;
6. identificar RECURSOS recorrentes importantes;
7. identificar relações recorrentes que realmente pertencem à ficha;
8. converter para a sintaxe do sistema;
9. aplicar `calibracao.md`;
10. normalizar a ficha sem acrescentar conteúdo inexistente.

Todos os personagens usam as mesmas mecânicas e as mesmas escalas. NPC não possui sistema próprio de atributos, perícias, poderes, traços, relações ou recursos.

## Ordem das fichas na criação de campanha

A ordem canônica da revisão mecânica inicial pertence a `../criacao/README.md`:

```text
personagens JOGADOR IA
→ personagens JOGADOR IA EVENTUAL
→ protagonista
```

O protagonista é revisado por último para evitar que sua ficha sirva como régua inconsciente para calibrar as demais.

NPCs comuns não entram nessa sequência apenas por estarem visíveis ou serem relevantes na ficção.

Cada personagem continua sendo calibrado isoladamente conforme `calibracao.md`.

> **A ordem protege o processo. Ela não cria balanceamento entre fichas.**

## Revisão mecânica da campanha

Quando este arquivo for usado dentro da criação de campanha, seguir os **cinco blocos canônicos** definidos em `../criacao/README.md`:

```text
1 - Identidade e conceito
2 - Atributos e perícias
3 - Poderes e capacidades
4 - Traços e relações
5 - Conferência final
```

### Bloco 1 — Identidade e conceito

Revisar identidade, origem, aparência, personalidade, comportamento, história essencial e papel narrativo quando aplicáveis.

O dado persistente de autoridade é `CONTROLE`. `GERÊNCIA` pode existir como linguagem de escolha durante a criação, mas não cria campo permanente separado.

### Bloco 2 — Atributos e perícias

Converter e revisar o conceito em:

```text
FIS | RES | MEN | VON
```

e nas perícias realmente relevantes.

### Bloco 3 — Poderes e capacidades

Converter e revisar poderes, equipamentos tratados como Poder quando aplicável, capacidades relevantes e limites conceituais segundo as regras do sistema.

### Bloco 4 — Traços e relações

Revisar TRAÇOS, fraquezas, características especiais e relações iniciais que realmente pertençam à ficha.

### Bloco 5 — Conferência final

Verificar se o conjunto representa o conceito aprovado, corrigir incoerências, remover excessos e somente então considerar a ficha pronta para aprovação final.

## Salvamento durante a revisão

Dentro da criação de campanha, cada bloco aprovado é persistido imediatamente antes de avançar.

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

Isso inclui:

```text
CONTROLE: JOGADOR HUMANO
CONTROLE: JOGADOR IA
CONTROLE: JOGADOR IA EVENTUAL
```

Vários personagens `JOGADOR IA EVENTUAL` podem compartilhar a mesma persona operacional, mas cada um continua sendo uma peça distinta e possui seu próprio arquivo.

NPCs comuns não pertencem por padrão a `personagens/`.

Um NPC simples pode existir apenas durante a cena. Quando um NPC precisa de persistência reservada para continuidade, sua ficha ou material operacional pertence a:

```text
campanhas/<nome>/mestre/
```

Quando houver volume suficiente, pode existir:

```text
campanhas/<nome>/mestre/npcs/
```

Não usar `mundo/npcs/` como destino padrão. `mundo/` guarda verdades estáveis do cenário; `mestre/` guarda NPCs e material reservado de condução.

## Personagens conhecidos

Para personagem canônico, conhecido ou licenciado:

1. o jogador escolhe a versão-base quando essa escolha for necessária;
2. o jogador pode alterar, combinar ou substituir elementos dessa versão;
3. a IA usa o cânone externo como referência de apoio, não como limite obrigatório;
4. quando a versão da campanha estiver suficientemente clara, consolidá-la;
5. a versão consolidada passa a ser a referência canônica local daquela campanha;
6. somente depois converter suas capacidades para a linguagem mecânica do sistema.

Se o jogador já tiver descrito uma combinação suficiente, não perguntar novamente qual versão usar.

> **A pergunta relevante é: “qual é a versão desta campanha?”**

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

Fichas reservadas podem usar estado canônico próprio quando uma aprovação aberta revelaria segredos.

## Progressão não é criação repetida

Concluir missão, capítulo ou arco não concede automaticamente:

- atributo novo;
- aumento de perícia;
- aumento de poder;
- nova capacidade.

A ficha só muda posteriormente quando a própria ficção muda de forma estável o personagem.

O procedimento de atualização pertence a `../persistencia/`.

> **Criação define a ficha inicial. Persistência acompanha mudanças reais posteriores.**
