# Mobilidade / Imobilizar

Mobilidade altera quanto o alvo consegue se deslocar dentro da natureza do efeito.

## Manifestação-base

`Mobilidade / Imobilizar → Médio / 1 alvo / Pontual / Cena`

## Resolução

Quando houver incerteza real:

`Mobilidade efetiva = patamar de Mobilidade usado + 1 + (Perícia aplicável × 0,2)`

Sem Perícia aplicável:

`Mobilidade efetiva = patamar de Mobilidade usado + 1`

A Resistência efetiva vem daquilo que realmente responde ao mecanismo de restrição ou contenção. Quando outra personagem estiver resistindo ativamente:

`Resistência ativa = Base da oposição + (Suporte da oposição × 0,2)`

Sem Suporte aplicável, usa-se apenas a Base da oposição. Resistência passiva, Poder, proteção, ancoragem ou outro mecanismo coerente usa seu próprio valor aplicável.

`Resultado = 2^(Mobilidade efetiva − Resistência efetiva)`

Ler o maior degrau da escala abaixo que o Resultado alcançar. O Resultado não amplia o repertório do Poder.

## Escala

`[2] Dificultar` | `[4] Restringir` | `[8] Imobilizar` | `[16] Conter` | `[32] Aprisionar`

- `[2]` — mover-se continua possível, mas perde eficiência.
- `[4]` — movimento fortemente limitado; algumas direções ou ações deixam de ser viáveis.
- `[8]` — perde funcionalmente a capacidade de se deslocar.
- `[16]` — tentativas simples de escapar, romper ou contornar deixam de funcionar.
- `[32]` — contenção total dentro da natureza do efeito, exigindo solução ou disputa compatível.

A condição não decide sozinha todas as outras ações possíveis; a cena determina o que ainda é viável.

## Persistência

Depois de estabelecido, o efeito permanece pela Duração escolhida enquanto sua estrutura existir:

`D = patamar de Mobilidade usado + (Perícia aplicável × 0,2)`

`V = maior entre [1] e o Atributo estrutural da Fonte`

O Atributo estrutural vem da natureza real da Fonte; não se escolhe o valor mais vantajoso. O valor de `V` fica fixado na criação da instância.

Enquanto `V > 0`, o efeito funciona integralmente na intensidade alcançada. Ele termina quando sua Duração termina ou quando chega a `V0`, o que acontecer primeiro.

Vida estrutural não é recuperada por Cura, descanso ou regeneração de VIDA comum.

### Reaplicação no mesmo alvo

O mesmo efeito de Mobilidade persistente aplicado novamente ao mesmo alvo consolida uma única instância.

Mesma Duração:

`D consolidada = maior D`

`V consolidada = maior V atual`

Durações diferentes:

`D consolidada = média das duas D`

`V consolidada = média das duas V atuais`

`Duração consolidada = maior Duração`

Da terceira aplicação em diante, comparar a nova aplicação com o estado consolidado atual. Se a instância anterior já chegou a `V0`, uma nova aplicação cria uma nova instância completa.

Ampliações de Alcance, Alvos, Área/Tamanho ou Duração usam `../consolidacao.md`.