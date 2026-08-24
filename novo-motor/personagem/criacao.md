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

Se uma resposta do jogador já fornecer uma delas de forma explícita, registrá-la e não perguntar novamente; seguir para o próximo campo ainda indefinido.

`IMPORTÂNCIA` e `CONTROLE` são independentes. As regras de cada campo pertencem a `ficha.md`.

## Método de criação assistida

A revisão de personagem usa como padrão uma mistura de **base pronta + liberdade total de adaptação antes do salvamento**.

O JOGADOR HUMANO não precisa construir cada campo do zero quando já existe material suficiente para uma proposta útil.

Durante cada bloco, o NARRADOR deve:

```text
consultar a base disponível
→ montar uma proposta coerente e suficientemente completa
→ apresentar a proposta ao jogador
→ receber correções, cortes, acréscimos ou mudanças
→ reapresentar quando necessário
→ salvar somente após aprovação explícita
```

A **base disponível** pode vir de:

- versão conhecida ou canônica escolhida para uma personagem licenciada;
- conceito e fatos já discutidos na campanha;
- blocos anteriores já aprovados;
- relações e decisões já estabelecidas;
- material original criado para aquela personagem.

A base serve para evitar uma criação vazia ou burocrática. Ela **não é uma prisão canônica**.

O jogador pode mudar antes da aprovação:

- idade;
- nome ou identidade;
- aparência e estilo;
- história;
- personalidade;
- relações;
- atributos e perícias;
- poderes e patamares;
- limitações;
- objetivos;
- qualquer outro elemento proposto.

Para personagem conhecido, o objetivo é começar de uma versão **reconhecível**, e então adaptá-la livremente ao cenário. Depois da aprovação, a versão consolidada na ficha passa a ser o cânone local da campanha.

Para personagem original, o NARRADOR usa o conceito e tudo que já foi aprovado como base para propor os próximos elementos em vez de obrigar o jogador a inventar cada campo isoladamente.

> **Proposta não é fato. Aprovação transforma a proposta em fato persistente.**

Uma correção pontual do jogador deve ser interpretada como alteração da proposta apresentada, **mantendo o restante igual**, salvo quando a própria correção exigir reorganização mais ampla.

Exemplo:

```text
NARRADOR:
Magia da Alma [4] => Geral / Dano [3] / Proteção [3] / Cura [2] / Projeção Astral [4]
Empatia [4] => ...

JOGADOR:
Mude Magia da Alma para [3], deixe Cura [2] e Projeção Astral [4] como únicas exceções e Empatia [2].

RESULTADO DA PROPOSTA:
Magia da Alma [3] => Geral / Dano / Proteção / Cura [2] / Projeção Astral [4]
Empatia [2] => ...
```

O que não foi pedido para mudar permanece como estava.

## Nascimento da ficha

Assim que `NOME + IMPORTÂNCIA + CONTROLE` estiverem definidos:

1. criar `personagens/<nome>.md`;
2. copiar o modelo-base completo de `ficha.md`;
3. usar `Status: PENDENTE DE REVISÃO`;
4. preencher somente Nome, Importância e CONTROLE;
5. deixar todos os demais campos e seções vazios.

Exemplo estrutural:

```text
# Ravena

Status: PENDENTE DE REVISÃO
Importância: Central
CONTROLE: JOGADOR IA

Nome real:
Idade:
Aparência:
Estilo:
Conceito:
Descrição:

TRAÇOS:

ATR: FIS [ ] | RES [ ] | MEN [ ] | VON [ ]
VIDA [ ] | ENERGIA [ ]
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

Não inventar ou **persistir antecipadamente** nome real, idade, aparência, estilo, origem, conceito, personalidade, comportamento, história, objetivos, medos, atributos, VIDA, ENERGIA, perícias, poderes, TRAÇOS, RECURSOS, relações, conhecimento ou qualquer outro conteúdo da ficha.

Essas informações podem ser **propostas** no bloco apropriado usando o método de criação assistida, mas só entram no arquivo depois da aprovação.

> **Primeiro identificamos a peça e sua autoridade. Depois descobrimos quem ela é.**

## Campo desconhecido fica vazio

Campos ainda não revisados permanecem vazios.

Nunca usar `[0]` ou `[+0]` para representar pendência. Zero é um valor mecânico real.

```text
ATR: FIS [ ] | RES [ ] | MEN [ ] | VON [ ]
VIDA [ ] | ENERGIA [ ]
```

significa ainda não definido.

```text
ATR: FIS [0] | RES [0] | MEN [0] | VON [0]
VIDA [35] | ENERGIA [10]
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

Em todos os blocos vale o mesmo ciclo:

```text
base disponível
→ proposta do NARRADOR
→ discussão e adaptação livre
→ aprovação do JOGADOR HUMANO
→ persistência
→ próximo bloco
```

### Bloco 1 — Identidade e conceito

Nome, Importância e CONTROLE já chegam definidos e não precisam ser redescobertos.

Este bloco deve deixar a personagem **identificável como pessoa e reconhecível em cena**, não apenas explicar sua origem de forma abstrata.

A revisão segue como padrão, quando aplicável:

