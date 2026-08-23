# Escalas de efeito

Status: EFEITOS CONSOLIDADOS

Este arquivo reúne tabelas de referência para traduzir a Exigência do motor geral de disputa em efeitos concretos.

As tabelas são referências de resolução, não uma lista fechada de Poderes. A natureza da capacidade continua determinando o que ela pode fazer.

## Regra estrutural dos efeitos persistentes

Todo efeito persistente comum possui uma Defesa e uma Vida próprias:

`D = nível do efeito usado + (Perícia aplicável × 0,2)`

`V = maior entre [1] e o Atributo estrutural da Fonte`

A Defesa é determinada pelo nível efetivamente usado e pela Perícia aplicável. A Vida é determinada pela Fonte, conforme `fonte-e-vida-estrutural.md`.

Essa regra vale para efeitos persistentes como `Proteção`, `Imobilizar`, `Supressão`, `Sono`, `Ilusão`, `Emoção` e outros efeitos que permaneçam em cena e possam ser atacados ou dissipados. Cada efeito ainda pode possuir regras específicas adicionais.

`Invocação` é uma exceção estrutural: a Vida da criação e a Defesa da criação seguem as regras próprias da Invocação, e a Defesa usa a `RES` da própria criação.

Quando a Vida estrutural de um efeito persistente chega a `V0`, o efeito encerra imediatamente. Não existe estado residual automático nem funcionamento parcial depois de `V0`, salvo quando uma regra específica disser expressamente o contrário.

### Aplicações iguais no mesmo alvo

Quando duas ou mais aplicações **do mesmo efeito persistente** atingem o mesmo alvo, elas não se acumulam por soma. Elas se consolidam em uma única instância.

A instância consolidada mantém os melhores componentes entre as aplicações compatíveis:

`D consolidada = maior D entre as aplicações`

`V consolidada = maior V entre as aplicações`

A intensidade e a duração mantêm a melhor configuração válida entre as aplicações quando forem realmente o mesmo efeito funcional.

Exemplo:

`Imobilizar A → D3,4 / V2`

`Imobilizar B → D2,8 / V4`

`Resultado consolidado → Imobilizar [D3,4 / V4]`

Essa consolidação vale somente para efeitos iguais. Efeitos diferentes, como `Imobilizar` e `Sono`, continuam existindo como instâncias separadas.

> **Efeitos iguais preservam os melhores componentes; efeitos diferentes não se fundem.**

## Escala-base

`[2] inicial forte` | `[4] relevante` | `[8] completo` | `[16] profundo/amplo` | `[32] absoluto`

Os nomes concretos dependem da categoria e da natureza do efeito.

> **Não criar uma categoria só porque o tema existe. Criar uma tabela apenas quando ela mede uma consequência que as escalas atuais não conseguem representar.**

## Base de manifestação

Cada efeito possui uma manifestação-base. Ela descreve como o efeito funciona normalmente antes de qualquer ampliação.

A leitura segue, quando aplicável:

`Efeito — Alcance / Alvos / Área ou Tamanho / Duração / Efetivo máximo [nível disponível]`

A base não determina sozinha o Resultado. O Resultado continua vindo da resolução contra a oposição aplicável.

Alterar Alcance, quantidade de Alvos, Área/Tamanho ou Duração além da base pertence às regras de Ampliação e custo.

> **Base do efeito = como ele normalmente se manifesta. Resultado = intensidade que ele consegue produzir contra a oposição. Ampliações = mudanças opcionais nessa manifestação.**

## Dano

A base de Dano depende da forma real pela qual ele é entregue.

`Dano [soco/espada/luta] — Curto / 1 alvo / Pontual / Instantâneo / Efetivo máximo [nível disponível]`

`Dano [disparo] — Médio / 1 alvo / Pontual / Instantâneo / Efetivo máximo [nível disponível]`

O Resultado de Dano é o Dano aplicado pela regra normal de combate e dano.

## Cura

Base de uso:

`Cura — Toque / 1 alvo / Pontual / Instantâneo / Efetivo máximo [nível disponível]`

O Resultado de Cura é a quantidade de VIDA recuperada pela regra normal de cura.

## Dissipar

