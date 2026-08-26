# NPCs

Status: APROVADO

NPC não é uma categoria mecânica diferente.

Todos os personagens usam as mesmas regras de:

- Patamar;
- Atributos;
- Perícias;
- Poderes;
- Traços;
- Vida;
- Mana;
- relações e recursos.

A diferença está em **quem controla o personagem** e em **quanto vale a pena registrar para garantir continuidade**.

---

## CONTROLE: NPC

Um NPC possui:

```text
CONTROLE: NPC
```

Isso significa que ele não possui um jogador dedicado.

Quando sua presença exigir agência:

```text
ROTINA EVIDENTE
→ NARRADOR pode narrar como consequência já determinada

DECISÃO VOLUNTÁRIA RELEVANTE, NÃO ADVERSARIAL
→ JOGADOR IA EVENTUAL assume temporariamente a peça

OPOSIÇÃO ATIVA
→ NPC pode ser delegado ao OPOSITOR depois que o NARRADOR julgar sua disponibilidade
```

A assunção temporária não altera o `CONTROLE` da ficha.

Isso vale para civis, comerciantes, guardas, monstros, inimigos, aliados circunstanciais, antagonistas recorrentes e entidades muito poderosas.

> **NPC não pertence ao NARRADOR como jogador. Rotina pode ser narrada; vontade relevante precisa da cadeira apropriada.**

---

## OPOSITOR e delegação temporária

`OPOSITOR` não é uma categoria de `CONTROLE`.

O OPOSITOR pode propor problemas, pressões, interrupções e ações usando elementos legítimos da ficção. O NARRADOR julga se a proposta é plausível e coerente.

Quando apropriado, o NARRADOR pode delegar temporariamente um NPC ao OPOSITOR para executar aquela oposição.

A delegação operacional não altera a ficha.

---

## Importância e mecânica

NPCs podem ser `Centrais`, `Relevantes` ou `Figurantes` conforme sua função estrutural na campanha.

Importância não modifica automaticamente:

- Patamar;
- Atributos;
- Perícias;
- Poderes;
- Traços;
- Vida;
- Mana;
- chance de sucesso;
- Dificuldade do cenário.

Vida e Mana são calculadas pelas mesmas regras usadas por qualquer outro personagem.

> **Figurante não significa mecanicamente fraco. Central não significa mecanicamente mais resistente.**

---

## Ficha rápida

NPCs simples não usam modelos automáticos que preencham capacidades inexistentes.

Uma ficha rápida registra apenas aquilo que realmente precisa ser conhecido para o NPC funcionar.

Exemplo:

```text
Guarda
Importância: Figurante
CONTROLE: NPC
Patamar: [1]

ATR relevantes:
Controle [1]
Resistência [1]

PERÍCIAS:
- Sociedade

Vida Máxima [14]
Mana Máxima [18]
```

Esse exemplo é apenas estrutural. Os valores reais dependem da construção do personagem.

---

## Ficha mínima

Um NPC ainda mais simples pode possuir apenas:

```text
Nome
Conceito
Importância
CONTROLE
Patamar, quando necessário
capacidades realmente relevantes
Vida/Mana, apenas se forem acompanhadas
```

> **Informação ausente não significa valor zero.**

Se Potência não aparece na ficha mínima, isso não significa `Potência [0]`. Significa apenas que esse valor não precisou ser registrado ainda.

Quando uma capacidade omitida se tornar mecanicamente relevante, ela deve ser estabelecida de forma coerente com o Conceito, a calibração e o que já foi definido; nunca inventada retroativamente apenas para contrariar uma solução válida.

---

## Vida e Mana em fichas compactas

Quando Vida ou Mana precisarem ser acompanhadas, seus valores máximos podem aparecer diretamente na ficha rápida como resultados derivados.

A ficha compacta não precisa exibir todos os seis Atributos apenas para mostrar esses resultados, desde que a construção subjacente seja coerente com as regras do personagem.

