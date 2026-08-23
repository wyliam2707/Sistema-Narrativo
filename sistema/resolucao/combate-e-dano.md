# Combate e dano

Status: APROVADO

Este arquivo define como uma intenção ofensiva é convertida em consequência quando o resultado não é evidente.

A organização temporal do combate pertence a `../operacao/turnos-de-combate.md`.

> **Combate usa turnos simultâneos de 10 segundos. Este arquivo calcula o que acontece dentro desse intervalo.**

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

pode representar toda a troca coerente que caiba naquele turno de 10 segundos.

O JOGADOR não precisa coreografar cada passo, esquiva ou golpe. O NARRADOR julga a intenção junto das demais declarações do mesmo turno e resolve somente aquilo que pode acontecer dentro do intervalo disponível.

Uma declaração como:

`Entro na sala e mato todo mundo.`

estabelece um objetivo amplo, não autorização para atravessar vários turnos. O primeiro turno resolve apenas o que cabe nos 10 segundos compartilhados e nas reações das outras peças.

A sentença termina antes se surgir nova decisão relevante; caso contrário, termina no limite do turno.

## Fonte do Dano

O Dano usa a fonte que realmente produz a agressão.

O corpo pode usar `FIS` como potência física de Dano quando o mecanismo for um golpe corporal coerente.

Uma arma, Poder ou equipamento que possua `Dano [X]` usa o próprio valor de Dano.

Exemplo:

`FIS [2] | Pistola — Dano [1] | Espada Mágica — Dano [3]`

Lê-se:

`golpe corporal → [2] | pistola → [1] | espada → [3]`

As fontes não são somadas automaticamente:

`FIS [2] + Espada Mágica Dano [3] ≠ Dano [5]`

`FIS` continua podendo importar para posição, agarrão, deslocamento, execução física ou outra disputa corporal quando a cena realmente exigir isso, sem aumentar automaticamente o Dano próprio da arma.

> **O corpo usa FIS. O equipamento usa sua própria potência. A Perícia informa quão bem a fonte escolhida é aplicada.**

## Perícia efetiva

Quando técnica ofensiva e defensiva realmente participam da mesma troca:

`Perícia efetiva = Perícia ofensiva − Perícia defensiva`

Cada ponto de diferença corresponde a `0,2` de patamar no cálculo de dano.

A Perícia efetiva pode ser positiva, zero ou negativa.

Uma técnica defensiva superior pode reduzir o dano recebido mesmo quando o ataque consegue entrar: desvio parcial, absorção, rotação com o impacto, proteção de ponto vital, mudança de ângulo ou outra resposta coerente.

A Perícia defensiva só entra quando realmente pode interferir na forma como aquele ataque é recebido.

Uma Perícia de combate não reduz automaticamente uma explosão inevitável, uma queda já consumada ou qualquer outro efeito contra o qual aquela técnica não tenha atuação plausível.

## Ataque efetivo

Para o cálculo de dano:

`Ataque efetivo = Dano + 1 + (Perícia efetiva × 0,2)`

O `+1` é estrutural do lado ofensivo.

Ampliações de Alcance, Alvos, Área ou outra dimensão não reduzem o Ataque efetivo. A configuração escolhida é paga integralmente antes da resolução conforme `consolidacao.md`.

O valor calculado não altera permanentemente o patamar do Poder, do FIS, da arma ou de qualquer outra capacidade da ficha. Ele existe apenas para resolver aquela aplicação de dano.

## Dano aplicado

`Dano aplicado = 2^(Ataque efetivo − Defesa efetiva)`

A progressão é exponencial: cada patamar de diferença dobra ou reduz pela metade o dano.

Sem diferença de Perícia:

`Ataque = Defesa → 2` | `Ataque +1 → 4` | `Ataque +2 → 8` | `Ataque +3 → 16` | `Ataque +4 → 32` | `Ataque +5 → 64`

No sentido contrário:

`Ataque -1 → 1` | `Ataque -2 → 0,5` | `Ataque -3 → 0,25` | `Ataque -4 → 0,125`

A diferença de patamar deve pesar. O sistema não corrige artificialmente uma luta apenas para torná-la justa.

### Dano mínimo contabilizável

`0,25` é o menor Dano mecanicamente acumulável.

`Dano ≥ 0,25 → contabiliza` | `Dano < 0,25 → não contabiliza`

Isso representa o ponto em que uma aplicação ainda consegue produzir desgaste relevante sobre aquela resistência.

A regra não transforma um mecanismo incapaz em ameaça apenas porque o valor alcançou `0,25`. Se a própria ficção mostra que o meio usado não pode afetar o alvo ou a estrutura, não há Dano acumulável.

> **Quantidade não transforma desgaste irrelevante em capacidade destrutiva.**

## Defesa efetiva

A defesa usada é aquela que realmente responde ao mecanismo do ataque.

`RES` representa resistência natural do corpo e de sua própria natureza: impacto, dor, fadiga, toxinas, doença, temperatura, pressão, falta de ar e efeitos físicos ou mágicos que ataquem diretamente sua integridade, quando aplicáveis.

`VON` responde a resistência mental, emocional ou volitiva.

Proteções externas não aumentam automaticamente `RES`. Elas podem resolver a ameaça por outro mecanismo.

Uma armadura pode interceptar um projétil. Uma máscara pode impedir a inalação de gás. Uma proteção ambiental pode criar condições seguras onde o corpo sozinho não resistiria.

