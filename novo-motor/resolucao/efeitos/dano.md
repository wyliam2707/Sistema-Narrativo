# Dano

Dano produz perda de VIDA ou dano estrutural quando o mecanismo consegue afetar o alvo.

## Manifestação-base

A base depende da forma de entrega:

`corpo / arma corpo a corpo → Curto / 1 alvo / Pontual / Instantâneo`

`disparo / projeção → Médio / 1 alvo / Pontual / Instantâneo`

## Fonte do Dano

Usar a capacidade que realmente produz a agressão.

`golpe corporal → FIS`, quando esse for o mecanismo

`arma, Poder ou equipamento com Dano [X] → usa seu próprio Dano [X]`

Fontes não são somadas automaticamente.

`FIS [2] + Arma Dano [3] ≠ Dano [5]`

## Resolução

Quando técnica ofensiva e defensiva realmente participam da mesma troca:

`Perícia efetiva = Perícia ofensiva − Perícia defensiva`

Se não existir Perícia defensiva capaz de interferir naquele mecanismo, ela não entra.

`Ataque efetivo = Dano + 1 + (Perícia efetiva × 0,2)`

A Defesa efetiva é somente aquilo que realmente resiste ao mecanismo do ataque, como `RES`, `VON`, Barreira, equipamento ou outra proteção coerente. Não somar automaticamente várias defesas.

`Dano aplicado = 2^(Ataque efetivo − Defesa efetiva)`

Referência sem diferença de Perícia:

`Ataque = Defesa → 2` | `+1 → 4` | `+2 → 8` | `+3 → 16` | `+4 → 32` | `+5 → 64`

`-1 → 1` | `-2 → 0,5` | `-3 → 0,25`

### Dano mínimo

`0,25` é o menor Dano mecanicamente acumulável.

`Dano ≥ 0,25 → contabiliza`

`Dano < 0,25 → não contabiliza`

Isso não torna capaz um meio que, pela própria ficção, não consegue afetar o alvo.

## Fraqueza e Mortal

Quando um TRAÇO se aplicar à resistência natural contra aquele mecanismo:

`Fraqueza: X → resistência natural contra X pela metade, arredondando para baixo`

`Mortal: X → resistência natural contra X passa a [0]`

Proteções externas continuam sendo julgadas separadamente quando ainda forem válidas.

## VIDA e estrutura

Contra uma personagem, o Dano aplicado é acumulado contra sua VIDA.

`Dano acumulado ≥ VIDA → Incapacitada`

salvo consequência mais severa claramente determinada pela natureza e intensidade do acontecimento.

Contra uma manifestação ou estrutura com `D / V`, sua regra própria define a Defesa e o Dano estrutural reduz `V`.

## Persistência

Dano é instantâneo. Depois da aplicação permanece a consequência na VIDA ou na estrutura atingida, não um efeito persistente de Dano.

Ampliações de Alcance, Alvos ou Área usam `../consolidacao.md` e não dividem automaticamente a intensidade entre os afetados.

> **A cena escolhe a fonte e a defesa. Esta página resolve quanto Dano realmente atravessa.**