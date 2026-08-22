# Material Reservado do MESTRE / NARRADOR

Status: APROVADO

MESTRE e NARRADOR designam a mesma persona.

A pasta `mestre/` de uma campanha existe para guardar **informações que somente a persona MESTRE / NARRADOR deve consultar diretamente durante o jogo**.

Ela funciona como memória reservada de condução da campanha.

> **Ser reservado altera quem pode consultar a informação. Não altera se ela é ou não verdadeira.**

## Função de `mestre/`

A pasta pode guardar, quando realmente necessários:

- fichas e informações de NPCs controlados pelo MESTRE / NARRADOR;
- identidades ocultas;
- conhecimentos secretos de NPCs;
- objetivos e intenções ainda desconhecidos;
- armadilhas e preparações já colocadas no mundo;
- verdades ocultas do cenário;
- anotações específicas de continuidade;
- planos ainda não executados;
- possibilidades de condução ainda não transformadas em fato.

Estrutura possível:

```text
aventuras/<campanha>/
└── mestre/
    ├── README.md
    ├── notas.md
    ├── npcs/
    ├── segredos/
    └── preparacoes/
```

Essa estrutura é flexível. Pastas e arquivos só precisam existir quando houver conteúdo real que justifique sua existência.

## O que significa "somente o MESTRE sabe"

A existência de uma informação em `mestre/` não concede esse conhecimento automaticamente:

- ao JOGADOR HUMANO;
- ao JOGADOR IA;
- ao JOGADOR IA EVENTUAL;
- ao OPOSITOR;
- aos personagens da ficção.

Cada personagem continua sabendo apenas aquilo que plausivelmente aprendeu na história.

O MESTRE / NARRADOR decide quando uma informação reservada pode ser revelada, percebida, descoberta ou disponibilizada para outra persona conforme a ficção e as regras do sistema.

> **Conhecimento do MESTRE não é conhecimento dos personagens nem das outras personas.**

## Relação com o OPOSITOR

O OPOSITOR não possui uma base canônica própria.

Ele usa fatos, circunstâncias, NPCs, ameaças e limitações que já existam e que estejam disponíveis para sustentar oposição coerente.

O MESTRE / NARRADOR pode disponibilizar ao OPOSITOR apenas o que ele precisa para exercer oposição naquela situação.

O OPOSITOR não ganha automaticamente acesso a toda a pasta `mestre/` nem pode transformar uma anotação reservada em fato apenas porque isso aumentaria a dificuldade.

> **O MESTRE prepara a situação. O OPOSITOR explora a oposição possível dentro dela.**

## Trilha preparada não é roteiro obrigatório

O MESTRE / NARRADOR pode preparar uma trilha de problemas, lugares, agentes, recursos e acontecimentos possíveis.

Essa preparação não obriga os jogadores a seguir um caminho predeterminado.

Exemplo:

```text
PREPARADO:
- existe um culto;
- o culto usa um galpão;
- há três entradas conhecidas;
- o ritual está marcado para a meia-noite;
- existem guardas no acesso principal.
```

Os jogadores podem entrar pela frente, procurar outro acesso, investigar fornecedores, abandonar o local, negociar, pedir ajuda ou encontrar uma solução não prevista.

O MESTRE / NARRADOR responde à nova decisão usando a realidade já estabelecida.

> **O MESTRE prepara situações e caminhos possíveis, não resultados obrigatórios.**

## Estados de uma anotação reservada

Para evitar que ideia, intenção e fato sejam confundidos, material reservado deve deixar claro qual é sua natureza quando houver risco de ambiguidade.

### FATO

Já é verdade na campanha.

```text
FATO:
- Trigon conhece a localização do santuário.
```

Pode fundamentar decisões e resoluções enquanto continuar verdadeiro.

### CONHECIMENTO DE NPC

É algo que determinado NPC realmente sabe.

```text
CONHECIMENTO:
- Trigon sabe que Corvin procura o grimório.
```

Isso não concede o mesmo conhecimento a outros personagens.

### PREPARAÇÃO

Algo já foi colocado, organizado ou estabelecido no mundo antes de se tornar relevante para a ação atual.

```text
PREPARAÇÃO:
- duas câmeras cobrem a entrada principal do galpão.
```

A preparação já existe e pode ser descoberta, evitada, explorada ou neutralizada pelos jogadores.

### PLANO

É uma intenção de alguém dentro da ficção, mas ainda não foi executada.

```text
PLANO:
- Trigon pretende capturar Dick se surgir oportunidade.
```

