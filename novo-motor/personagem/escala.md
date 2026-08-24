# Escalas de Capacidade

Status: EM DESENVOLVIMENTO

Este arquivo registra apenas as escalas atualmente válidas para a construção do personagem.

## Atributos

Os Atributos usam:

```text
Corpo — POD [0–7] | HAB [0–7] | RES [0–7]
Mente — POD [0–7] | HAB [0–7] | RES [0–7]
```

Criação-base atual:

```text
12 pontos de Atributo
mínimo [0]
máximo [7]
```

A função do número depende do Atributo:

```text
POD → potência e intensidade
HAB → execução, precisão e controle
RES → resistência e sustentação
```

## Perícias

Perícias usam escala de `[0]` a `[5]`.

```text
[0] → sem bônus de treinamento relevante
[1] a [5] → graus crescentes de treinamento, domínio ou especialização
```

Perícia e Atributo não são a mesma coisa. A Perícia informa o campo de treinamento; o Atributo informa a capacidade usada na ação.

## Poderes

Poderes não usam uma escala universal de potência.

```text
Nome [X]
```

Nos Poderes ativos, `[X]` significa somente:

> máximo de Energia que pode ser investido naquele Poder em um único uso.

A potência, alcance, dano, número de alvos, duração e demais propriedades são definidos pelo arquivo do próprio Poder.

Exemplo:

```text
Teleporte [5]
```

não significa que Teleporte está em “grau 5”. Significa apenas que aquele personagem pode investir até 5 de Energia no Teleporte por uso.

## Passivos

Passivos também não usam uma escala universal.

Quando houver `[X]`, o próprio Passivo define o significado:

```text
RD [3] → reduz 3 de dano
Vida Extra [30] → +30 Vida
Proteção [2] → +2 Esquiva e +2 Percepção
Regeneração [2] → recupera 2 de Vida por hora
```

## Regra de leitura

Não comparar números de categorias diferentes como se fossem a mesma escala.

```text
Atributo [4]
Perícia [4]
Poder [4]
Passivo [4]
```

podem representar coisas completamente diferentes.

> **Atributos e Perícias possuem escalas próprias. Poderes e Passivos definem o significado do número em sua própria descrição.**
