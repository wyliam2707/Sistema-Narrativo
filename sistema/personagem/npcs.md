# NPCs

Status: APROVADO

NPC não é uma categoria mecânica diferente. Todos os personagens usam as mesmas regras, escalas e estruturas de `ATRIBUTOS`, `PERÍCIAS`, `PODERES`, `TRAÇOS`, `RELAÇÕES` e `RECURSOS`.

A diferença está em **quem controla o personagem** e em **quanto vale a pena registrar para garantir continuidade**.

## Controle normal

Um NPC possui:

```text
CONTROLE: NPC
```

Sua autoridade normal pertence ao `NARRADOR`.

Isso vale para:

- civis;
- comerciantes;
- guardas;
- monstros;
- inimigos;
- aliados circunstanciais;
- antagonistas recorrentes;
- entidades muito poderosas.

Um NPC pode ser mais poderoso, mais antigo ou mais importante que um personagem Central e ainda continuar sendo NPC.

## OPOSITOR e delegação temporária

`OPOSITOR` não é uma categoria de `CONTROLE`.

O OPOSITOR pode propor problemas, pressões, interrupções e ações hostis usando elementos legítimos da ficção. O `NARRADOR` julga se a proposta é plausível e coerente.

Quando apropriado, o NARRADOR pode delegar temporariamente um NPC ao OPOSITOR para executar aquela oposição.

Exemplo:

```text
Assassino de Trigon
Importância: Figurante
CONTROLE: NPC
```

O NARRADOR pode aprovar a entrada do assassino na cena e entregá-lo temporariamente ao OPOSITOR durante o confronto.

Isso não altera a ficha. O personagem continua `CONTROLE: NPC`.

## Importância não cria mecânica própria

NPCs podem ser `Relevantes` ou `Figurantes` conforme sua função estrutural na campanha.

A importância não modifica atributos, perícias, poderes, resistência, chance de sucesso ou qualquer outra regra mecânica.

Ela também não determina o tamanho da ficha.

Um Figurante pode ter uma ficha extensa se isso for útil. Um Relevante pode ter poucas linhas se isso for suficiente.

A quantidade de aparições, sozinha, não muda a importância de um NPC.

## Ficha rápida

NPCs simples não usam modelos especiais como `Humano [1]`, `Demônio [3]` ou qualquer regra que preencha automaticamente todos os atributos.

Uma ficha rápida registra apenas o que realmente precisa ser conhecido para aquele NPC funcionar.

Exemplo:

```text
Guarda
Importância: Figurante
CONTROLE: NPC

PER:
Soldado [+1]

PODERES:
Arsenal [1] => Dano
```

Tudo que não precisa ser destacado pode permanecer sem registro específico.

Se o personagem possuir uma capacidade excepcional, ela é registrada normalmente pelas mesmas regras usadas por qualquer outro personagem:

```text
Guarda
Importância: Figurante
CONTROLE: NPC

ATR:
RES [1]

PER:
Soldado [+1]

PODERES:
Arsenal [1] => Dano
```

## NPCs poderosos

Poder narrativo ou mecânico não exige uma ficha maior.

Um NPC extremamente poderoso pode possuir uma ficha operacional curta, desde que ela contenha tudo que precisa ser resolvido em jogo.

Exemplo conceitual:

```text
Trigon
Importância: Relevante
CONTROLE: NPC

TRAÇOS:
- Entidade demoníaca extraplanar.
- Senhor de domínio demoníaco próprio.

ATR:
FOR [4] | AGI [2] | RES [4] | MEN [4] | VON [5]

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

A ficha curta não reduz o poder do personagem. Ela apenas evita registrar informação que não é necessária para operação ou continuidade.

## Vitória não é poder bruto

Todos os personagens usam as mesmas escalas, mas isso não significa que confrontos sejam simétricos.

Um personagem pode vencer alguém muito superior em força, resistência ou potência geral por meio de percepção, perícia, especialização, preparação, relações, recursos ou exploração correta de uma vulnerabilidade.

> **Capacidade de vencer não é a mesma coisa que poder bruto.**

Um personagem especializado não precisa receber atributos maiores apenas para enfrentar um adversário mais poderoso.

## Persistência

Um NPC simples pode existir somente durante a cena e nunca receber arquivo persistente.

Criar um registro persistente quando houver informação que valha a pena preservar entre cenas, por exemplo:

- relações recorrentes;
- desavenças;
- promessas e pactos;
- objetivos próprios;
- conhecimento relevante;
- recursos estabelecidos;
- limitações;
- consequências ainda ativas;
- mudanças que possam afetar decisões futuras.

Ter um arquivo persistente não altera `Importância` nem `CONTROLE`.

## Onde registrar NPCs persistentes

NPCs persistentes pertencem ao **mundo da campanha**, não à pasta de personagens jogáveis.

Estrutura recomendada:

```text
aventuras/<campanha>/
├── personagens/
│   ├── Personagem do Jogador.md
│   └── Personagem da IA.md
│
└── mundo/
    ├── README.md
    ├── cenario.md
    └── npcs/
        ├── Trigon.md
        └── Outro NPC.md
```

`personagens/` fica reservado aos personagens efetivamente jogáveis sob `JOGADOR HUMANO` ou `JOGADOR IA`.

`mundo/npcs/` guarda NPCs que precisam de continuidade própria dentro da campanha.

## Ganchos para o OPOSITOR

Uma ficha persistente de NPC deve preservar fatos que possam gerar pressão futura quando existirem de verdade na ficção.

Isso pode incluir:

- relações tensas;
- interesses conflitantes;
- obrigações;
- pactos;
- recursos vulneráveis;
- limitações;
- inimigos;
- desavenças ainda não resolvidas.

Esses elementos não são acontecimentos pré-programados. São apenas fatos disponíveis para o OPOSITOR explorar quando fizer sentido.

O OPOSITOR pode propor uma complicação a partir deles, mas não pode inventar conhecimento, recursos, fraquezas ou preparações que o personagem não possua.

O NARRADOR continua julgando a validade da proposta.

## Calibração

NPCs, antagonistas, aliados e protagonistas obedecem à mesma regra de `calibracao.md`:

> **cada personagem é construído pelo que ele é, nunca para equilibrar outra ficha.**
