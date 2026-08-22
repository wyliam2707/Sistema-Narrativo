# Escalas de efeito

Status: EFEITOS CONSOLIDADOS / CONSOLIDAÇÃO EM CONSTRUÇÃO

Este arquivo reúne tabelas de referência para traduzir a Exigência do motor geral de disputa em efeitos concretos.

As tabelas são referências de resolução, não uma lista fechada de Poderes. A natureza da capacidade continua determinando o que ela pode fazer.

## Escala-base

`[2] inicial forte` | `[4] relevante` | `[8] completo` | `[16] profundo/amplo` | `[32] absoluto`

Os nomes concretos dependem da categoria e da natureza do efeito.

> **Não criar uma categoria só porque o tema existe. Criar uma tabela apenas quando ela mede uma consequência que as escalas atuais não conseguem representar.**

## Sentidos — supressão

A escala começa prejudicando um sentido específico. Depois de sua supressão funcional completa, resultados maiores espalham a interferência para os demais sentidos.

`[2] Prejudicar` | `[4] Comprometer` | `[8] Suprimir` | `[16] Supressão ampla` | `[32] Supressão dominante`

- `[2] Prejudicar` — o sentido funciona, mas com dificuldade relevante. Ex.: visão embaçada, pouca luz, ruído atrapalhando a audição.
- `[4] Comprometer` — o sentido continua funcionando, mas perde informação importante. Ex.: ver vultos e silhuetas sem identificar rostos; ouvir sem distinguir bem palavras ou direção.
- `[8] Suprimir` — o sentido deixa de fornecer informação funcional. Ex.: visão equivalente a uma sala totalmente escura; audição completamente abafada.
- `[16] Supressão ampla` — suprime o sentido principal em `[8]` e espalha um efeito `[2]` aos demais sentidos afetáveis.
- `[32] Supressão dominante` — suprime o sentido principal em `[8]` e espalha um efeito `[4]` aos demais sentidos afetáveis.

Não existe “mais que totalmente cego”. Depois da supressão completa do sentido principal, resultados maiores ampliam a consequência para funções relacionadas.

## Controle

`[2] Influenciar` | `[4] Induzir` | `[8] Comandar` | `[16] Dominar` | `[32] Controle absoluto`

- `[2] Influenciar` — a influência pesa fortemente, mas o alvo ainda decide.
- `[4] Induzir` — direciona uma decisão específica; ainda pode existir conflito interno.
- `[8] Comandar` — impõe uma ordem concreta dentro do repertório do Poder.
- `[16] Dominar` — valores, vínculos e interesses podem ser sobrepostos; sequências de ações podem ser impostas.
- `[32] Controle absoluto` — dentro do repertório do Poder, a vontade do alvo deixa funcionalmente de participar da decisão.

A intensidade não expande o repertório. Um Poder de sugestão não se transforma automaticamente em possessão corporal apenas por alcançar `[32]`.

## Mobilidade

`[2] Dificultar` | `[4] Restringir` | `[8] Imobilizar` | `[16] Conter` | `[32] Aprisionar`

- `[2] Dificultar` — mover-se continua possível, mas exige esforço ou perde eficiência.
- `[4] Restringir` — o movimento fica fortemente limitado; algumas direções ou ações deixam de ser viáveis.
- `[8] Imobilizar` — o alvo perde funcionalmente a capacidade de se deslocar.
- `[16] Conter` — além de imobilizado, tentativas simples de escapar, romper ou contornar a contenção deixam de funcionar.
- `[32] Aprisionar` — contenção total dentro da natureza do efeito, exigindo solução ou disputa compatível para escapar.

## Supressão

A mesma régua serve para reduzir Atributos e Poderes.

`[2] −0,5` | `[4] −1,0` | `[8] −2,0` | `[16] −2,0 principal / −0,5 demais` | `[32] −2,0 principal / −1,0 demais`

Referências comuns de Atributo:

`Lento → AGI` | `Fraco → FOR` | `Frágil → RES` | `Confuso → MEN` | `Suscetível → VON`

A supressão de Atributo respeita o piso `[0]`; ela reduz o patamar disponível, não cria Atributo negativo.

Quando aplicada a um Poder, `[0]` significa que o Poder está funcionalmente suprimido enquanto o efeito permanecer.

A defesa contra a Supressão vem daquilo que realmente sustenta a capacidade. Pode ser o próprio Poder, um Atributo coerente ou outra proteção aplicável. Usa-se o maior valor aplicável, sem soma automática.

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

## Informação

`[2] Indício` | `[4] Revelar` | `[8] Compreender` | `[16] Aprofundar` | `[32] Devassar`

