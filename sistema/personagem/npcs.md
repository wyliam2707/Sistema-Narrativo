# NPCs

Status: APROVADO

NPC não é uma categoria mecânica diferente. Todos os personagens usam as mesmas regras, escalas e estruturas de `ATRIBUTOS`, `PERÍCIAS`, `PODERES`, `TRAÇOS`, `RELAÇÕES`, `RECURSOS`, `VIDA` e `ENERGIA`.

A diferença está em **quem controla o personagem** e em **quanto vale a pena registrar para garantir continuidade**.

## CONTROLE: NPC

Um NPC possui:

```text
CONTROLE: NPC
```

Isso significa que ele não possui um jogador dedicado.

Quando sua presença exigir agência:

```text
ROTINA EVIDENTE
→ NARRADOR pode narrar como consequência já determinada.

DECISÃO VOLUNTÁRIA RELEVANTE, NÃO ADVERSARIAL
→ JOGADOR IA EVENTUAL assume temporariamente a peça.

OPOSIÇÃO ATIVA
→ NPC pode ser delegado ao OPOSITOR depois que o NARRADOR julgar sua disponibilidade.
```

A assunção temporária não altera o `CONTROLE` da ficha. O personagem continua `CONTROLE: NPC`.

Isso vale para civis, comerciantes, guardas, monstros, inimigos, aliados circunstanciais, antagonistas recorrentes e entidades muito poderosas.

Um NPC pode ser mais poderoso, mais antigo ou mais importante que um personagem Central e ainda continuar sendo NPC.

> **NPC não pertence ao NARRADOR como jogador. Rotina pode ser narrada; vontade relevante precisa de uma cadeira.**

## OPOSITOR e delegação temporária

`OPOSITOR` não é uma categoria de `CONTROLE`.

O OPOSITOR pode propor problemas, pressões, interrupções e ações usando elementos legítimos da ficção. O `NARRADOR` julga se a proposta é plausível e coerente.

Quando apropriado, o NARRADOR pode delegar temporariamente um NPC ao OPOSITOR para executar aquela oposição ou movimento do cenário.

Exemplo:

```text
Assassino de Trigon
Importância: Figurante
CONTROLE: NPC
```

A delegação operacional não altera a ficha. O personagem continua `CONTROLE: NPC`.

## Importância e mecânica

NPCs podem ser `Relevantes` ou `Figurantes` conforme sua função estrutural na campanha.

A importância não modifica automaticamente atributos, perícias, poderes, resistência, chance de sucesso ou potência.

Ela também não determina o tamanho da ficha.

A `VIDA` é a exceção em que a função narrativa pode orientar diretamente a duração esperada de uma peça em confronto. Isso não significa que a categoria calcule a VIDA por fórmula: o valor final continua sendo escolhido e registrado explicitamente.

Assim, um Figurante pode possuir `RES [4]` e ainda ter `VIDA [5]`. Ele continua muito difícil de ferir, mas quando um ataque capaz realmente o atinge não precisa sustentar a duração de um protagonista.

Da mesma forma, uma entidade central ou chefe excepcional pode possuir `VIDA [50]` ou mais quando sua durabilidade em cena justificar isso.

Um Figurante pode ter uma ficha extensa se isso for útil. Um Relevante pode ter poucas linhas se isso for suficiente.

## Ficha rápida

NPCs simples não usam modelos automáticos que preencham capacidades inexistentes.

Uma ficha rápida registra apenas o que realmente precisa ser conhecido para aquele NPC funcionar.

Exemplo:

```text
Guarda
Importância: Figurante
CONTROLE: NPC

VIDA [5]

PER:
Soldado [+1]

PODERES:
Arsenal [1] => Dano
```

Se possuir capacidade excepcional, ela é registrada normalmente pelas mesmas regras usadas por qualquer outro personagem.

Exemplo:

```text
Monstro de guarda
Importância: Figurante
CONTROLE: NPC

ATR:
RES [4]

VIDA [5]

PODERES:
Força monstruosa [3] => Dano / Movimento
```

`RES [4]` não transforma automaticamente esse monstro em um chefe. Ataques fracos terão enorme dificuldade para produzir Dano relevante, mas a criatura é incapacitada quando seu Dano acumulado alcança sua `VIDA [5]`, salvo consequência mais severa exigida pela própria ficção.

## NPCs poderosos

Poder narrativo ou mecânico não exige uma ficha maior.

Um NPC extremamente poderoso pode possuir uma ficha operacional curta, desde que ela contenha tudo que precisa ser resolvido em jogo.

