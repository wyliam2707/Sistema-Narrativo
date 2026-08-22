# Energia

Status: APROVADO

ENERGIA representa a reserva limitada que sustenta usos ativos de capacidades, independentemente de sua explicação ficcional.

Ela pode representar mana, fôlego extraordinário, carga tecnológica, munição abstrata, cargas de um artefato, energia de um anel ou outro recurso consumível coerente com a personagem.

> **Energia é a regra. A fonte diz o que ela representa na ficção.**

## Reserva

A Reserva própria do personagem é determinada pelo maior patamar entre seus Atributos.

`maior Atributo [0] → 10 Energia` | `[1] → 20` | `[2] → 40` | `[3] → 60` | `[4] → 80` | `[5] → 100`

A Reserva mede quanto esforço ou recurso próprio o personagem consegue sustentar. Ela não aumenta o patamar de nenhuma capacidade.

> **Patamar determina quanto o personagem consegue produzir. Reserva determina quanto tempo ele consegue sustentar seus usos.**

## Custo de uso

Quando uma capacidade consome Energia, o custo-base é igual ao patamar efetivamente empregado naquele uso.

`uso [0] → custo 0` | `[1] → 1` | `[2] → 2` | `[3] → 3` | `[4] → 4` | `[5] → 5`

O patamar máximo da capacidade define até onde ela pode chegar. O personagem pode empregar um patamar menor quando a ficção permitir dosar a potência.

Exemplo: `FOR [5] usada em [2] → custo-base 2`.

Assim, um personagem muito poderoso não precisa operar sempre no máximo para resolver ameaças menores.

O custo pode representar coisas diferentes conforme a fonte: mana de um mago, esforço físico extraordinário, carga do anel do Lanterna Verde, batarangs e cargas do Arsenal de Batman ou outro recurso equivalente.

Capacidades passivas não gastam Energia apenas por existirem. Uma resistência natural, armadura já vestida ou característica permanente não consome automaticamente Energia a cada vez que é atingida, salvo quando sua própria descrição estabelecer um gasto ativo.

## Ampliação

Quando uma aplicação é ampliada além de sua manifestação-base, a Consolidação pode gerar uma carga adicional.

Como referência:

`Ampliação [2] → carga +1` | `[4] → +2` | `[8] → +3` | `[16] → +4`

O NARRADOR apresenta o custo como:

`custo [patamar usado + carga de ampliação]`

O JOGADOR escolhe quanto da carga adicional paga em Energia.

Cada ponto de carga de ampliação não pago reduz em `1` o Efeito efetivo daquela aplicação.

Assim, ampliar não reduz obrigatoriamente a potência nem aumenta obrigatoriamente o gasto: o JOGADOR pode pagar com Energia, com eficiência ou combinar os dois.

Exemplo: `Magia [2] => Dano` com carga `+2` é apresentada como `custo [2 + 2]`. Se o JOGADOR paga `3` de Energia, paga o custo-base `2` e apenas `1` da ampliação. O ponto restante reduz o Ataque efetivo em `1`.

A redução não altera o patamar do Poder na ficha. Ela vale somente para aquela aplicação.

A regra detalhada de Consolidação está em `consolidacao.md`.

## Cinco estados

A Reserva pode ser lida em cinco estados narrativos, além de Esgotada:

`Cheia | Alta | Média | Baixa | Crítica | Esgotada`

Os cinco estados com Energia disponível dividem igualmente a Reserva máxima.

O valor numérico pode ser mostrado junto do estado para facilitar o controle. O estado comunica rapidamente a condição; o número preserva precisão operacional.

## Recuperação natural

Todo gasto realizado desde o último fôlego forma um bloco de esforço recente.

Após aproximadamente `5 minutos` de descanso real, o personagem pode recuperar `50%` da Energia gasta nesse bloco. Essa parcela é recuperável uma única vez pelo fôlego curto.

A metade restante torna-se desgaste profundo e só pode ser recuperada com aproximadamente `1 a 2 horas` de descanso real.