- `[2] Indício` — obtém uma pista útil, mas incompleta.
- `[4] Revelar` — identifica a informação principal, ainda com detalhes ausentes.
- `[8] Compreender` — obtém informação funcionalmente completa sobre o objetivo investigado.
- `[16] Aprofundar` — revela relações, causas, contexto e detalhes ocultos relevantes.
- `[32] Devassar` — alcança tudo que aquela capacidade consegue descobrir dentro de seu repertório.

A Resistência vem daquilo que torna a informação difícil de obter: criatura, ocultação, Atributo, proteção ou dificuldade natural da própria informação.

`Exigência` diz quanto se quer descobrir. `Resistência` diz quão difícil é descobrir.

Não se somam automaticamente diferentes fontes de resistência; a ficção determina qual obstáculo está sendo enfrentado naquela aplicação.

## Invocação

Invocação cria uma entidade ou objeto dentro do repertório real do Poder. O patamar determina a configuração máxima da criação; não obriga a usar toda a potência disponível.

### Distribuição de Atributos

Uma criação recebe apenas os Atributos necessários para cumprir sua função. Atributos não elevados permanecem `[0]` ou são irrelevantes.

`Invocação [1] → 1 atributo [1]`

`Invocação [2] → 1 atributo [2] | 2 atributos [1]`

`Invocação [3] → 1 atributo [3] | 2 atributos [2] | 3 atributos [1]`

`Invocação [4] → 1 atributo [4] | 2 atributos [3] | 3 atributos [2] | 4 atributos [1]`

`Invocação [5] → 1 atributo [5] | 2 atributos [4] | 3 atributos [3] | 4 atributos [2] | 5 atributos [1]`

Exemplos: `Cadeira comum → atributos relevantes [0]` | `Mesa reforçada → FOR [1]` | `Parede passiva com Invocação [5] → RES [5]` | `Parede ativa → FOR [4] | RES [4]` | `Golem bruto → FOR [4] | RES [4]` | `Golem de combate → FOR [3] | AGI [3] | RES [3]`.

> **Invocação determina como se estrutura aquilo que foi criado. O Poder determina o que pode ser criado.**

### Quantidade de criaturas

Ao criar várias criaturas no mesmo vínculo, cada dobra na quantidade reduz em 1 o patamar efetivo disponível para cada criatura.

| Invocação | 1 criatura | 2 criaturas | 4 criaturas | 8 criaturas | 16 criaturas |
|---|---:|---:|---:|---:|---:|
| `[1]` | `[1]` | — | — | — | — |
| `[2]` | `[2]` | `[1]` | — | — | — |
| `[3]` | `[3]` | `[2]` | `[1]` | — | — |
| `[4]` | `[4]` | `[3]` | `[2]` | `[1]` | — |
| `[5]` | `[5]` | `[4]` | `[3]` | `[2]` | `[1]` |

O valor da célula é o patamar efetivo de cada criatura antes de distribuir seus Atributos.

Uma nova Invocação de criaturas rompe o vínculo de criaturas anterior e o substitui. Criaturas não podem ser acumuladas uso após uso para escapar da redução por quantidade.

Objetos não usam esse limite de vínculo. Sua permanência, quantidade física, área e tamanho serão tratados pelas escalas de Consolidação/Ampliação.

Criações que agem autonomamente são tratadas como criaturas para esta regra. Criações passivas são tratadas como objetos.

## Metamorfose

Metamorfose usa a mesma lógica de configuração de Invocação, mas aplica a forma ao próprio personagem e somente sobre seus Atributos físicos.

Ao assumir uma nova forma, `FOR`, `AGI` e `RES` da forma anterior deixam de ser usados e partem de `[0]`. A Metamorfose então redefine esses três Atributos conforme sua configuração.

`Metamorfose [1] → [1]/[0]/[0]`

`Metamorfose [2] → [2]/[0]/[0] ou [1]/[1]/[0]`

`Metamorfose [3] → [3]/[0]/[0] ou [2]/[2]/[0] ou [1]/[1]/[1]`

`Metamorfose [4] → [4]/[0]/[0] ou [3]/[3]/[0] ou [2]/[2]/[2]`

`Metamorfose [5] → [5]/[0]/[0] ou [4]/[4]/[0] ou [3]/[3]/[3]`

Os valores podem ser distribuídos entre `FOR`, `AGI` e `RES` conforme a forma.

`MEN` e `VON` permanecem os do personagem. `VIDA` e `Energia` também permanecem originais; trocar de forma não cura Dano nem recupera Energia.

Exemplos: `Pássaro → FOR [0] | AGI [5] | RES [0]` | `Gorila → FOR [4] | AGI [0] | RES [4]` | `Predador equilibrado → FOR [3] | AGI [3] | RES [3]`.

### Transformação imposta

Transformar outra criatura não produz “percentuais de transformação”. A mudança pretendida acontece por inteiro quando alcançada; a oposição determina principalmente quanto ela consegue se consolidar.

Contra uma transformação imposta, usa-se como resistência o maior valor aplicável entre `RES`, `VON` ou outra proteção/Poder coerente.