Dissipar é um efeito próprio. Ele causa dano sobre a estrutura de **STATUS persistentes**, não sobre a Vida física comum do alvo.

Base de uso:

`Dissipar — Médio / 1 alvo / Pontual / Instantâneo / 1 STATUS / Efetivo máximo [nível do efeito]`

A quantidade de STATUS é uma dimensão específica de Dissipar e é adicional às dimensões gerais de Alvos e Área.

`1 STATUS [base] → +0` | `2 STATUS → +1` | `4 STATUS → +2` | `6 STATUS → +3` | `16 STATUS → +4` | `32 STATUS → +5`

`STATUS` define quantos efeitos persistentes diferentes podem ser atacados pela mesma aplicação. `Alvos` define em quantos alvos essas instâncias podem ser escolhidas. `Área` define o espaço atingido quando a aplicação usa uma zona.

Exemplo: `Dissipar [1] | 1 STATUS | 2 alvos [+1] | Área Pontual [+0]` pode atacar uma instância de STATUS em cada um de dois alvos.

Cada STATUS atingido resolve separadamente contra sua própria Defesa:

`Dissipar efetivo vs D do efeito persistente → Dano aplicado → reduz V do efeito`

Todo efeito persistente consolidado segue a regra de Defesa e Vida estrutural definida no topo deste arquivo e em `fonte-e-vida-estrutural.md`.

Dissipar pode atingir tanto efeitos prejudiciais quanto benéficos persistentes, desde que estejam dentro de seu repertório.

> **Dissipar é dano contra STATUS persistente. STATUS, Alvos e Área medem coisas diferentes e podem ser ampliados separadamente.**

## Sentidos — supressão

Base de uso:

`Sentidos — Médio / 1 alvo / Pontual / Cena / Efetivo máximo [nível do efeito]`

A escala começa prejudicando um sentido específico. Depois de sua supressão funcional completa, resultados maiores espalham a interferência para os demais sentidos.

`[2] Prejudicar` | `[4] Comprometer` | `[8] Suprimir` | `[16] Supressão ampla` | `[32] Supressão dominante`

- `[2] Prejudicar` — o sentido funciona, mas com dificuldade relevante.
- `[4] Comprometer` — o sentido continua funcionando, mas perde informação importante.
- `[8] Suprimir` — o sentido deixa de fornecer informação funcional.
- `[16] Supressão ampla` — suprime o sentido principal em `[8]` e espalha um efeito `[2]` aos demais sentidos afetáveis.
- `[32] Supressão dominante` — suprime o sentido principal em `[8]` e espalha um efeito `[4]` aos demais sentidos afetáveis.

Não existe “mais que totalmente cego”. Depois da supressão completa do sentido principal, resultados maiores ampliam a consequência para funções relacionadas.

## Controle

Base de uso:

`Controle — Médio / 1 alvo / Pontual / Cena / Efetivo máximo [nível do efeito]`

`[2] Influenciar` | `[4] Induzir` | `[8] Comandar` | `[16] Dominar` | `[32] Controle absoluto`

- `[2] Influenciar` — a influência pesa fortemente, mas o alvo ainda decide.
- `[4] Induzir` — direciona uma decisão específica; ainda pode existir conflito interno.
- `[8] Comandar` — impõe uma ordem concreta dentro do repertório do Poder.
- `[16] Dominar` — valores, vínculos e interesses podem ser sobrepostos; sequências de ações podem ser impostas.
- `[32] Controle absoluto` — dentro do repertório do Poder, a vontade do alvo deixa funcionalmente de participar da decisão.

A intensidade não expande o repertório. Um Poder de sugestão não se transforma automaticamente em possessão corporal apenas por alcançar `[32]`.

## Mobilidade

Base de uso:

`Mobilidade / Imobilizar — Médio / 1 alvo / Pontual / Cena / Efetivo máximo [nível do efeito]`

`[2] Dificultar` | `[4] Restringir` | `[8] Imobilizar` | `[16] Conter` | `[32] Aprisionar`