```text
Nome de uso / codinome
→ Nome real
→ Idade
→ Aparência
→ Estilo
→ Origem / natureza
→ Conceito
→ demais informações de identidade necessárias
```

Revisar e preencher, quando relevantes:

- nome de uso, codinome ou identidade pela qual é conhecida;
- nome real, civil ou pessoal, quando diferente do nome de uso;
- outros nomes realmente usados;
- idade;
- aparência física suficiente para reconhecê-la;
- estilo visual e forma habitual de se apresentar;
- origem;
- natureza;
- conceito;
- demais elementos de identidade necessários para a interpretação.

`Nome real`, `Aparência` e `Estilo` fazem parte do **modelo-base padrão da ficha**. Permanecem vazios antes da revisão e são preenchidos no Bloco 1 quando aplicáveis.

A aparência não precisa virar catálogo de medidas. Deve registrar aquilo que realmente define a presença visual da personagem e ajuda o NARRADOR a descrevê-la de modo consistente.

`Aparência:` responde principalmente **como a pessoa é fisicamente reconhecida**.

`Estilo:` responde principalmente **como costuma se apresentar** — roupas, cores, acessórios, cabelo quando tratado como escolha estética, uniforme, armadura, maquiagem, símbolos ou outros elementos recorrentes.

`Descrição:` pode complementar esses campos com presença, impressão geral ou outra síntese útil, mas não substitui `Aparência` e `Estilo` quando ambos forem relevantes.

Se for personagem conhecido, canônico ou licenciado, a versão-base e eventuais combinações ou alterações são tratadas aqui, salvo quando o jogador já tiver fornecido essa informação.

A versão conhecida deve virar uma **proposta concreta local**, não um pedido para que o jogador recite o cânone campo por campo. O NARRADOR pode apresentar uma base reconhecível e o jogador modifica o que quiser antes de aprovar.

Depois de consolidada, a versão da campanha passa a ser a referência canônica local daquela personagem.

> **A pergunta relevante é: “quem é esta versão e como ela é reconhecida quando entra em cena?”**

### Bloco 2 — Atributos e perícias

Converter e revisar o conceito aprovado em:

```text
FIS | RES | MEN | VON
```

e nas perícias realmente relevantes.

O NARRADOR deve apresentar uma proposta calibrada, com justificativa quando útil, em vez de pedir ao jogador que escolha todos os números sem referência.

Aplicar `calibracao.md` sem usar outra ficha como molde automático.

Depois que os Atributos forem aprovados, preencher `VIDA` e `ENERGIA` na ficha para consulta rápida conforme `ficha.md` e as regras aplicáveis à personagem. Exceções específicas já aprovadas pertencem à própria personagem e não alteram automaticamente as demais fichas.

### Bloco 3 — Poderes e capacidades

Converter e revisar:

- poderes;
- equipamentos tratados como Poder quando aplicável;
- capacidades especiais;
- repertórios;
- limites conceituais relevantes.

O NARRADOR apresenta um arsenal coerente com a base aprovada. O jogador pode alterar nomes, patamares, repertórios, exceções e limites antes do salvamento.

Usar as regras atuais de `poderes.md`, `escala.md`, `calibracao.md` e `../resolucao/` quando necessário.

### Bloco 4 — Traços e relações

Revisar e preencher:

- TRAÇOS;
- fraquezas;
- características especiais qualitativas;
- RECURSOS recorrentes relevantes;
- relações que realmente pertençam à ficha.

Relações e fatos já discutidos anteriormente devem reaparecer automaticamente na proposta deste bloco. Não perguntar novamente se eles existem quando já foram explicitamente estabelecidos.

### Bloco 5 — Conferência final

Este bloco não é apenas uma inspeção mecânica.

Ele deve transformar tudo que já foi aprovado em uma personagem **completa para interpretação**.

O NARRADOR revisa a ficha inteira e, quando ainda houver campos narrativos vazios ou pouco desenvolvidos, apresenta uma proposta final misturando:

- a base original ou canônica escolhida;
- tudo que foi discutido durante a criação;
- os quatro blocos já aprovados;
- adaptações locais feitas pelo jogador;
- consequências naturais dessas escolhas para personalidade, objetivos, medos, conhecimento e história.

É especialmente apropriado completar e revisar aqui:

```text
Personalidade e tendências
Desejos / objetivos atuais
Medos / limites relevantes
Conhecimento atual relevante
História consolidada relevante
```

O jogador pode editar livremente essa síntese antes de aprovar.

O Bloco 5 também verifica incoerências, remove excessos e confirma que não restou campo importante esquecido apenas porque estava fora da conversa.

Campos comprovadamente inúteis para aquela personagem podem ser removidos somente depois dessa conferência.

> **O final da revisão combina a base reconhecível com tudo que a campanha transformou nela.**

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

Uma resposta que altera apenas parte da proposta não autoriza apagar ou simplificar silenciosamente o restante.

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

Concluir missão, capítulo ou arco não concede automaticamente atributo, períícia, poder ou capacidade nova.

A ficha só muda posteriormente quando a própria ficção muda de forma estável o personagem.

O procedimento de atualização pertence a `../persistencia/`.

> **Criação identifica a peça e constrói sua ficha inicial. Persistência acompanha mudanças reais posteriores.**