Na Metamorfose voluntária sobre si mesmo, a defesa contra a própria mudança é `[0]`.

A duração e a persistência da forma pertencem à Consolidação.

## Sono

Sono usa a mesma arquitetura de aprofundamento dos Sentidos.

`[2] Sonolência` | `[4] Torpor` | `[8] Sono` | `[16] Sono [8] + Distração [2]` | `[32] Sono [8] + Distração [4]`

- `[2] Sonolência` — a consciência começa a perder prontidão.
- `[4] Torpor` — atenção e resposta ficam fortemente comprometidas.
- `[8] Sono` — o alvo adormece funcionalmente.
- `[16]` — o alvo está em Sono `[8]` e estímulos externos sofrem Distração `[2]` para alcançá-lo.
- `[32]` — o alvo está em Sono `[8]` e estímulos externos sofrem Distração `[4]` para alcançá-lo.

Depois de `[8]`, não existe “mais dormindo”; o aprofundamento representa o quanto estímulos externos têm dificuldade de alcançar a consciência.

A duração é independente. Um Sono `[8]` que dure uma semana pode ser narrativamente descrito como coma prolongado sem exigir um novo patamar de efeito.

## Ilusão

`[2] Distorcer` | `[4] Ocultar ou Criar` | `[8] Substituir` | `[16] Construir Cena` | `[32] Realidade Ilusória`

- `[2] Distorcer` — altera uma percepção existente sem removê-la completamente.
- `[4] Ocultar ou Criar` — remove um elemento da percepção ou acrescenta um elemento inexistente. Ex.: ocultar uma pessoa ou porta; criar uma pessoa falsa, porta falsa, som ou clarão.
- `[8] Substituir` — oculta o elemento real e coloca outra percepção em seu lugar.
- `[16] Construir Cena` — vários elementos falsos funcionam juntos de forma coerente.
- `[32] Realidade Ilusória` — a experiência perceptiva pode ser amplamente reconstruída dentro do repertório do Poder.

Ilusão também pode ser aplicada à memória quando o repertório do Poder permitir: distorcer, ocultar, criar ou substituir uma lembrança segue a mesma régua.

`Sentidos` reduz ou elimina a capacidade de perceber. `Ilusão` altera aquilo que é percebido.

Duração e persistência pertencem à Consolidação.

## Emoção

Emoção usa a mesma arquitetura de Ilusão, aplicada ao estado emocional.

`[2] Distorcer` | `[4] Ocultar ou Criar` | `[8] Substituir` | `[16] Construir Estado` | `[32] Realidade Emocional`

- `[2] Distorcer` — altera a intensidade ou direção de uma emoção já existente.
- `[4] Ocultar ou Criar` — suprime uma emoção presente ou cria uma que não existia.
- `[8] Substituir` — troca uma emoção por outra.
- `[16] Construir Estado` — combina várias respostas emocionais de forma coerente.
- `[32] Realidade Emocional` — reconstrói amplamente a experiência emocional dentro do repertório do Poder.

Emoção altera o que o alvo sente. Controle altera ou impõe o que ele faz.

Duração e persistência pertencem à Consolidação.

## Deslocar

Deslocar é o efeito fundamental para mudar posição ou estabelecer passagem entre posições. A natureza do Poder determina como isso acontece.

`Telecinese → move fisicamente` | `Teleporte → transporta instantaneamente` | `Portal → conecta posições` | `Banimento → desloca para outro plano`

O Poder produz intensidade como em uma disputa. A oposição vem de quem ou do que realmente impede o deslocamento: `FOR`, `RES`, `VON`, ancoragem, Poder, proteção dimensional ou outro mecanismo coerente.

O resultado acumulado é aplicado às dimensões necessárias da Consolidação, especialmente alcance/distância e duração.

A intenção define primeiro o requisito necessário. Ex.: levantar alguém no ar pode exigir apenas alcance curto; o excedente pode sustentar a duração. Transportar alguém até uma base distante exige alcançar a escala de distância correspondente e pode ter duração instantânea.

O repertório continua limitando o uso. Excedente de Telecinese não permite banimento planar se o Poder não possui essa capacidade.

Quando uma entidade externa interfere, ela pode oferecer Resistência e também agir durante as janelas de aplicação.

> **A Resistência reduz o Progresso por aplicação. O tempo necessário para acumular Progresso cria oportunidades reais de reação.**

## Consolidação — próxima etapa

As escalas de efeito acima definem **o que acontece**.

A próxima etapa define como o resultado disponível é aplicado às dimensões que sustentam ou ampliam esse efeito, incluindo pelo menos:

`Duração` | `Alvos/Quantidade` | `Alcance/Distância` | `Área/Tamanho`

Essas dimensões serão consolidadas separadamente antes de substituir qualquer referência preliminar anterior.
