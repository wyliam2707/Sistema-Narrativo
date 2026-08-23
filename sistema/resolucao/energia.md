# Energia

Status: APROVADO

ENERGIA representa a reserva limitada usada por capacidades que possuem custo ativo.

Sua explicação ficcional pode ser mana, esforço, carga tecnológica, munição abstrata, combustível, cargas de artefato ou outro recurso coerente.

> **Energia mede quanto recurso ainda pode ser gasto; não aumenta a potência de uma capacidade.**

## 1. Reserva

A Reserva própria é determinada pelo maior Atributo da personagem:

`maior Atributo [0] → 10 Energia` | `[1] → 20` | `[2] → 40` | `[3] → 60` | `[4] → 80` | `[5] → 100`

Exceções aprovadas podem registrar outro valor diretamente na ficha.

## 2. Custo do uso

Quando uma capacidade consome Energia, seu custo-base é o patamar efetivamente usado:

`uso [0] → 0` | `[1] → 1` | `[2] → 2` | `[3] → 3` | `[4] → 4` | `[5] → 5`

Quando houver Ampliação:

`Custo = patamar efetivamente usado + Ampliação usada`

As dimensões, limites e cálculo de Ampliação pertencem exclusivamente a `consolidacao.md`.

O custo é pago antes da resolução da aplicação.

Se não houver Energia suficiente, a configuração precisa ser reduzida antes da resolução.

Capacidades passivas não gastam Energia apenas por existirem, salvo regra específica da própria capacidade.

## 3. Recuperação

Todo gasto realizado desde o último fôlego forma um bloco de esforço recente.

Após aproximadamente `5 minutos` de descanso real, recupera-se `50%` da Energia gasta nesse bloco. Essa parcela só pode ser recuperada uma vez pelo fôlego curto.

A metade restante exige aproximadamente `1 a 2 horas` de descanso real.

Novos gastos depois do fôlego formam um novo bloco sem apagar o desgaste profundo já acumulado.

Enquanto houver desgaste profundo pendente, ele limita quanto da Reserva pode ser recuperado naturalmente:

`máximo recuperável antes do descanso longo = Energia máxima − desgaste profundo`

> **Fôlego recupera metade do esforço recente. Descanso prolongado recupera o restante.**

## 4. Bateria

`Bateria [X]` representa uma reserva externa separada.

Capacidade:

`Bateria [1] → 20` | `[2] → 40` | `[3] → 60` | `[4] → 80` | `[5] → 100`

A Bateria não aumenta a Reserva própria nem altera Atributos ou patamares.

Sua natureza e forma de recarga pertencem à própria capacidade ou recurso. Na ausência de regra específica, recupera sua carga completa uma vez por dia.

Quando a Bateria puder alimentar a Reserva, transfere-se até a quantidade disponível ou até completar a Reserva máxima.

## 5. Notação operacional

Quando necessário:

`Energia [atual/máxima] - Bateria [atual/máxima] - Descanso [curto]-[profundo]`

Exemplo:

`Energia [55/100] - Bateria [40/40] - Descanso [0]-[45]`

Trechos sem valor relevante podem ser omitidos.

O STATUS apenas preserva esses valores atuais; os cálculos pertencem a este arquivo.

## Regra final

> **Reserva diz quanto recurso existe. A configuração define quanto custa. Bateria fornece reserva externa. Descanso recupera o que foi gasto.**