```text
Vida Máxima [X]
Mana Máxima [Y]
```

Valores atuais pertencem ao STATUS.

---

## Perícias em NPCs

Perícias não possuem graduação numérica.

Exemplo:

```text
PERÍCIAS:
- Crime
- Investigar
```

Quando uma Perícia for realmente relevante, concede `+1d` conforme `pericias.md`.

Não criar `Soldado [+2]`, `Combate [+3]` ou qualquer outra graduação antiga.

Também não criar Perícia genérica de combate apenas para aumentar ataques.

---

## Poderes em NPCs

Poderes não usam escala genérica `[1]` a `[5]`.

A ficha registra quais partes do arsenal funcional o NPC realmente possui.

Exemplo conceitual:

```text
PODERES:
- Movimento
- Proteção
- Terror
```

Configuração, Dano, Efeito, custo, alcance e demais opções pertencem aos Hubs e regras dos próprios Poderes.

---

## NPCs poderosos

Poder narrativo ou mecânico não exige uma ficha maior.

Um NPC extremamente poderoso pode possuir uma ficha operacional curta, desde que contenha tudo que precisa ser resolvido em jogo.

Exemplo estrutural:

```text
Entidade antiga
Importância: Relevante
CONTROLE: NPC
Patamar: [7]

ATR:
Potência [6] | Controle [4] | Resistência [7]
Intelecto [5] | Presença [7] | Vontade [7]

PERÍCIAS:
- Ocultismo
- Manipulação
- Sociedade

PODERES:
- Movimento
- Influência
- Proteção
- Invocação

RECURSOS:
- domínio próprio
- servos
- conhecimento antigo
```

A ficha curta não reduz a capacidade do personagem.

---

## Vitória não é poder bruto

Confrontos não precisam ser simétricos.

Um personagem pode vencer alguém superior em certas capacidades por meio de especialização, conhecimento, preparação, relação favorável entre capacidades, ambiente, recursos ou exploração correta de uma vulnerabilidade.

> **Capacidade de vencer não é a mesma coisa que poder bruto.**

Uma ficha não deve ser inflada apenas para garantir determinado resultado de confronto.

---

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

---

## Onde registrar NPCs persistentes

NPCs sem agência de jogador pertencem ao material de condução da campanha.

Destino padrão:

```text
campanhas/<nome>/mestre/
```

Quando houver vários NPCs persistentes:

```text
campanhas/<nome>/mestre/npcs/
```

Personagens com agência de jogador pertencem a:

```text
campanhas/<nome>/personagens/
```

`mundo/` guarda fatos estáveis do cenário e não é o destino padrão de fichas de NPC.

> **Personagem com agência → `personagens/`. NPC persistente → `mestre/`.**

---

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

Informações genuinamente reservadas podem permanecer em `mestre/` como material separado.

---

## Ganchos para o OPOSITOR

Uma ficha persistente de NPC pode preservar fatos capazes de gerar movimento futuro quando existirem de verdade na ficção.

Isso pode incluir:

- relações tensas;
- interesses conflitantes;
- obrigações;
- pactos;
- recursos vulneráveis;
- limitações;
- inimigos;
- desavenças não resolvidas.

Esses elementos não são acontecimentos pré-programados.

O OPOSITOR pode propor movimento a partir deles, mas não pode inventar retroativamente conhecimento, recursos, fraquezas ou preparações apenas para contrariar uma solução válida.

O NARRADOR continua julgando a proposta.

---

## Calibração

NPCs, antagonistas, aliados e protagonistas obedecem à mesma regra de `calibracao.md`:

> **cada personagem é construído pelo que ele é, nunca para equilibrar outra ficha por iniciativa do sistema.**

## Regra final

> **NPC usa as mesmas regras de qualquer personagem. O que muda é agência e quantidade de informação persistida. Ficha compacta omite o desnecessário; nunca transforma ausência de informação em valor zero.**