Exemplo conceitual:

```text
Trigon
Importância: Relevante
CONTROLE: NPC

VIDA [50]

TRAÇOS:
- Entidade demoníaca extraplanar.
- Senhor de domínio demoníaco próprio.

ATR:
FIS [4] | RES [4] | MEN [4] | VON [5]

PER:
Demonologia [+4]
Manipulação [+4]

PODERES:
Poder Demoníaco [5] => Geral / Dano / Proteção / Movimento / Manifestação / Influência
Magia [4] => Geral / Portal / Invocação / Contenção
Domínio [4] => Geral

RECURSOS:
Domínio de Trigon => exércitos demoníacos, servos, fortalezas, conhecimento antigo
```

A ficha curta não reduz o poder do personagem. Ela apenas evita registrar informação desnecessária.

## Vitória não é poder bruto

Todos os personagens usam as mesmas escalas, mas isso não significa que confrontos sejam simétricos.

Um personagem pode vencer alguém muito superior em capacidade física, resistência ou potência geral por meio de percepção, perícia, especialização, preparação, relações, recursos ou exploração correta de uma vulnerabilidade.

> **Capacidade de vencer não é a mesma coisa que poder bruto.**

Um personagem especializado não precisa receber atributos maiores apenas para enfrentar um adversário mais poderoso.

## Persistência

Um NPC simples pode existir somente durante a cena e nunca receber arquivo persistente.

Criar registro persistente quando houver informação que realmente precise sobreviver entre cenas, por exemplo:

- relações recorrentes;
- desavenças;
- promessas e pactos;
- objetivos próprios;
- conhecimento relevante;
- recursos estabelecidos;
- limitações;
- consequências ainda ativas;
- mudanças que possam afetar decisões futuras.

Ter arquivo persistente não altera `Importância` nem `CONTROLE`.

## Onde registrar NPCs persistentes

NPCs sem agência de jogador pertencem ao material de condução da campanha.

O destino atual é:

```text
campanhas/<nome>/mestre/
```

Quando houver vários NPCs persistentes e uma subdivisão realmente ajudar:

```text
campanhas/<nome>/mestre/npcs/
```

Exemplo:

```text
campanhas/<nome>/
├── personagens/
│   ├── protagonista.md
│   ├── ravena.md
│   └── dick-grayson.md
│
└── mestre/
    ├── README.md
    └── npcs/
        ├── trigon.md
        └── outro-npc.md
```

`personagens/` é reservado às peças com agência de jogador:

```text
JOGADOR HUMANO
JOGADOR IA
JOGADOR IA EVENTUAL
```

`mestre/` guarda NPCs persistentes, adversários e demais informações reservadas de condução.

`mundo/` guarda fatos estáveis do cenário e **não** é o destino padrão de fichas de NPC.

> **Personagem com agência → `personagens/`. NPC persistente → `mestre/`.**

## Mudança de CONTROLE

Se um NPC passar a receber formalmente:

```text
CONTROLE: JOGADOR IA EVENTUAL
```

então ele passa a ser uma peça com agência de jogador.

Sua ficha canônica deve ficar em:

```text
campanhas/<nome>/personagens/<personagem>.md
```

Não manter uma segunda ficha completa em `mestre/`.

Informações genuinamente reservadas que ainda não devam fazer parte da ficha aberta podem permanecer em `mestre/` como material separado.

## Ganchos para o OPOSITOR

Uma ficha persistente de NPC pode preservar fatos que possam gerar movimento futuro quando existirem de verdade na ficção.

Isso pode incluir:

- relações tensas;
- interesses conflitantes;
- obrigações;
- pactos;
- recursos vulneráveis;
- limitações;
- inimigos;
- desavenças ainda não resolvidas.

Esses elementos não são acontecimentos pré-programados. São fatos disponíveis quando houver causa, oportunidade e meios coerentes.

O OPOSITOR pode propor movimento a partir deles, mas não pode inventar retroativamente conhecimento, recursos, fraquezas ou preparações para contrariar uma solução válida.

O NARRADOR continua julgando a proposta.

## Calibração

NPCs, antagonistas, aliados e protagonistas obedecem à mesma regra de `calibracao.md`:

> **cada personagem é construído pelo que ele é, nunca para equilibrar outra ficha.**

A VIDA pode ser escolhida de acordo com a durabilidade que aquela peça precisa sustentar na história sem alterar seus demais patamares mecânicos.