# Emoção

Emoção altera o estado emocional dentro do repertório do Poder.

## Manifestação-base

`Emoção → Médio / 1 alvo / Pontual / Cena`

## Resolução

Quando houver incerteza real:

`Emoção efetiva = patamar de Emoção usado + 1 + (Perícia aplicável × 0,2)`

Sem Perícia aplicável:

`Emoção efetiva = patamar de Emoção usado + 1`

A Resistência efetiva vem daquilo que realmente responde ao mecanismo emocional. Quando outra personagem estiver resistindo ativamente:

`Resistência ativa = Base da oposição + (Suporte da oposição × 0,2)`

Sem Suporte aplicável, usa-se apenas a Base da oposição. Resistência passiva, proteção, Poder ou outro mecanismo coerente usa seu próprio valor aplicável.

`Resultado = 2^(Emoção efetiva − Resistência efetiva)`

Ler o maior degrau da escala abaixo que o Resultado alcançar. O Resultado não amplia o repertório do Poder.

## Escala

`[2] Distorcer` | `[4] Ocultar ou Criar` | `[8] Substituir` | `[16] Construir Estado` | `[32] Realidade Emocional`

- `[2]` — altera intensidade ou direção de uma emoção existente.
- `[4]` — suprime uma emoção presente ou cria uma nova.
- `[8]` — substitui uma emoção por outra.
- `[16]` — combina várias respostas emocionais em um estado coerente.
- `[32]` — reconstrói amplamente a experiência emocional dentro do repertório.

Emoção altera o que o alvo sente. Controle altera ou impõe o que ele faz.

## Persistência

Depois de estabelecido, o efeito permanece pela Duração escolhida enquanto sua estrutura existir:

`D = patamar de Emoção usado + (Perícia aplicável × 0,2)`

`V = maior entre [1] e o Atributo estrutural da Fonte`

O Atributo estrutural vem da natureza real da Fonte; não se escolhe o valor mais vantajoso. O valor de `V` fica fixado na criação da instância.

Enquanto `V > 0`, o efeito funciona integralmente na intensidade alcançada. Ele termina quando sua Duração termina ou quando chega a `V0`, o que acontecer primeiro.

Vida estrutural não é recuperada por Cura, descanso ou regeneração de VIDA comum.

### Reaplicação no mesmo alvo

O mesmo efeito de Emoção persistente aplicado novamente ao mesmo alvo consolida uma única instância.

Mesma Duração:

`D consolidada = maior D`

`V consolidada = maior V atual`

Durações diferentes:

`D consolidada = média das duas D`

`V consolidada = média das duas V atuais`

`Duração consolidada = maior Duração`

Da terceira aplicação em diante, comparar a nova aplicação com o estado consolidado atual. Se a instância anterior já chegou a `V0`, uma nova aplicação cria uma nova instância completa.

Ampliações de Alcance, Alvos, Área/Tamanho ou Duração usam `../consolidacao.md`.