- `[2] Dificultar` — mover-se continua possível, mas exige esforço ou perde eficiência.
- `[4] Restringir` — o movimento fica fortemente limitado; algumas direções ou ações deixam de ser viáveis.
- `[8] Imobilizar` — o alvo perde funcionalmente a capacidade de se deslocar.
- `[16] Conter` — além de imobilizado, tentativas simples de escapar, romper ou contornar a contenção deixam de funcionar.
- `[32] Aprisionar` — contenção total dentro da natureza do efeito, exigindo solução ou disputa compatível para escapar.

## Supressão

Base de uso:

`Supressão — Médio / 1 alvo / Pontual / Cena / Efetivo máximo [nível do efeito]`

A mesma régua serve para reduzir Atributos e Poderes.

`[2] −0,5` | `[4] −1,0` | `[8] −2,0` | `[16] −2,0 principal / −0,5 demais` | `[32] −2,0 principal / −1,0 demais`

Referências comuns de Atributo:

`Lento ou Fraco → FIS` | `Frágil → RES` | `Confuso → MEN` | `Suscetível → VON`

O nome da condição continua descrevendo **qual aspecto ficcional** foi afetado. Como força, velocidade, coordenação e reação agora pertencem ao mesmo Atributo, diferentes supressões físicas podem reduzir FIS sem se transformarem na mesma condição narrativa.

A supressão de Atributo respeita o piso `[0]`; ela reduz o patamar disponível, não cria Atributo negativo.

Quando aplicada a um Poder, `[0]` significa que o Poder está funcionalmente suprimido enquanto o efeito permanecer.

A defesa contra a Supressão vem daquilo que realmente sustenta a capacidade. Pode ser o próprio Poder, um Atributo coerente ou outra proteção aplicável. Usa-se o maior valor aplicável, sem soma automática.

## Proteção — Barreira

Base de uso:

`Proteção/Barreira — Si mesmo / 1 alvo / Pontual / Cena / Efetivo máximo [nível da Proteção]`

Barreira funciona como uma camada independente de proteção.

`Barreira [D / V]`

A Defesa segue a regra geral de efeitos persistentes:

`D = nível da Proteção usado + (Perícia aplicável × 0,2)`

A Vida segue a regra de Fonte:

`V = maior entre [1] e o Atributo estrutural da Fonte`

O ataque resolve normalmente contra `D` da Barreira. O Dano reduz primeiro sua Vida.

Se o Dano não superar a Vida restante, ele é absorvido e reduz essa Vida.

Se superar, a Barreira é rompida e o excedente continua para a próxima camada ou alvo.

`Excedente = Dano aplicado − Vida restante da Barreira`

`Ataque efetivo restante = D da Barreira + log₂(Excedente)`

Depois da reconversão, o Ataque efetivo restante é sempre arredondado para baixo antes de atingir a próxima camada.

Se não houver excedente, o ataque termina na Barreira.

> **Proteção é um efeito persistente comum: sua Defesa vem do nível usado e Perícia; sua Vida vem da Fonte.**

## Informação

Base de uso:

`Informação — Curto / 1 alvo ou fonte / Pontual / Instantâneo / Efetivo máximo [nível do efeito]`

`[2] Indício` | `[4] Revelar` | `[8] Compreender` | `[16] Aprofundar` | `[32] Devassar`

A Resistência vem daquilo que torna a informação difícil de obter: criatura, ocultação, Atributo, proteção ou dificuldade natural da própria informação.

`Exigência` diz quanto se quer descobrir. `Resistência` diz quão difícil é descobrir.

Não se somam automaticamente diferentes fontes de resistência; a ficção determina qual obstáculo está sendo enfrentado naquela aplicação.

### Foco e vínculo

Informação pode exigir um foco para alcançar alguém ou alguma fonte que não esteja disponível diretamente. O foco é uma condição de vínculo, não um bônus numérico automático.

Exemplos possíveis, conforme a natureza do Poder: `cabelo | sangue | objeto pessoal | nome verdadeiro | fotografia | espelho preparado`.

Possuir o foco permite estabelecer o mecanismo quando o repertório realmente comporta esse tipo de leitura. Ele não aumenta sozinho o Efetivo nem aprofunda o Resultado.

> **O foco torna a leitura possível. O Resultado determina quanto é descoberto.**

## Invocação

Base de uso:

