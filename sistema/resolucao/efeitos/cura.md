# Cura

Cura recupera VIDA quando a capacidade possui esse efeito.

## Manifestação-base

`Cura → Toque / 1 alvo / Pontual / Instantâneo`

## Resultado

Cura reduz o Dano acumulado do alvo.

Quando uma Perícia realmente governa a aplicação:

`Cura efetiva = Cura usada + 1 + (Perícia aplicável × 0,2)`

`Cura aplicada = máx(1, 2^(Cura efetiva − RES do alvo))`

A Cura aplicada reduz o Dano acumulado, nunca abaixo de zero.

Uma aplicação capaz de recuperar Dano usa pelo menos patamar `[1]`.

Uma Cura muito abaixo da `RES` ainda recupera no mínimo `1` ponto por aplicação bem-sucedida.

## Ampliação e custo

Alcance, Alvos, Área e demais dimensões seguem `../consolidacao.md`.

Ampliação não reduz a Cura efetiva e não divide automaticamente o valor recuperado entre vários alvos.

Quando o uso consome Energia:

`Custo = patamar efetivamente usado + Ampliação usada`

O custo é pago antes da resolução.

## Persistência

Cura é instantânea.

Depois da aplicação permanece apenas a redução do Dano acumulado; não existe um efeito persistente de Cura apenas para representar VIDA já recuperada.

> **Dano acumula ferimento. Cura remove esse acúmulo pela mesma lógica de diferença de patamar.**
