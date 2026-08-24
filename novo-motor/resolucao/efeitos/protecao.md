# Proteção — Barreira

Barreira cria uma camada independente que recebe o ataque antes do alvo protegido.

## Manifestação-base

`Proteção/Barreira → Si mesmo / 1 alvo / Pontual / Cena`

## Estrutura

`Barreira [D / V]`

`D = patamar da Proteção usado + (Perícia aplicável × 0,2)`

`V = maior entre [1] e o Atributo estrutural da Fonte`

Para identificar o Atributo estrutural, usar a natureza real da proteção:

`proteção física ou estrutural → RES`

`proteção mágica ou espiritual → VON`

Outra Fonte só usa outro Atributo quando a própria natureza da manifestação justificar isso. Não escolher o Atributo apenas por ser mais vantajoso.

O valor de `V` é fixado quando a Barreira é criada. Mudanças posteriores no Atributo da Fonte não recalculam aquela instância.

Cada Fonte mantém uma única Barreira ativa; uma nova Barreira da mesma Fonte substitui a anterior. Barreiras de Fontes diferentes coexistem como camadas separadas.

## Ataque contra Barreira

O ataque resolve contra `D` da Barreira e o Dano reduz primeiro sua Vida estrutural `V`.

Se o Dano não superar a Vida restante, o ataque termina na Barreira.

Se superar:

`Excedente = Dano aplicado − Vida restante da Barreira`

`Ataque efetivo restante = D da Barreira + log₂(Excedente)`

Arredondar o Ataque efetivo restante para baixo antes de atingir a próxima camada ou alvo.

## Persistência

Enquanto `V > 0`, a Barreira funciona integralmente. Ela termina quando sua Duração termina ou quando chega a `V0`, o que acontecer primeiro.

Vida estrutural não é recuperada por Cura, descanso ou regeneração de VIDA comum.

Se a Barreira depender continuamente de uma Fonte e essa Fonte deixar de existir, a Barreira termina. Se já for autônoma, continua segundo sua Duração e `V`.

Ampliações de Alcance, Alvos, Área/Tamanho ou Duração usam `../consolidacao.md`.