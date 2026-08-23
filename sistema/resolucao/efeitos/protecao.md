# Proteção — Barreira

Barreira cria uma camada independente que recebe o ataque antes do alvo protegido.

## Manifestação-base

`Proteção/Barreira → Si mesmo / 1 alvo / Pontual / Cena`

## Estrutura

`Barreira [D / V]`

`D = nível da Proteção usado + (Perícia aplicável × 0,2)`

`V = maior entre [1] e o Atributo estrutural da Fonte`

Cada Fonte mantém uma única Barreira ativa; uma nova Barreira da mesma Fonte substitui a anterior. Barreiras de Fontes diferentes coexistem como camadas separadas.

## Ataque contra Barreira

O ataque resolve contra `D` da Barreira e o Dano reduz primeiro sua Vida.

Se o Dano não superar a Vida restante, o ataque termina na Barreira.

Se superar:

`Excedente = Dano aplicado − Vida restante da Barreira`

`Ataque efetivo restante = D da Barreira + log₂(Excedente)`

Arredondar o Ataque efetivo restante para baixo antes de atingir a próxima camada ou alvo.

Persistência geral usa `README.md`; Fonte usa `../fonte-e-vida-estrutural.md`; Ampliação usa `../consolidacao.md`.