O plano pode falhar, mudar, ser abandonado ou nunca encontrar oportunidade.

Ele não deve ser tratado como acontecimento consumado.

### POSSIBILIDADE

É uma ideia de condução do MESTRE / NARRADOR que ainda não constitui verdade da ficção.

```text
POSSIBILIDADE:
- Trigon pode tentar negociar com Ravena em algum momento.
```

Uma possibilidade não pode fundamentar retroativamente uma resolução como se já fosse fato.

## Preparado, planejado, proposto e acontecido

Durante o jogo, a distinção prática pode ser resumida assim:

```text
PREPARADO
→ algo já existe no cenário.

PLANEJADO
→ alguém pretende fazer, mas ainda não fez.

PROPOSTO
→ uma persona apresenta uma ação possível agora.

ACONTECIDO
→ a ação foi resolvida ou estabelecida e passou a fazer parte da história.
```

Somente o que realmente aconteceu entra no Livro como acontecimento.

## NPCs na pasta do MESTRE

NPCs cuja informação de condução não deva ficar disponível às outras personas podem permanecer em:

```text
mestre/npcs/
```

A ficha pode usar as mesmas regras gerais de personagem.

Pode conter, conforme necessário:

- capacidades;
- recursos;
- personalidade;
- objetivos;
- conhecimento atual;
- relações;
- segredos;
- preparação;
- outros fatos necessários para interpretá-lo e conduzi-lo de forma coerente.

Ser NPC do MESTRE não cria uma mecânica diferente nem autoriza capacidades retroativas.

O OPOSITOR pode receber temporariamente um NPC para exercer oposição, mas o NPC continua pertencendo à realidade administrada pelo MESTRE / NARRADOR.

## Relação com o Livro

Material reservado e Livro cumprem funções diferentes.

```text
MESTRE/
→ preserva o que o MESTRE precisa saber para conduzir a realidade ainda oculta ou operacional.

LIVRO
→ registra aquilo que efetivamente aconteceu na ficção.
```

Se Trigon apenas pretende montar uma armadilha, isso pode permanecer como PLANO em `mestre/`.

Se Trigon realmente monta a armadilha, o acontecimento entra no Livro, mesmo que os protagonistas ainda não saibam dela.

A armadilha ainda existente pode continuar registrada em material operacional reservado enquanto sua existência permanecer relevante.

> **O Livro registra o acontecimento. `mestre/` preserva a informação reservada necessária para continuar conduzindo suas consequências.**

## Relação com outras camadas

Material reservado não substitui a natureza normal do fato.

Uma verdade reservada pode também pertencer conceitualmente a uma camada específica:

```text
NPC
→ quem esse personagem é e o que sabe.

MUNDO
→ verdade sobre cenário, organização, lugar ou regra local.

STATUS
→ estado atual que precisa continuar verdadeiro.

PROGRESSÃO
→ consequência causal ainda viva.

LIVRO
→ acontecimento que efetivamente ocorreu.
```

`mestre/` determina principalmente **quem pode consultar diretamente aquela informação durante o jogo**.

Não é necessário duplicar o mesmo fato em vários arquivos apenas por estar reservado. Registrar onde ele for mais útil para continuidade, preservando sua natureza e visibilidade.

## Proibição de criação retroativa

A pasta `mestre/` não é uma caixa-preta que permite justificar qualquer coisa depois que o jogador já declarou uma solução.

Não se deve criar retroativamente:

- imunidade;
- poder;
- recurso;
- guarda;
- armadilha;
- conhecimento;
- passagem secreta;
- preparação;
- regra local;
- outro fato conveniente;

apenas para impedir uma ação válida, recuperar dificuldade ou proteger uma trama planejada.

Quando um fato oculto for usado como fundamento importante de uma resolução, ele precisa já existir de forma coerente antes de ser necessário para contrariar aquela ação.

> **Segredo pode estar oculto dos jogadores. Não pode nascer retroativamente apenas porque se tornou conveniente ao MESTRE ou ao OPOSITOR.**

## Princípio final

```text
MESTRE / NARRADOR
→ prepara e mantém a realidade reservada.

OPOSITOR
→ usa oposição que possua fundamento nessa realidade.

JOGADORES
→ escolhem como agir diante do que encontram.

LIVRO
→ registra o caminho que efetivamente aconteceu.
```

> **O MESTRE prepara o problema. O OPOSITOR explora o problema. Os JOGADORES decidem o que fazer com ele.**
