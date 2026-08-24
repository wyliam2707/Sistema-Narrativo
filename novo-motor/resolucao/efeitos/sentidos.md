# Sentidos — supressão

Sentidos reduz ou elimina a capacidade funcional de perceber por um sentido afetável pelo Poder.

## Manifestação-base

`Sentidos → Médio / 1 alvo / Pontual / Cena`

## Resolução

Quando houver incerteza real:

`Sentidos efetivo = patamar de Sentidos usado + 1 + (Perícia aplicável × 0,2)`

Sem Perícia aplicável:

`Sentidos efetivo = patamar de Sentidos usado + 1`

A Resistência efetiva vem daquilo que realmente responde à supressão sensorial. Quando outra personagem estiver resistindo ativamente:

`Resistência ativa = Base da oposição + (Suporte da oposição × 0,2)`

Sem Suporte aplicável, usa-se apenas a Base da oposição. Resistência passiva, sentido extraordinário, Poder, proteção ou outro mecanismo coerente usa seu próprio valor aplicável.

`Resultado = 2^(Sentidos efetivo − Resistência efetiva)`

Ler o maior degrau da escala abaixo que o Resultado alcançar. O Resultado não amplia o repertório do Poder.

## Escala

`[2] Prejudicar` | `[4] Comprometer` | `[8] Suprimir` | `[16] Supressão ampla` | `[32] Supressão dominante`

- `[2]` — o sentido funciona com dificuldade relevante.
- `[4]` — o sentido perde informação importante.
- `[8]` — o sentido deixa de fornecer informação funcional.
- `[16]` — sentido principal em `[8]` e demais sentidos afetáveis em `[2]`.
- `[32]` — sentido principal em `[8]` e demais sentidos afetáveis em `[4]`.

Depois de `[8]`, o efeito não torna o sentido “mais suprimido”; resultados maiores espalham a interferência para funções relacionadas.

## Persistência

Depois de estabelecido, o efeito permanece pela Duração escolhida enquanto sua estrutura existir:

`D = patamar de Sentidos usado + (Perícia aplicável × 0,2)`

`V = maior entre [1] e o Atributo estrutural da Fonte`

O Atributo estrutural vem da natureza real da Fonte; não se escolhe o valor mais vantajoso. O valor de `V` fica fixado na criação da instância.

Enquanto `V > 0`, o efeito funciona integralmente na intensidade alcançada. Ele termina quando sua Duração termina ou quando chega a `V0`, o que acontecer primeiro.

Vida estrutural não é recuperada por Cura, descanso ou regeneração de VIDA comum.

### Reaplicação no mesmo alvo

O mesmo efeito de Sentidos persistente aplicado novamente ao mesmo alvo consolida uma única instância.

Mesma Duração:

`D consolidada = maior D`

`V consolidada = maior V atual`

Durações diferentes:

`D consolidada = média das duas D`

`V consolidada = média das duas V atuais`

`Duração consolidada = maior Duração`

Da terceira aplicação em diante, comparar a nova aplicação com o estado consolidado atual. Se a instância anterior já chegou a `V0`, uma nova aplicação cria uma nova instância completa.

Ampliações de Alcance, Alvos, Área/Tamanho ou Duração usam `../consolidacao.md`.