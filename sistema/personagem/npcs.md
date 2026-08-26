# NPCs

Status: APROVADO

NPC não é uma categoria mecânica diferente.

> **NPC usa as mesmas regras de personagem; o que muda é quanto precisa ser representado na ficha e como sua agência é atribuída por outras áreas.**

## Mesma mecânica

NPCs usam normalmente:

- Patamar;
- Atributos;
- Perícias;
- Poderes;
- Traços;
- Vida;
- Mana;
- relações e recursos, quando relevantes.

Importância não modifica automaticamente nenhuma dessas capacidades.

```text
Figurante
≠ mecanicamente fraco

Central
≠ mecanicamente mais resistente
```

A calibração inicial segue `../criacao/calibracao.md`: cada NPC é construído pelo que ele realmente é, não para equilibrar outra ficha.

## CONTROLE na ficha

Uma ficha de NPC pode registrar:

```text
CONTROLE: NPC
```

Este arquivo apenas registra o campo.

Quem joga o NPC, quando existe delegação e como decisões voluntárias são atribuídas pertencem a:

```text
../personas/npcs-e-delegacao.md
```

Continuidade fora de cena pertence a:

```text
../agencia/continuidade-de-npcs.md
```

## Ficha completa, rápida ou mínima

NPC usa o nível de detalhe necessário para funcionar e permanecer coerente.

### Ficha completa

Pode usar o mesmo modelo de `ficha.md` quando todas as informações forem relevantes.

### Ficha rápida

Registra somente capacidades que precisam ser consultadas com frequência.

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

Vida Máxima [resultado derivado, se necessário]
Mana Máxima [resultado derivado, se necessário]
```

### Ficha mínima

Pode conter apenas:

```text
Nome
Conceito
Importância
CONTROLE
Patamar, se necessário
capacidades realmente relevantes
Vida/Mana, se forem acompanhadas
```

> **Informação omitida não significa valor zero.**

Se Potência não aparece, isso não estabelece `Potência [0]`; significa apenas que o valor não precisou ser registrado ainda.

Quando um valor omitido se tornar necessário, ele deve ser estabelecido de forma coerente com Conceito, Patamar, calibração e fatos já definidos — nunca retroativamente para contrariar uma solução válida.

## Vida e Mana

Quando forem acompanhadas, Vida e Mana seguem as mesmas fórmulas de qualquer personagem:

```text
Vida → ../resolucao/vida.md
Mana → ../resolucao/mana.md
```

A ficha pode registrar os máximos. Valores atuais pertencem a `../persistencia/`.

## Perícias

Perícias de NPC não possuem graduação.

```text
PERÍCIAS:
- Crime
- Investigar
```

Quando relevante, a Perícia concede `+1d` conforme `pericias.md`.

Não criar `Soldado [+2]`, `Combate [+3]` ou Perícia genérica de combate apenas para aumentar ataques.

## Poderes

Poderes de NPC também não usam grau genérico `[1–5]`.

```text
PODERES:
- Movimento
- Proteção
- Terror
```

A ficha registra a posse; funcionamento e Hub pertencem a `../resolucao/poderes/`.

## NPC poderoso pode ter ficha curta

Quantidade de texto não mede poder.

Um NPC de Patamar alto pode possuir ficha compacta se ela contiver tudo que precisa ser resolvido.

Exemplo:

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
```

## Persistência e continuidade

Este arquivo não decide onde NPCs são salvos nem quando continuam sendo acompanhados.

Usar:

```text
onde salvar NPC persistente?
→ ../persistencia/material-reservado.md

quando continuar acompanhando fora de cena?
→ ../agencia/continuidade-de-npcs.md

ganchos que podem voltar a mover a história?
→ ../agencia/ganchos-do-opositor.md

quem joga ou recebe delegação da peça?
→ ../personas/npcs-e-delegacao.md
```

## Regra final

> **`personagem/npcs.md` define somente como representar mecanicamente NPCs. Autoridade pertence a `personas/`, continuidade a `agencia/` e armazenamento a `persistencia/`.**
