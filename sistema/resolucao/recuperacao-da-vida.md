# Recuperação da VIDA

Status: APROVADO

Este arquivo trata da recuperação de VIDA por tempo, Regeneração e Medicina.

A regra do efeito `Cura` pertence a `efeitos/cura.md`.

`RES` ajuda o personagem a suportar dano, mas não acelera sua recuperação.

## Recuperação natural por estado

A recuperação natural acontece por estado, não ponto a ponto.

Referência de tempo para reduzir um estado de VIDA:

`Ferido → 1 dia` | `Ferido* → 3 dias` | `Grave → 1 semana` | `Grave* → 2 semanas` | `Crítico → 1 mês` | `Crítico* → 2 meses`

Ao completar o período adequado de recuperação, o personagem desce um estado e o Dano acumulado é reduzido em `5`, preservando sua posição relativa dentro da faixa.

Exemplo: `Vida: Crítico | Dano: 27 → 1 mês → Vida: Grave* | Dano: 22`.

Depois disso, o novo estado passa a determinar o próximo período de recuperação.

Exemplo de recuperação natural completa a partir de `Crítico*`:

`Crítico* → 2 meses → Crítico → 1 mês → Grave* → 2 semanas → Grave → 1 semana → Ferido* → 3 dias → Ferido → 1 dia → Ileso`

Os tempos são referências para recuperação adequada. A natureza da lesão, repouso, tratamento e circunstâncias podem justificar variação.

## Regeneração

`Regeneração [X]` representa recuperação própria extraordinariamente acelerada.

Em condições adequadas de recuperação, ela reduz `X` pontos de Dano acumulado por hora.

`Regeneração [1] → 1/h` | `[2] → 2/h` | `[3] → 3/h` | `[4] → 4/h` | `[5] → 5/h`

Ela não é defesa: não reduz o Dano quando ele é recebido e não aumenta `RES`.

A atuação forçada de Regeneração durante conflito, caso exista para uma capacidade específica, pertence às regras de uso ativo e Energia; esta regra trata apenas da recuperação regenerativa normal.

## Medicina

`Medicina` é uma Perícia aberta, seguindo as regras gerais de Perícias.

Quando o paciente aceita o tratamento, está inconsciente ou de outra forma não oferece resistência, Medicina não é uma disputa e não possui oposição artificial.

A resolução lê a Perícia do profissional, os recursos disponíveis, o tempo, a natureza da lesão e a gravidade do estado.

Quando existe tratamento médico adequado durante a recuperação natural, cada grau de Medicina reduz diretamente em `10%` o tempo necessário para recuperar cada estado.

`Medicina [+0] → 100% do tempo` | `[+1] → 90%` | `[+2] → 80%` | `[+3] → 70%` | `[+4] → 60%` | `[+5] → 50%`

`Tempo final = Tempo normal × (1 − 0,10 × Medicina)`

Essa redução pressupõe que o tratamento apropriado possa realmente ser fornecido com os recursos, condições e continuidade necessários. A Perícia não cria equipamentos, medicamentos ou capacidade sobrenatural inexistentes na ficção.

Medicina pode tratar, estabilizar, diagnosticar, impedir agravamento e melhorar a recuperação dentro do que os meios disponíveis permitem.

> **Medicina reduz o tempo. Cura remove Dano diretamente. Regeneração transforma recuperação em horas.**

## Incapacitado

`Incapacitado` não entra automaticamente na sequência de recuperação natural.

Primeiro a personagem precisa sobreviver e ser estabilizada conforme a natureza do dano. Depois disso, a resolução estabelece em qual estado ela inicia a recuperação, normalmente `Crítico*` ou `Crítico` quando a lesão foi severa.

Medicina pode ser decisiva nessa estabilização quando houver tempo, recursos e competência apropriados.

## Princípio

> **Energia volta rápido porque representa esforço. VIDA volta devagar porque representa dano real.**

> **RES suporta o dano. Recuperação trata o que ficou depois dele.**
