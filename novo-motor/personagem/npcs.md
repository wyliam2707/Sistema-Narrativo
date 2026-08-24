# NPCs

Status: EM DESENVOLVIMENTO

NPC não é uma categoria mecânica diferente. Quando precisar de ficha, usa a mesma estrutura de qualquer personagem:

```text
Atributos
+ Perícias
+ Poderes
+ Passivos
= Valores Derivados
```

A diferença está em quem controla a peça e em quanto vale a pena registrar para garantir continuidade.

## Controle

Um NPC pode ser identificado como:

```text
Controle: NPC
```

Isso não altera seus números nem concede regras especiais.

## Ficha rápida

NPCs simples registram somente aquilo que realmente precisa ser conhecido para funcionar na cena.

Exemplo:

```text
Guarda
Controle: NPC

Atributos
Corpo — POD [1] | HAB [1] | RES [1]
Mente — POD [0] | HAB [1] | RES [1]

Perícias
Sociedade [1]

Poderes
Golpe [1]
Disparo [1]

Passivos
—

Derivados
[preencher somente valores já definidos pelas regras atuais]
```

Não criar automaticamente Poderes, Passivos ou valores apenas para completar a ficha.

## NPCs extraordinários

Um NPC poderoso continua usando os mesmos quatro blocos mecânicos.

```text
Atributos
Perícias
Poderes
Passivos
```

Ele pode possuir valores maiores, mais Poderes, limites `[X]` diferentes ou Passivos incomuns quando o conceito justificar.

## Sem Arsenal próprio

NPCs também não usam uma camada mecânica separada de Arsenal.

Uma espada, arma de fogo, garra, raio, armadura ou campo de força deve ser representado pela mesma linguagem de Poderes e Passivos usada para qualquer personagem.

## Importância narrativa

Categorias narrativas como protagonista, relevante ou figurante não modificam automaticamente Atributos, Perícias, Poderes, Passivos ou Valores Derivados.

Se uma diferença mecânica for necessária, ela deve aparecer explicitamente na ficha.

## Estado atual

Vida atual, Energia atual, condições e efeitos temporários continuam separados da ficha-base.

```text
Ficha
Vida [máxima] | Energia [máxima]

Estado atual
Vida [atual/máxima] | Energia [atual/máxima] | condições
```

> **NPC usa o mesmo motor. A ficha pode ser mais curta, mas a linguagem mecânica não muda.**