`Invocação — Médio / 1 criação / Tamanho Humano / Cena / Efetivo máximo [nível da Invocação]`

Invocação é um **efeito de criação/chamada**: pode trazer, criar ou chamar um aliado, criatura, objeto, máquina ou outro reforço coerente com o repertório do Poder. A aparência ou natureza física do resultado não determina por si só o Atributo da Fonte.

A capacidade de invocar e a estrutura da criatura resultante são coisas diferentes. Uma criação física pode ser produzida por magia, tecnologia, conhecimento ou outra Fonte. Um robô pode, por exemplo, ser invocado por uma capacidade de engenharia baseada em MEN; sua `RES` e seus demais Atributos pertencem à própria criatura, não ao invocador.

### Invocação sustentada por MEN/VON

Para uma Invocação sustentada por eixo mágico/mental (`MEN` ou `VON`), a Vida da criação é:

`Vida = maior entre MEN e VON + 3`

A fórmula vale para a Vida da **criação invocada**, não para a Vida do invocador.

### Defesa da criação

Quando a Invocação for atacada diretamente, sua Defesa estrutural usa a **RES da própria criatura ou objeto invocado**.

`Defesa da Invocação = RES da própria criação`

A RES da criação é determinada pela distribuição de Atributos da própria Invocação.

### Outras Fontes de Invocação

Quando a Invocação for sustentada por outra Fonte coerente, a Vida estrutural da manifestação usa a regra da Fonte aplicável, respeitando o mínimo `[1]`. Isso não transforma `RES` do invocador em requisito universal para Invocação.

### Distribuição de Atributos da criação

Uma criação recebe apenas os Atributos necessários para cumprir sua função. Atributos não elevados permanecem `[0]` ou são irrelevantes.

`Invocação [1] → 1 atributo [1]`

`Invocação [2] → 1 atributo [2] | 2 atributos [1]`

`Invocação [3] → 1 atributo [3] | 2 atributos [2] | 3 atributos [1]`

`Invocação [4] → 1 atributo [4] | 2 atributos [3] | 3 atributos [2] | 4 atributos [1]`

`Invocação [5] → 1 atributo [5] | 2 atributos [4] | 3 atributos [3] | 4 atributos [2]`

Como existem quatro Atributos universais (`FIS | RES | MEN | VON`), não existe uma quinta posição de distribuição.

Exemplos: `Cadeira comum → atributos relevantes [0]` | `Parede passiva → RES [5]` | `Parede ativa → FIS [4] | RES [4]` | `Golem bruto → FIS [4] | RES [4] | MEN [0]` | `Entidade equilibrada → FIS [3] | RES [3] | MEN [3]`.

> **Invocação determina a chamada/criação. Os Atributos, a Vida e a Defesa pertencem à criatura ou objeto resultante.**

### Função, contenção e eixo da disputa

Os Atributos da criação representam funções reais dela. Uma contenção pode concentrar sua configuração em qualquer Atributo coerente com o mecanismo que a mantém funcionando, desde que isso caiba no repertório do Poder.

Exemplos: `Contenção física ativa → FIS [5]` | `Contenção estrutural → RES [5]` | `Contenção mental → MEN [5]` | `Contenção espiritual → VON [5]`.

Isso não transforma o Atributo escolhido em uma defesa universal. O alvo continua podendo responder por qualquer mecanismo que permaneça realmente disponível na situação.

Como `FIS` reúne força, velocidade, coordenação e reação, duas respostas físicas diferentes podem usar o mesmo Atributo sem se tornarem a mesma ação. O mecanismo continua importando: romper, escapar por movimento, atacar a fonte, mudar a posição ou usar outro recurso são soluções diferentes mesmo quando algumas consultam FIS.

Contra um alvo livre e capaz de reagir, uma contenção especializada pode precisar primeiro alcançá-lo, acompanhá-lo ou sobreviver às suas respostas. O alvo também pode destruir a criação, dissipar um efeito quando isso for permitido, teleportar-se ou usar outro meio coerente.

Uma condição anterior pode eliminar alternativas. Se o alvo já estiver `Imobilizado [8]`, por exemplo, uma Invocação posterior pode concentrar sua configuração na função necessária para mantê-lo preso em vez de reproduzir uma disputa de captura já resolvida. Isso não é bônus nem combinação automática: a primeira resolução mudou a situação.