Quando mais de uma proteção existe, o NARRADOR identifica qual delas realmente responde ao ataque. Não há soma automática de camadas.

Barreiras e outras proteções com VIDA própria são resolvidas como camadas independentes conforme `escalas-de-efeito.md`.

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

Se o alvo realmente for pego sem perceber, talvez sua Perícia defensiva não possa participar normalmente. O ataque continua sendo calculado pela mesma regra, mas apenas com as capacidades que a situação permite.

Além disso, o local declarado orienta a consequência.

Acertar o joelho não aumenta automaticamente o patamar de Dano. Pode, entretanto, produzir consequência funcional específica conforme a severidade alcançada: dificuldade para apoiar a perna, mobilidade comprometida, queda ou incapacidade de continuar usando aquele membro.

> **Descrição detalhada não cria bônus gratuito. Ela pode mudar quais defesas se aplicam e onde a consequência acontece.**

## VIDA como limite de acúmulo

`VIDA [X]` é o limite de Dano acumulado que a personagem consegue sustentar antes de ficar Incapacitada.

Ela não é derivada de `RES`.

```text
RES → quanto o ataque consegue afetar a personagem
VIDA → quanto Dano relevante ela consegue acumular depois disso
```

Assim, duas peças podem possuir a mesma resistência e durações completamente diferentes em combate.

Exemplo:

```text
Monstro A → RES [4] | VIDA [5]
Monstro B → RES [4] | VIDA [35]
```

Os dois são igualmente difíceis de ferir pelo mesmo mecanismo de ataque. Porém, quando Dano real consegue atravessar a resistência, o primeiro pode cair muito mais cedo.

Quando:

```text
Dano acumulado ≥ VIDA
```

alcança-se `Incapacitado`, salvo se a natureza e o excesso do ataque justificarem consequência ainda mais severa.

A VIDA não possui teto universal. `35` é uma referência comum para heróis, protagonistas e antagonistas centrais, não uma regra para toda criatura. Figurantes e minions podem possuir `VIDA [5]`, `[10]`, `[15]` ou `[20]`; entidades e chefes excepcionais podem possuir `VIDA [50]` ou mais.

O valor da ficha é explícito. Importância e função narrativa podem orientar a duração que a peça precisa sustentar, mas não existe fórmula automática ligando Importância, RES e VIDA.

### Régua heroica de 35

Para personagens com `VIDA [35]`, a régua detalhada continua sendo uma referência útil:

`0–4 Ileso | 5 Ferido | 10 Ferido* | 15 Grave | 20 Grave* | 25 Crítico | 30 Crítico* | 35 Incapacitado`

Personagens com outra VIDA não precisam ser forçados a percorrer essa régua inteira. O controle principal é sempre:

```text
Dano acumulado / VIDA máxima
```

Os rótulos narrativos intermediários podem ser usados quando ajudarem a comunicar gravidade, mas não substituem o limite explícito da ficha.

A VIDA também não funciona como proteção contra assimetrias evidentes.

Um resultado muito acima da capacidade de sobrevivência pode saltar o acúmulo normal. Quando a natureza do ataque e o excesso tornam sobrevivência incoerente, a consequência pode ser imediatamente letal mesmo antes de uma leitura burocrática de etapas.

Exemplo: `Dano [5]` contra `Defesa [0]`, sem diferença de Perícia, é tratado como Ataque efetivo `[6]` e produz `64` de Dano aplicado. Contra `VIDA [35]`, isso ultrapassa toda a referência heroica; contra uma criatura de `VIDA [5]`, o excesso é ainda mais brutal. Se o golpe realmente atinge de forma compatível com sua natureza destrutiva, isso pode representar morte imediata.

## Quantidade e incapacidade

Acúmulo só faz sentido quando cada aplicação consegue produzir alguma consequência real sobre o alvo.

Uma grande quantidade de ataques incapazes não deve vencer automaticamente uma defesa apenas por contabilidade.

> **Quantidade não transforma automaticamente uma ameaça incapaz em uma ameaça capaz.**

Se a ficção mostra que o mecanismo não consegue afetar o alvo, o NARRADOR não acumula frações indefinidamente até fabricar um resultado incoerente.

Como referência matemática, resultados abaixo de `0,25` já são considerados irrelevantes para acúmulo.

## Consolidação do ataque

Dano é normalmente instantâneo. Alcance natural, um alvo e área mínima pertencem à manifestação-base da capacidade.

Quando o ataque amplia Alcance, quantidade de Alvos ou Área, usa as regras de `consolidacao.md`.

A ampliação não divide automaticamente o Dano entre os afetados. Toda Ampliação usada é paga integralmente em Energia antes da resolução.

Depois que o Dano é aplicado, permanece o ferimento na VIDA; o ataque não continua existindo como efeito persistente apenas para representar o Dano já causado.

## Regra de uso

Em combate, para cada aplicação relevante dentro do turno:

`determinar fonte de Dano e defesa aplicável → calcular Perícia efetiva → configurar e pagar Ampliação, se houver → calcular Ataque efetivo → calcular Dano aplicado → acumular contra VIDA → interpretar a consequência`

A quantidade e a precedência das aplicações que realmente cabem nos 10 segundos são julgadas pela situação e por `../operacao/turnos-de-combate.md`; não existe uma economia abstrata de “uma ação”.

> **Turno organiza o tempo. Esta regra calcula o dano.**