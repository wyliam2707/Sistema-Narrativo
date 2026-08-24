# Arsenal — Corpo a Corpo

Status: EM DESENVOLVIMENTO

Este arquivo reúne armas e formas de ataque usadas diretamente em combate físico próximo no `novo-motor/`.

Formato:

```text
Nome - Alcance - Dano - Crítico - Tipo - Pegada
```

Campos:

```text
Nome     → arma ou forma de ataque.
Alcance  → Toque ou, quando possível, também Arremesso.
Dano     → dano base da arma; `POD` nesta lista significa POD Corpo.
Crítico  → faixa de ameaça e multiplicador.
Tipo     → natureza principal do dano.
Pegada   → Livre, 1 mão ou 2 mãos.
```

`Livre` indica um ataque corporal que não exige uma mão específica nem ocupa pegada, podendo representar soco, chute, joelhada, cotovelada ou outro golpe semelhante.

Todo personagem possui automaticamente o ataque básico `Arte Marcial`.

## Lista

```text
Arte Marcial - Toque - 1d4 + POD - 20 x2 - Contusão - Livre

Corte — 1 mão
Espada curta - Toque - 1d6 + POD - 19-20 x2 - Corte - 1 mão
Espada longa - Toque - 1d8 + POD - 19-20 x2 - Corte - 1 mão
Machado de mão - Toque / Arremesso - 1d6 + POD - 20 x3 - Corte - 1 mão

Corte — 2 mãos
Espadão - Toque - 2d6 + POD - 19-20 x2 - Corte - 2 mãos
Machado grande - Toque - 1d12 + POD - 20 x3 - Corte - 2 mãos
Glaive - Toque - 1d10 + POD - 20 x3 - Corte - 2 mãos

Perfuração — 1 mão
Adaga - Toque / Arremesso - 1d4 + POD - 19-20 x2 - Perfuração - 1 mão
Rapieira - Toque - 1d6 + POD - 18-20 x2 - Perfuração - 1 mão
Picareta de guerra - Toque - 1d6 + POD - 20 x3 - Perfuração - 1 mão

Perfuração — 2 mãos
Lança - Toque / Arremesso - 1d8 + POD - 20 x3 - Perfuração - 2 mãos
Pique - Toque - 1d10 + POD - 20 x3 - Perfuração - 2 mãos
Lança pesada - Toque - 1d12 + POD - 20 x3 - Perfuração - 2 mãos

Impacto — 1 mão
Clava - Toque - 1d6 + POD - 20 x2 - Impacto - 1 mão
Maça - Toque - 1d8 + POD - 20 x2 - Impacto - 1 mão
Martelo de guerra - Toque - 1d8 + POD - 20 x3 - Impacto - 1 mão

Impacto — 2 mãos
Bastão - Toque - 1d8 + POD - 20 x2 - Impacto - 2 mãos
Malho - Toque - 1d10 + POD - 20 x3 - Impacto - 2 mãos
Martelo pesado - Toque - 1d12 + POD - 20 x3 - Impacto - 2 mãos
```

## Descrições

**Arte Marcial** — golpes corporais como socos, chutes, joelhadas e cotoveladas, disponíveis naturalmente a qualquer personagem.

**Espada curta** — lâmina compacta e ágil, apropriada para combate próximo com uma mão.

**Espada longa** — espada versátil de uma mão, equilibrando alcance, controle e poder de corte.

**Machado de mão** — machado compacto que pode ser usado no corpo a corpo ou lançado contra um alvo.

**Espadão** — grande espada empunhada com as duas mãos para produzir golpes de corte muito poderosos.

**Machado grande** — machado pesado de duas mãos, construído para concentrar grande força em cada golpe.

**Glaive** — arma de haste com lâmina na extremidade, combinando alcance físico e golpes amplos de corte.

**Adaga** — lâmina pequena e leve, adequada para perfurações rápidas e também para arremesso.

**Rapieira** — espada fina e precisa, especializada em estocadas rápidas e perfurações bem colocadas.

**Picareta de guerra** — arma curta de ponta rígida, feita para concentrar a força do golpe em uma área pequena.

**Lança** — haste longa com ponta perfurante, utilizável em combate próximo ou como arma de arremesso.

**Pique** — lança muito longa de duas mãos, voltada a manter ameaças afastadas e realizar estocadas profundas.

**Lança pesada** — versão robusta da lança, dependente das duas mãos para aplicar perfurações de grande impacto.

**Clava** — arma simples e resistente que causa dano por golpes contundentes diretos.

**Maça** — arma de uma mão com cabeça pesada, feita para transmitir grande impacto no ponto atingido.

**Martelo de guerra** — martelo de combate compacto que concentra a força do usuário em golpes pesados e precisos.

**Bastão** — haste longa empunhada com as duas mãos, útil para golpes contundentes e controle corporal.

**Malho** — grande arma de impacto de duas mãos, lenta e pesada, mas capaz de golpes muito fortes.

**Martelo pesado** — martelo de grandes dimensões que exige duas mãos e transforma força física em impacto extremo.
