# Atributos e Poderes

Status: RASCUNHO / NÃO IMPLEMENTADO

Este documento registra uma possibilidade para separar a competência comum da personagem da potência e resolução de seus Poderes.

## Ideia central

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
PERÍCIAS
→ competência comum
→ valor final já calculado na ficha
→ 1d20 + Perícia

PODERES
→ capacidade extraordinária ou de confronto
→ cada Poder informa qual Atributo utiliza
→ o Poder define sua própria fórmula
```

Isso permite que uma personagem possua atributos físicos baixos e ainda tenha um Poder extremamente destrutivo, sem obrigar a potência sobrenatural a representar a constituição física da personagem.

## Objetivo

Evitar um atributo genérico de Poder quando o próprio conceito da habilidade já permite indicar a característica relevante.

> **O jogador não escolhe o Atributo durante o uso. O Poder já traz essa escolha registrada na ficha.**

Esta proposta permanece em estudo e não altera as regras aprovadas.