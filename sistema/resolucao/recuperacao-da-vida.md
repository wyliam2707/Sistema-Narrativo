# Recuperação da VIDA

Status: APROVADO

A recuperação natural de VIDA é lenta e acompanha a gravidade real do ferimento.

`RES` ajuda o personagem a suportar dano, mas não acelera sua cura. Recuperação acelerada pertence a tratamento, Cura, Regeneração ou outra capacidade específica.

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

Assim, Regeneração realiza em horas uma recuperação que naturalmente poderia exigir dias, semanas ou meses.

Ela não é defesa: não reduz o Dano quando ele é recebido e não aumenta `RES`.

A atuação forçada de Regeneração durante conflito, caso exista para uma capacidade específica, pertence às regras de uso ativo e Energia; esta regra trata apenas da recuperação regenerativa normal.

## Cura

Cura é o contraponto mecânico do Dano.

Dano aumenta o Dano acumulado. Cura reduz o Dano acumulado.

Quando uma Cura é aplicada, usa-se a mesma lógica de comparação exponencial empregada pelo Dano, mas em sentido restaurador.

Quando uma Perícia realmente governa a aplicação da Cura e não existe oposição, ela entra apenas como técnica de quem cura.

`Cura efetiva = Cura usada + 1 + (Perícia aplicável × 0,2) − Ampliação não paga`

`Cura aplicada = máx(1, 2^(Cura efetiva − RES do alvo))`

`Ampliação não paga` normalmente é `0`. Quando Alcance, Alvos ou Área são ampliados pela regra de Consolidação, cada ponto de carga adicional que o JOGADOR escolhe não pagar em Energia reduz a Cura efetiva em `1` naquela aplicação.

A Cura aplicada reduz o Dano acumulado, nunca abaixo de zero.

Uma aplicação capaz de recuperar Dano usa pelo menos patamar `[1]`; seu custo-base de Energia segue a regra normal do patamar efetivamente usado. Ampliações podem acrescentar custo conforme `consolidacao.md`.

A resistência do alvo importa porque organismos mais extraordinários também são mais difíceis de alterar e reconstruir. Uma Cura muito abaixo da `RES` ainda recupera no mínimo `1` ponto por aplicação bem-sucedida.

Isso permite que um curador inferior trate um alvo muito mais resistente, mas de forma lenta e custosa em Energia e tempo.

Exemplo conceitual: se cada aplicação só alcança a Cura mínima de `1`, remover `35` de Dano exige `35` aplicações e o custo correspondente aos patamares usados.

Uma Cura ampliada para vários Alvos ou Área não divide automaticamente seu valor entre os afetados. A ampliação é paga antes da aplicação por Energia, perda de Cura efetiva ou uma combinação das duas.

Depois que a Cura é aplicada, permanece a redução de Dano na VIDA; a Cura não continua existindo como efeito persistente apenas para representar aquilo que já restaurou.

> **Dano e Cura usam a mesma régua de diferença de patamar; um destrói, o outro restaura.**

## Medicina

`Medicina` é uma Perícia aberta, seguindo as regras gerais de Perícias.

Quando o paciente aceita o tratamento, está inconsciente ou de outra forma não oferece resistência, Medicina não é uma disputa e não possui oposição artificial.

A resolução lê a Perícia do profissional, os recursos disponíveis, o tempo, a natureza da lesão e a gravidade do estado.

`Medicina [+0]` pode sustentar cuidados cotidianos plausíveis e primeiros socorros simples. Graus maiores representam formação, experiência e capacidade progressivamente superiores; especialidades como `Cirurgião` podem prevalecer quando forem mais específicas para o procedimento.

Quando existe tratamento médico adequado durante a recuperação natural, cada grau de Medicina reduz diretamente em `10%` o tempo necessário para recuperar cada estado.

`Medicina [+0] → 100% do tempo` | `[+1] → 90%` | `[+2] → 80%` | `[+3] → 70%` | `[+4] → 60%` | `[+5] → 50%`

`Tempo final = Tempo normal × (1 − 0,10 × Medicina)`

Exemplo: `Crítico → 1 mês` com `Medicina [+5]` exige aproximadamente `15 dias` de recuperação adequada.

Essa redução pressupõe que o tratamento apropriado possa realmente ser fornecido com os recursos, condições e continuidade necessários. A Perícia não cria equipamentos, medicamentos, instalações ou procedimentos inexistentes na ficção.

Medicina não cria capacidade sobrenatural de reconstrução. Sem um Poder, tecnologia ou recurso que efetivamente produza Cura, a Perícia trata, estabiliza, diagnostica, impede agravamento e melhora as condições de recuperação dentro do que a medicina disponível consegue realizar.

> **Medicina reduz o tempo. Cura remove Dano diretamente. Regeneração transforma recuperação em horas.**

## Incapacitado

`Incapacitado` não entra automaticamente na sequência de recuperação natural.

Primeiro a personagem precisa sobreviver e ser estabilizada conforme a natureza do dano. Depois disso, a resolução estabelece em qual estado ela inicia a recuperação, normalmente `Crítico*` ou `Crítico` quando a lesão foi severa.

Medicina pode ser decisiva nessa estabilização quando houver tempo, recursos e competência apropriados.

## Princípio

> **Energia volta rápido porque representa esforço. VIDA volta devagar porque representa dano real.**

> **RES suporta o dano. Recuperação trata o que ficou depois dele.**
