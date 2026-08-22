# Combate e dano

Este arquivo define como uma intenção de combate é convertida em consequência quando o resultado não é evidente.

A regra existe para sustentar tanto declarações amplas quanto ações detalhadas, sem exigir que o JOGADOR coreografe golpe por golpe.

## Princípio

A cena determina primeiro:

- qual capacidade ofensiva realmente está sendo usada;
- qual Perícia ofensiva é aplicável;
- se existe Perícia defensiva capaz de interferir naquela troca;
- qual defesa realmente responde ao mecanismo do ataque.

Só depois disso o cálculo é feito.

> **O cálculo organiza a consequência. A ficção decide quais valores entram nele.**

## Declaração ampla

Uma declaração como:

`Vou até ele e ataco.`

pode representar uma troca inteira de combate.

O NARRADOR não precisa pedir ao JOGADOR cada passo, esquiva ou golpe. Ele usa as capacidades relevantes, resolve a troca e narra uma sequência coerente até surgir um novo ponto real de decisão.

A resolução termina quando a consequência volta a exigir escolha.

## Perícia efetiva

Quando técnica ofensiva e defensiva realmente participam da mesma troca:

`Perícia efetiva = Perícia ofensiva − Perícia defensiva`

Cada ponto de diferença corresponde a `0,2` de patamar no cálculo de dano.

A Perícia efetiva pode ser positiva, zero ou negativa.

Uma técnica defensiva superior pode, portanto, reduzir o dano recebido mesmo quando o ataque consegue entrar: desvio parcial, absorção, rotação com o impacto, proteção de ponto vital, mudança de ângulo ou outra resposta coerente.

A Perícia defensiva só entra quando realmente pode interferir na forma como aquele ataque é recebido.

Uma Perícia de combate não reduz automaticamente uma explosão inevitável, uma queda já consumada ou qualquer outro efeito contra o qual aquela técnica não tenha atuação plausível.

## Ataque efetivo

Para o cálculo de dano:

`Ataque efetivo = Dano + 1 + (Perícia efetiva × 0,2)`

O `+1` é estrutural do lado ofensivo.

Isso significa que um ataque de mesmo patamar da defesa ainda produz consequência relevante, enquanto cada patamar de diferença continua tendo peso crescente.

O valor calculado não altera permanentemente o patamar do Poder, da FOR ou de qualquer outra capacidade da ficha. Ele existe apenas para resolver aquela aplicação de dano.

## Dano aplicado

`Dano aplicado = 2^(Ataque efetivo − Defesa efetiva)`

A progressão é exponencial: cada patamar de diferença dobra ou reduz pela metade o dano.

Sem diferença de Perícia, a referência básica fica:

`Ataque = Defesa → 2` | `Ataque +1 → 4` | `Ataque +2 → 8` | `Ataque +3 → 16` | `Ataque +4 → 32` | `Ataque +5 → 64`

No sentido contrário:

`Ataque -1 → 1` | `Ataque -2 → 0,5` | `Ataque -3 → 0,25` | `Ataque -4 → 0,125`

A diferença de patamar deve pesar. O sistema não corrige artificialmente uma luta apenas para torná-la justa.

## Defesa efetiva

A defesa usada é aquela que realmente responde ao mecanismo do ataque.

`RES` representa resistência natural do corpo e de sua própria natureza: impacto, dor, fadiga, toxinas, doença, temperatura, pressão, falta de ar e efeitos físicos ou mágicos que ataquem diretamente sua integridade, quando aplicáveis.

`VON` responde a resistência mental, emocional ou volitiva.

Proteções externas não aumentam automaticamente `RES`. Elas podem resolver a ameaça por outro mecanismo.

Uma armadura pode interceptar um projétil. Uma máscara pode impedir a inalação de gás. Uma proteção ambiental pode criar condições seguras onde o corpo sozinho não resistiria.

Quando mais de uma proteção existe, o NARRADOR identifica qual delas realmente responde ao ataque. Não há soma automática de camadas.

## Fraqueza e Mortal

Quando aplicáveis à resistência natural:

`Fraqueza: X` → a resistência natural contra X é reduzida à metade, arredondando para baixo.

`Mortal: X` → a resistência natural contra X passa a `[0]`.

Esses TRAÇOS alteram apenas a resistência natural. Proteções externas continuam funcionando se o mecanismo delas ainda for válido.

Reduzir uma defesa não é o mesmo que ignorá-la. Se um efeito ignora uma proteção, aquela proteção simplesmente não participa daquela resolução.

## Ataques detalhados

Uma declaração detalhada não recebe bônus por ser mais bonita ou mais longa.

Ela pode, porém, mudar a situação.

Exemplo:

`Me aproximo e tento acertar o joelho dele pelas costas.`

Se o alvo realmente for pego sem perceber, talvez sua Perícia defensiva não possa participar normalmente. O ataque continua sendo calculado pela mesma regra, mas com apenas as capacidades que a situação permite.

Além disso, o local declarado orienta a consequência.

Acertar o joelho não aumenta automaticamente o patamar de Dano. Pode, entretanto, produzir consequência funcional específica conforme a severidade alcançada: dificuldade para apoiar a perna, mobilidade comprometida, queda ou incapacidade de continuar usando aquele membro.

> **Descrição detalhada não cria bônus gratuito. Ela pode mudar quais defesas se aplicam e onde a consequência acontece.**

## VIDA como referência de acúmulo

Enquanto a consequência permitir desgaste progressivo, o dano acumulado usa a seguinte régua:

`0–4 Ileso | 5 Ferido | 10 Ferido* | 15 Grave | 20 Grave* | 25 Crítico | 30 Crítico* | 35 Incapacitado`

A régua comunica progressão e ajuda o personagem a perceber quando permanecer na luta deixou de ser seguro.

Ela não funciona como proteção contra assimetrias evidentes.

Um resultado muito acima da capacidade de sobrevivência pode saltar etapas. Quando a natureza do ataque e o excesso tornam sobrevivência incoerente, a consequência pode ser imediatamente letal.

`Ataque [5]` contra `Defesa [0]`, sem diferença de Perícia, é tratado como ataque efetivo `[6]` e produz `64` de dano aplicado: mais que toda a referência de `35` para Incapacitado. Se o golpe realmente atinge de forma compatível com sua natureza destrutiva, isso pode representar morte imediata.

## Quantidade e incapacidade

Acúmulo só faz sentido quando cada aplicação consegue produzir alguma consequência real sobre o alvo.

Uma grande quantidade de ataques incapazes não deve vencer automaticamente uma defesa apenas por contabilidade.

> **Quantidade não transforma automaticamente uma ameaça incapaz em uma ameaça capaz.**

Se a ficção mostra que o mecanismo não consegue afetar o alvo, o NARRADOR não precisa acumular frações indefinidamente até fabricar um resultado incoerente.

## Regra de uso

Em combate, o procedimento mínimo é:

`determinar ataque e defesa aplicáveis → calcular Perícia efetiva → calcular Ataque efetivo → calcular Dano aplicado → interpretar a consequência`

Para uma ação simples, isso basta.

> **Ataque, defesa, resultado. O restante existe apenas quando a própria ficção exige mais detalhe.**
