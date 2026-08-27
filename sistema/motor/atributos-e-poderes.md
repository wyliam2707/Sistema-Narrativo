# Atributos e Poderes

Status: RASCUNHO / NÃO IMPLEMENTADO

Este documento registra uma possibilidade para separar a competência comum da personagem da potência e resolução de seus Poderes.

## Atributos como valores-base

A personagem possui seis Atributos fundamentais:

```text
FOR [x]
DES [x]
VIG [x]
INT [x]
SAB [x]
CAR [x]
```

A proposta atual é que esses Atributos sejam usados como **valores-base de construção e derivação**, mas não sejam rolados diretamente em testes.

Em jogo não existe, por princípio:

```text
1d20 + FOR
1d20 + DES
1d20 + INT
```

O Atributo alimenta outros números já definidos na ficha.

Exemplos em estudo:

```text
Atributo + treinamento
→ valor final de uma Perícia

VIG + Patamar
→ Vida

DES
→ base de Defesa e/ou Reflexos

Atributos mentais
→ base de resistências ou efeitos apropriados

Atributo indicado pelo Poder
→ acerto, dano, cura, proteção ou outro efeito descrito pelo próprio Poder
```

Assim, o Atributo continua sendo estrutural para a personagem sem virar uma escolha de resolução durante a sessão.

## Ideia central dos Poderes

Os Poderes não precisam usar um atributo universal de "Poder".

Cada Poder já define, em sua própria descrição, qual Atributo participa de sua resolução e de quais partes do efeito ele participa.

Exemplos conceituais:

```text
magia ofensiva
→ pode usar INT para acerto e/ou dano

cura e proteção
→ pode usar SAB para intensidade, cura ou proteção

efeito mental/social sobrenatural
→ pode usar CAR para acerto, intensidade ou efeito
```

Essas associações são exemplos de construção, não uma obrigação universal. Um Poder específico pode usar outro Atributo quando sua natureza justificar.

## Poder como regra fechada

O Poder pronto deve informar diretamente:

```text
Nome
Atributo utilizado
como o Atributo entra na resolução
Alcance
Alvo
Dano ou Efeito
Resistência aplicável
Custo
outras propriedades necessárias
```

Exemplo conceitual:

```text
Bola de Fogo
Atributo: INT
Acerto: 1d20 + INT
Dano: 3d6 + INT
Resistência: Reflexos
```

Outro exemplo:

```text
Cura
Atributo: SAB
Cura: 3d6 + SAB
Alcance: Toque
```

Outro exemplo:

```text
Influência Mental
Atributo: CAR
Acerto/Efeito: definido pelo Poder
Resistência: Vontade
```

## Separação conceitual

```text
ATRIBUTOS
→ valores fundamentais
→ alimentam números derivados
→ não são rolados diretamente

PERÍCIAS
→ competência comum
→ valor final já calculado na ficha
→ 1d20 + Perícia

PODERES
→ capacidade extraordinária ou de confronto
→ cada Poder informa qual Atributo utiliza
→ o Poder define sua própria fórmula

DEFESAS / RESISTÊNCIAS
→ valores derivados já calculados na ficha
→ usados como CD para ataques e efeitos
```

Isso permite que uma personagem possua atributos físicos baixos e ainda tenha um Poder extremamente destrutivo, sem obrigar a potência sobrenatural a representar a constituição física da personagem.

## Objetivo

Manter os seis Atributos como a fundação matemática da personagem sem obrigar o jogador a escolher ou testar Atributos diretamente durante a sessão.

> **O Atributo constrói a ficha; a ficha resolve o jogo.**

Esta proposta permanece em estudo e não altera as regras aprovadas.