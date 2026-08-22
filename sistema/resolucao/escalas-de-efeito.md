# Escalas de efeito

Status: EM CONSTRUÇÃO

Este arquivo reúne tabelas de referência para traduzir a Exigência do motor geral de disputa em efeitos concretos.

As tabelas são referências de resolução, não uma lista fechada de Poderes. A natureza da capacidade continua determinando o que ela pode fazer.

## Escala-base

`[2] inicial forte` | `[4] relevante` | `[8] completo` | `[16] profundo/amplo` | `[32] absoluto`

Os nomes concretos dependem da categoria e da natureza do efeito.

## Consolidação: duração e persistência

Quando um efeito persistente supera sua Exigência-base, o excedente forma sua Consolidação.

`Consolidação = Progresso acumulado − Exigência-base`

O mesmo valor representa simultaneamente duração e persistência quando a natureza do efeito permitir.

`[2] instante` | `[4] ~2 turnos` | `[8] ~1 minuto / cena curta` | `[16] ~1 hora` | `[32] ~1 dia`

O marco determina o efeito. O excedente determina quanto ele se consolida.

## Sentidos — supressão

A escala começa prejudicando um sentido específico. Depois de sua supressão funcional completa, resultados maiores espalham a interferência para os demais sentidos.

`[2] Prejudicar` | `[4] Comprometer` | `[8] Suprimir` | `[16] Supressão ampla` | `[32] Supressão dominante`

- `[2] Prejudicar` — o sentido funciona, mas com dificuldade relevante. Ex.: visão embaçada, pouca luz, ruído atrapalhando a audição.
- `[4] Comprometer` — o sentido continua funcionando, mas perde informação importante. Ex.: ver vultos e silhuetas sem identificar rostos; ouvir sem distinguir bem palavras ou direção.
- `[8] Suprimir` — o sentido deixa de fornecer informação funcional. Ex.: visão equivalente a uma sala totalmente escura; audição completamente abafada.
- `[16] Supressão ampla` — suprime o sentido principal em `[8]` e espalha um efeito `[2]` aos demais sentidos afetáveis.
- `[32] Supressão dominante` — suprime o sentido principal em `[8]` e espalha um efeito `[4]` aos demais sentidos afetáveis.

## Controle

`[2] Influenciar` | `[4] Induzir` | `[8] Comandar` | `[16] Dominar` | `[32] Controle absoluto`

A intensidade alcançada mede quanto o efeito consegue interferir na decisão do alvo, sempre dentro do repertório real do Poder usado.

## Mobilidade

`[2] Dificultar` | `[4] Restringir` | `[8] Imobilizar` | `[16] Conter` | `[32] Aprisionar`

- `[2] Dificultar` — mover-se continua possível, mas exige esforço ou perde eficiência.
- `[4] Restringir` — o movimento fica fortemente limitado; algumas direções ou ações deixam de ser viáveis.
- `[8] Imobilizar` — o alvo perde funcionalmente a capacidade de se deslocar.
- `[16] Conter` — além de imobilizado, tentativas simples de escapar, romper ou contornar a contenção deixam de funcionar.
- `[32] Aprisionar` — contenção total dentro da natureza do efeito, exigindo solução ou disputa compatível para escapar.

## Supressão de Atributo

A natureza do efeito determina qual Atributo é reduzido.

`[2] −0,5` | `[4] −1,0` | `[8] −2,0` | `[16] −2,0 principal / −0,5 demais` | `[32] −2,0 principal / −1,0 demais`

Referências comuns:

`Lento → AGI` | `Fraco → FOR` | `Frágil → RES` | `Confuso → MEN` | `Suscetível → VON`

A supressão respeita o piso `[0]`; ela reduz o patamar disponível, não cria Atributo negativo.

## Proteção — Barreira

Barreira funciona como uma camada independente de proteção.

`Barreira [X] → VIDA 4 | RES efetiva = X + (Perícia aplicável × 0,2)`

Como Poder, Barreira possui patamar mínimo `[1]`.

Exemplo: `Barreira [2] + Conhecimento em Magia [+2] → VIDA 4 | RES [2,4]`.

O ataque resolve normalmente contra a RES efetiva da Barreira. O Dano reduz primeiro a VIDA da Barreira.

Se o Dano não superar a VIDA restante, ele é absorvido e reduz essa VIDA.

Se superar, a Barreira é rompida e o excedente continua para a próxima camada ou alvo.

`Excedente = Dano aplicado − VIDA restante da Barreira`

O excedente é convertido novamente em Ataque efetivo usando a fórmula inversa:

`Ataque efetivo restante = RES efetiva da Barreira + log₂(Excedente)`

Depois da reconversão, o Ataque efetivo restante é sempre arredondado para baixo antes de atingir a próxima camada.

Se não houver excedente, o ataque termina na Barreira.

> **Uma proteção absorve aquilo que consegue suportar. O excedente continua com a força que restou.**

A recuperação, reconstrução ou remoção de efeitos e Barreiras será tratada em regra própria posterior.
