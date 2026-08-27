# Testes de Perícia com d20

Status: RASCUNHO / NÃO IMPLEMENTADO

## Ideia central

Os testes comuns usam diretamente o **valor final da Perícia já calculado na ficha**.

```text
1d20 + Perícia
```

O jogador não escolhe Atributo durante a resolução e não refaz a soma de Atributo + Perícia durante a sessão.

A relação entre Atributo e Perícia é resolvida antes, na criação ou evolução da personagem, e o resultado final fica impresso na ficha.

Exemplo:

```text
Esportes +6
Investigar +7
Medicina +5
Ocultismo +6
Ciência +8
```

Durante o jogo:

```text
atividade atlética
→ 1d20 + Esportes

investigar uma cena
→ 1d20 + Investigar

tratar um ferimento
→ 1d20 + Medicina

reconhecer conhecimento mágico
→ 1d20 + Ocultismo

analisar fenômeno científico
→ 1d20 + Ciência
```

## Ficha como interface

O objetivo é que a ficha física já entregue ao jogador todos os números necessários para resolver tarefas comuns.

```text
DECLARA A AÇÃO
→ identifica a Perícia correspondente
→ lê o valor final na ficha
→ rola 1d20 + esse valor
→ compara à Dificuldade
```

Não há escolha de Atributo em tempo de jogo para testes de Perícia.

## Atributos

Atributos podem continuar existindo como valores fundamentais da personagem e participar da criação dos valores finais das Perícias.

Uma possibilidade em estudo é:

```text
Atributo base + treinamento da Perícia
= valor final da Perícia na ficha
```

Exemplo conceitual:

```text
Atributo relacionado 2
Esportes 4
→ Esportes +6 na ficha
```

Depois de calculado, a ficha mostra apenas o valor que será usado na mesa.

## Eficiência

Uma única rolagem pode determinar sucesso e eficiência.

```text
resultado < Dificuldade
→ falha

resultado ≥ Dificuldade
→ sucesso

margem acima da Dificuldade
→ pode indicar qualidade, rapidez ou eficiência quando relevante
```

As faixas de eficiência ainda precisam ser definidas.

## Separação de Poderes e combate

Este motor é pensado para tarefas de competência: investigação, conhecimento, medicina, exploração, interação, atividades físicas e equivalentes.

A potência de Poderes extraordinários não precisa ser derivada dessas Perícias.

Uma personagem pode ser fisicamente frágil e ainda possuir um Poder de enorme escala. O Poder define sua própria capacidade de confronto.

## Objetivo de design

```text
uma Perícia
+ um valor final já impresso
+ 1d20
+ uma Dificuldade
= teste resolvido
```

> **A complexidade de construção fica fora da sessão; durante o jogo, a ficha apresenta diretamente o bônus utilizado.**

Este documento é somente uma proposta de motor e não altera regras aprovadas.