Da mesma forma, conhecer o alvo pode orientar o mecanismo escolhido. Uma prisão física pode ser inútil contra alguém capaz de rompê-la facilmente, enquanto uma contenção de VON pode ser mais adequada se o Poder realmente puder prender por esse eixo.

> **A criação escolhe os Atributos que realizam sua função. A fuga enfrenta o mecanismo que realmente a sustenta. Enquanto houver alternativas coerentes de reação, o alvo pode mudar o mecanismo da resposta.**

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

Objetos não usam esse limite de vínculo. Sua permanência, quantidade física, Área e Tamanho usam as regras de Consolidação.

Criações que agem autonomamente são tratadas como criaturas para esta regra. Criações passivas são tratadas como objetos.

A relação entre o patamar total de Invocação, o patamar usado na criação e a Consolidação natural está detalhada em `consolidacao.md`.

## Transformação

Base de uso:

`Transformação — Si mesmo / 1 alvo / Pontual / Cena / Efetivo máximo [nível da Transformação]`

Transformação usa a mesma lógica de configuração de Invocação quando redefine a própria forma física, mas aplica a configuração sobre `FIS` e `RES` do alvo transformado.

Quando o personagem transforma voluntariamente a si mesmo, `FIS` e `RES` da forma anterior deixam de ser usados e partem de `[0]`. A Transformação então redefine esses dois Atributos conforme sua configuração.

`Transformação [1] → [1]/[0]`

`Transformação [2] → [2]/[0] ou [1]/[1]`

`Transformação [3] → [3]/[0] ou [2]/[2]`

`Transformação [4] → [4]/[0] ou [3]/[3]`

`Transformação [5] → [5]/[0] ou [4]/[4]`

Os valores podem ser distribuídos entre `FIS` e `RES` conforme a forma.

`MEN` e `VON` permanecem os do personagem. `VIDA` e `Energia` também permanecem originais; trocar de forma não cura Dano nem recupera Energia.

Exemplos: `Forma extremamente veloz/ágil → FIS [5] | RES [0]` | `Gorila sobrenatural → FIS [4] | RES [4]`.

### Transformação imposta

Transformar outra criatura não produz “percentuais de transformação”. A mudança pretendida acontece por inteiro quando alcançada; a oposição determina principalmente quanto ela consegue se consolidar.

Contra uma Transformação imposta, usa-se como resistência o maior valor aplicável entre `RES`, `VON` ou outra proteção/Poder coerente.

Na Transformação voluntária sobre si mesmo, a defesa contra a própria mudança é `[0]`.

A Duração e as demais dimensões da forma usam como ponto de partida a base da Transformação e podem ser ampliadas quando necessário.

## Sono

Base de uso:

`Sono — Médio / 1 alvo / Pontual / Cena / Efetivo máximo [nível do efeito]`

Sono usa a mesma arquitetura de aprofundamento dos Sentidos.

`[2] Sonolência` | `[4] Torpor` | `[8] Sono` | `[16] Sono [8] + Distração [2]` | `[32] Sono [8] + Distração [4]`

- `[2] Sonolência` — a consciência começa a perder prontidão.
- `[4] Torpor` — atenção e resposta ficam fortemente comprometidas.
- `[8] Sono` — o alvo adormece funcionalmente.
- `[16]` — o alvo está em Sono `[8]` e estímulos externos sofrem Distração `[2]` para alcançá-lo.
- `[32]` — o alvo está em Sono `[8]` e estímulos externos sofrem Distração `[4]` para alcançá-lo.

Depois de `[8]`, não existe “mais dormindo”; o aprofundamento representa o quanto estímulos externos têm dificuldade de alcançar a consciência.

A Duração é independente. Um Sono `[8]` que dure uma semana pode ser narrativamente descrito como coma prolongado sem exigir um novo patamar de efeito.

## Ilusão

Base de uso:

`Ilusão — Médio / 1 alvo ou elemento / Pontual / Cena / Efetivo máximo [nível do efeito]`

`[2] Distorcer` | `[4] Ocultar ou Criar` | `[8] Substituir` | `[16] Construir Cena` | `[32] Realidade Ilusória`

