# Patamar

Status: APROVADO

O **Patamar** representa o grau geral de desenvolvimento mecânico do personagem.

Sua escala vai de:

> **[1] a [7]**

O Patamar não mede fama, importância narrativa ou dificuldade do mundo. Ele organiza limites e quantidades mecânicas do personagem.

A Dificuldade das ações continua pertencendo à situação concreta, conforme `../resolucao/`.

---

## 1. Patamar e [X]

Quando uma regra de Poder usar `[X]`, `[X]` representa o Patamar do personagem.

Em Poderes, `[X]` funciona como o limite máximo de Mana que pode ser gasto em um único uso, salvo regra específica que diga o contrário.

Exemplo:

```text
Patamar [3]
→ [X] = 3
→ até 3 Mana em um único uso de Poder
```

---

## 2. Pontos de Atributo na criação

Na criação:

> **Pontos de Atributo = Patamar × 4**

Esses pontos são distribuídos entre os seis Atributos:

```text
Potência
Controle
Resistência
Intelecto
Presença
Vontade
```

Atributos podem possuir valores negativos normalmente.

Cada ponto reduzido abaixo de `[0]` devolve 1 ponto para redistribuição.

Exemplo:

```text
Patamar [2]
→ 8 pontos de Atributo

Potência [-1]
→ devolve 1 ponto
→ a soma distribuída entre os demais Atributos aumenta em 1
```

A redistribuição altera onde os pontos estão, mas não cria pontos além da reserva total permitida pela regra.

---

## 3. Limite de Atributo na criação

O maior valor que um Atributo pode possuir durante a criação é:

> **Patamar + 2**, respeitando o máximo permanente absoluto `[7]`.

Referência:

```text
Patamar [1] → máximo [3]
Patamar [2] → máximo [4]
Patamar [3] → máximo [5]
Patamar [4] → máximo [6]
Patamar [5] → máximo [7]
Patamar [6] → máximo [7]
Patamar [7] → máximo [7]
```

Esse limite vale para criação. Outras regras de progressão permanente devem respeitar o máximo permanente geral `[7]`, salvo regra futura explicitamente aprovada que estabeleça outra exceção.

---

## 4. Perícias iniciais

A quantidade inicial de Perícias depende da função da personagem na campanha:

```text
personagem simples
→ 1 Perícia

personagem relevante
→ 2 Perícias

vilão ou personagem jogador
→ 3 Perícias
```

As Perícias escolhidas devem ser coerentes com Conceito, formação, experiência e função da personagem.

Perícias não possuem grau; sua presença relevante concede `+1d` conforme `pericias.md` e `../resolucao/`.

---

## 5. Traços positivos iniciais

Na criação:

> **Pontos de Traços positivos = Patamar + 1**

Exemplos:

```text
Patamar [1] → 2 pontos
Patamar [4] → 5 pontos
Patamar [7] → 8 pontos
```

A regra específica de valores e aquisição de Traços pertence a `tracos.md` e à futura migração mecânica da criação.

---

## 6. Poderes iniciais

Na criação:

> **Poderes iniciais = Patamar + 1**

Exemplos:

```text
Patamar [1] → 2 Poderes
Patamar [4] → 5 Poderes
Patamar [7] → 8 Poderes
```

Poderes não possuem uma escala genérica própria de `[1]` a `[5]`.

Cada Poder define seu funcionamento e é configurado por seu próprio Hub. O Patamar entra quando uma regra usar `[X]` ou quando a criação determinar quantidades e limites.

---

## 7. Pontos obtidos por Traços negativos

Vícios e Corrupções podem gerar pontos adicionais conforme seus valores negativos.

Cada ponto negativo pode ser convertido em **uma** destas opções:

- `+1` ponto de Traço positivo;
- `+1` Poder.

O mesmo ponto negativo nunca compra as duas coisas ao mesmo tempo.

Exemplo:

```text
Traços negativos somando [-3]
→ 3 pontos extras
→ podem ser distribuídos entre Traços positivos e Poderes
```

A distribuição deve respeitar o Conceito e as regras específicas de Traços.

---

## 8. Patamar não altera a realidade do cenário

Patamar não desloca a régua de Dificuldade.

```text
Patamar baixo
≠ mundo automaticamente fácil

Patamar alto
≠ mundo automaticamente difícil
```

Uma ação quase impossível pode ter Dificuldade alta mesmo em Patamar `[1]`, enquanto tarefas comuns continuam comuns em Patamar `[7]`.

> **Patamar descreve o desenvolvimento mecânico do personagem. Dificuldade descreve o problema concreto.**

---

## Regra final

> **Patamar organiza desenvolvimento, limites de criação, quantidade inicial de capacidades e o valor `[X]`. Ele não substitui Atributos, não gradua Perícias e não serve para balancear a dificuldade do mundo.**
