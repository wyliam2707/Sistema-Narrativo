# Combate e dano

Status: APROVADO

Este arquivo define como uma aplicação ofensiva vira Dano quando o resultado não é evidente.

A ordem do combate pertence a `ordem-de-resolucao-do-combate.md` e `../operacao/turnos-de-combate.md`.

> **A cena determina quais valores participam. Esta regra calcula o Dano.**

## 1. Fonte do Dano

Usar a capacidade que realmente produz a agressão.

- golpe corporal → `FIS` quando esse for o mecanismo;
- arma, Poder ou equipamento com `Dano [X]` → usa seu próprio `Dano [X]`.

Fontes não são somadas automaticamente.

`FIS [2] + Arma Dano [3] ≠ Dano [5]`

## 2. Perícia efetiva

Quando técnica ofensiva e defensiva realmente participam da mesma troca:

`Perícia efetiva = Perícia ofensiva − Perícia defensiva`

Se não existir Perícia defensiva capaz de interferir naquele mecanismo, ela não entra no cálculo.

## 3. Ataque efetivo

`Ataque efetivo = Dano + 1 + (Perícia efetiva × 0,2)`

O valor existe somente para resolver aquela aplicação.

Ampliações de Alcance, Alvos, Área ou outra dimensão não alteram o Ataque efetivo; seguem `consolidacao.md`.

## 4. Defesa aplicável

A Defesa é aquilo que realmente resiste ao mecanismo do ataque.

Como referências comuns:

`RES` → integridade e resistência física.

`VON` → resistência mental, emocional ou volitiva.

Poderes, Barreiras, equipamentos ou outras proteções entram somente quando realmente respondem ao ataque, conforme suas regras próprias.

Não somar automaticamente várias defesas apenas porque coexistem.

> **A cena determina qual ataque e qual defesa realmente participam.**

## 5. Dano aplicado

`Dano aplicado = 2^(Ataque efetivo − Defesa efetiva)`

A diferença de patamar é exponencial: cada ponto dobra ou reduz pela metade o Dano.

Referência sem diferença de Perícia:

`Ataque = Defesa → 2` | `+1 → 4` | `+2 → 8` | `+3 → 16` | `+4 → 32` | `+5 → 64`

`-1 → 1` | `-2 → 0,5` | `-3 → 0,25`

### Dano mínimo

`0,25` é o menor Dano mecanicamente acumulável.

`Dano ≥ 0,25 → contabiliza`

`Dano < 0,25 → não contabiliza`

Isso não torna capaz um meio que, pela própria ficção, não consegue afetar o alvo.

## 6. Fraqueza e Mortal

Quando um TRAÇO se aplicar à resistência natural contra aquele mecanismo:

`Fraqueza: X → resistência natural contra X pela metade, arredondando para baixo`

`Mortal: X → resistência natural contra X passa a [0]`

Proteções externas continuam sendo julgadas separadamente quando ainda forem válidas.

## 7. VIDA e incapacidade

`VIDA [X]` determina quanto Dano acumulado a peça suporta antes de ficar Incapacitada.

`RES → quanto o ataque consegue afetar`

`VIDA → quanto Dano relevante pode ser acumulado`

VIDA não é derivada de RES e não possui valor universal.

Quando:

`Dano acumulado ≥ VIDA`

→ a peça fica `Incapacitada`, salvo consequência mais severa claramente determinada pela natureza e intensidade do acontecimento.

O valor de VIDA usado é sempre o registrado na ficha da peça.

## 8. Fluxo

```text
Fonte do Dano
→ Perícia efetiva, se aplicável
→ Ataque efetivo
→ Defesa aplicável
→ Dano aplicado
→ acumular em VIDA
→ interpretar a consequência
```

Custos e Ampliação são resolvidos antes da aplicação pelas regras correspondentes.

> **Use somente as partes necessárias para resolver a troca e continue a cena.**