- `[2] Distorcer` — altera uma percepção existente sem removê-la completamente.
- `[4] Ocultar ou Criar` — remove um elemento da percepção ou acrescenta um elemento inexistente.
- `[8] Substituir` — oculta o elemento real e coloca outra percepção em seu lugar.
- `[16] Construir Cena` — vários elementos falsos funcionam juntos de forma coerente.
- `[32] Realidade Ilusória` — a experiência perceptiva pode ser amplamente reconstruída dentro do repertório do Poder.

Ilusão também pode ser aplicada à memória quando o repertório do Poder permitir: distorcer, ocultar, criar ou substituir uma lembrança segue a mesma régua.

`Sentidos` reduz ou elimina a capacidade de perceber. `Ilusão` altera aquilo que é percebido.

## Emoção

Base de uso:

`Emoção — Médio / 1 alvo / Pontual / Cena / Efetivo máximo [nível do efeito]`

Emoção usa a mesma arquitetura de Ilusão, aplicada ao estado emocional.

`[2] Distorcer` | `[4] Ocultar ou Criar` | `[8] Substituir` | `[16] Construir Estado` | `[32] Realidade Emocional`

- `[2] Distorcer` — altera a intensidade ou direção de uma emoção já existente.
- `[4] Ocultar ou Criar` — suprime uma emoção presente ou cria uma que não existia.
- `[8] Substituir` — troca uma emoção por outra.
- `[16] Construir Estado` — combina várias respostas emocionais de forma coerente.
- `[32] Realidade Emocional` — reconstrói amplamente a experiência emocional dentro do repertório do Poder.

Emoção altera o que o alvo sente. Controle altera ou impõe o que ele faz.

## Deslocar

Deslocar é o efeito fundamental para mudar posição ou estabelecer passagem entre posições. A natureza do Poder determina como isso acontece.

`Telecinese → move fisicamente` | `Teleporte → transporta instantaneamente` | `Portal → conecta posições` | `Banimento → desloca para outra posição ou plano`

As formas possuem bases diferentes porque o modo de manifestação muda.

### Telecinese

`Telecinese — Médio / 1 alvo / Pontual / Instantâneo / Efetivo máximo [nível do efeito]`

O Resultado determina quanto deslocamento físico o efeito consegue produzir contra a resistência aplicável.

### Teleporte

`Teleporte — Toque / 1 alvo / Pontual / Instantâneo / Efetivo máximo [nível do efeito]`

A distância alcançada é lida pelo Resultado:

`[0] Local` | `[2] Cidade` | `[4] Estado/Região` | `[8] País` | `[16] Planeta` | `[32] Planar`

### Portal

`Portal — Curto / 1 portal / Tamanho Humano / Instantâneo / Efetivo máximo [nível do efeito]`

A distância entre as posições conectadas é lida pelo Resultado:

`[0] Local` | `[2] Cidade` | `[4] Estado/Região` | `[8] País` | `[16] Planeta` | `[32] Planar`

### Banimento

`Banimento — Médio / 1 alvo / Pontual / Instantâneo / Efetivo máximo [nível do efeito]`

A distância do deslocamento é lida pelo Resultado:

`[0] Local` | `[2] Cidade` | `[4] Estado/Região` | `[8] País` | `[16] Planeta` | `[32] Planar`

A oposição vem de quem ou do que realmente impede o deslocamento: `FIS`, `RES`, `VON`, ancoragem, Poder, proteção dimensional ou outro mecanismo coerente.

O repertório continua limitando o uso. Um Resultado suficiente para distância Planar não permite banimento planar se o Poder não possui essa capacidade.

> **Alcance = chegar até o alvo. Distância = até onde o efeito o desloca ou conecta.**

## Consolidação

As tabelas acima definem **o que acontece** e cada base define **como o efeito normalmente se manifesta**.

`consolidacao.md` detalha as ampliações dessas manifestações, incluindo:

`Duração` | `Alvos` | `Alcance` | `Área/Tamanho`

A Consolidação também define o limite `Ampliação [X]`, o custo adicional de cada degrau e a regra de pagamento integral da configuração escolhida.