Exemplos: `100/100 → gasta 10 → 90/100 → 5m recupera +5 → 95/100 → 2h recupera +5 → 100/100` | `100/100 → gasta 100 → 0/100 → 5m recupera +50 → 50/100 → 2h recupera +50 → 100/100`.

Depois do fôlego de 5 minutos, novos gastos formam um novo bloco e podem gerar nova parcela recuperável no próximo fôlego. A parte já marcada para o descanso longo continua aguardando esse descanso.

Enquanto existir valor preso na camada de descanso longo, a Energia não pode se recuperar naturalmente acima de:

`Energia máxima recuperável antes do descanso longo = Energia máxima − Descanso de 2h`

Exemplo: `Energia [10/100] - Descanso [45]-[45]` permite chegar, com o fôlego curto, no máximo a `55/100`. Depois disso permanece `Energia [55/100] - Descanso [0]-[45]` até ocorrer o descanso prolongado.

> **Fôlego recupera metade do esforço recente. Descanso prolongado recupera o desgaste restante.**

## Bateria

`Bateria [X]` é uma fonte separada de Energia armazenada.

Ela não aumenta a Reserva própria do personagem e não soma seu patamar aos Atributos.

Sua capacidade é:

`Bateria [1] → 20` | `[2] → 40` | `[3] → 60` | `[4] → 80` | `[5] → 100`

Uma Bateria pode ser um medalhão, cristal, bateria tecnológica, fonte mística, estoque de equipamentos ou qualquer outra forma coerente de reserva externa.

Por padrão, a Bateria recupera sua carga completa uma vez por dia. Uma Bateria específica pode estabelecer outra forma de recarga.

## Uso da Bateria

Transferir Energia da Bateria para a Reserva é uma ação.

O personagem pode transferir qualquer quantidade disponível na Bateria, até completar sua Reserva máxima.

Exemplo: `Energia 20/80 - Bateria 60/60 → usa a Bateria → Energia 80/80 - Bateria 0/60`.

Se a Reserva não tiver espaço para toda a carga, apenas a quantidade necessária é transferida e o restante permanece na Bateria.

## Notação operacional

Quando for útil mostrar tudo de forma compacta, usa-se uma única linha:

`Energia [10/100] - Bateria [40/40] - Descanso [45]-[45]`

`Energia [atual/máxima]` mostra a Reserva própria atual e máxima.

`Bateria [atual/máxima]` mostra a carga externa disponível.

`Descanso [X]-[Y]` mostra quanto ainda pode ser recuperado em cada camada de descanso. O primeiro valor corresponde à parcela recuperável pelo fôlego de aproximadamente 5 minutos; o segundo corresponde ao desgaste profundo recuperável após aproximadamente 1 a 2 horas.

Depois de usar o fôlego curto, sua parcela cai para zero. Exemplo: `Energia [55/100] - Bateria [40/40] - Descanso [0]-[45]`.

O segundo valor também define quanto da Reserva máxima continua bloqueado até o descanso prolongado. Portanto, com `Descanso [0]-[45]` em uma Reserva máxima de `100`, o teto de recuperação natural imediata é `55`.

Quando o descanso prolongado é concluído e não existem novos gastos pendentes, ambos os valores retornam a zero.

Quando não houver Bateria, seu trecho pode ser omitido.

## Escala e confronto

A progressão foi calibrada para que um personagem consiga operar repetidamente próximo do próprio patamar máximo durante um confronto sério contra um equivalente.

Um personagem cujo maior Atributo é `[5]` possui `100` de Reserva. Um uso-base em `[5]` custa `5`; ampliações podem elevar esse gasto quando o JOGADOR preferir preservar integralmente o Efeito efetivo.

Isso não significa que toda luta precisa durar vinte usos. Resultado evidente, estratégia, ambiente, diferença de patamar, dano, retirada, incapacidade, ampliação ou qualquer outra consequência podem encerrá-la antes.

> **A Reserva deve permitir um confronto sério entre equivalentes sem transformar esforço máximo em recurso infinito.**
