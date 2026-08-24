# STATUS

Status: APROVADO

STATUS registra **como a peça está agora**.

Ele não redefine mecânicas. Sua função é preservar o estado atual já estabelecido pela ficção e por `../resolucao/`.

```text
FICHA
→ quem a peça é e do que é capaz

STATUS
→ como ela está neste momento
```

## Estrutura básica

Quando relevantes, registrar:

```text
Vida / Dano atual
Energia atual
Condições
Efeitos Ativos
Local / posição relevante
outros estados temporários que ainda possam alterar a continuidade
```

Nem todo campo precisa existir para toda peça.

> **STATUS guarda somente o que ainda pode importar agora.**

## Vida e Energia

STATUS registra apenas os valores atuais já determinados pelas regras correspondentes.

As regras de Dano e VIDA pertencem a `../resolucao/combate-e-dano.md`.

A regra de Cura pertence a `../resolucao/efeitos/cura.md`.

As regras de recuperação natural, Regeneração e Medicina pertencem a `../resolucao/recuperacao-da-vida.md`.

As regras de Energia, Bateria e recuperação pertencem a `../resolucao/energia.md`.

Exemplos de registro:

```text
Dano [12/35]
Energia [53/80]
Energia [55/100] - Bateria [40/40] - Descanso [0]-[45]
```

O STATUS não recalcula esses valores; apenas preserva o resultado atual.

## Condições

Condição descreve um estado temporário relevante da peça.

Exemplos:

```text
Cego
Envenenado
Imobilizado
Exausto
Sangrando
```

Condições não recebem bônus ou penalidades automáticos apenas por possuírem um nome. A consequência vem daquilo que foi realmente estabelecido pela cena e pela resolução.

Nem toda descrição momentânea precisa ser registrada. Só permanece no STATUS aquilo que ainda puder alterar decisões ou resoluções futuras.

## Efeitos Ativos

Efeito Ativo registra uma manifestação temporária que continua existindo ou produzindo consequência.

Preservar no STATUS somente as informações mecânicas que já foram estabelecidas pela regra específica, como Fonte, `D/V`, Duração ou outro dado necessário para continuidade.

O STATUS não define como esses valores são calculados.

Regras de efeitos persistentes, Proteção, Invocação, Fonte e Vida estrutural pertencem a `../resolucao/`.

Evitar duplicação: se um único registro já descreve adequadamente o estado relevante, não criar outra entrada dizendo a mesma coisa.

## Localização

Local registra onde a peça está apenas no nível necessário para evitar confusão de continuidade ou alterar uma resolução futura.

```text
Local: Biblioteca do Castelo
Local: Telhado da Torre Norte
Local: corredor, junto à saída
```

Posição exata só precisa ser registrada enquanto continuar relevante.

## Entrada, mudança e saída

STATUS possui três operações:

```text
ENTRA
→ um novo estado relevante passa a existir.

MUDA
→ um estado existente se altera de forma relevante.

SAI
→ o estado deixa de existir ou deixa de importar.
```

Quando algo deixa de ser relevante, remover do STATUS em vez de manter histórico.

## Atualização imediata

Assim que uma consequência é estabelecida, o STATUS é atualizado.

Energia muda quando o custo é efetivamente pago. Dano ou Cura alteram o valor atual quando resolvidos. Condições e Efeitos Ativos entram, mudam ou saem quando a cena estabelece isso.

> **Resolveu, atualizou. STATUS representa o presente.**

## Autoridade

STATUS registra fatos estabelecidos, nunca intenções, previsões ou resultados ainda não resolvidos.

```text
JOGADORES / OPOSITOR
→ declaram intenções conforme sua autoridade.

NARRADOR
→ julga o que se torna verdade.

PERSISTÊNCIA
→ registra o resultado atual.
```

Uma declaração por si só não altera STATUS.

## Fronteiras

STATUS não substitui:

```text
FICHA
→ capacidades e informações consolidadas da peça.

RESOLUÇÃO
→ regras que determinam resultados e valores.

LIVRO
→ histórico do que aconteceu.

PROGRESSÃO
→ fatos passados que continuam causalmente vivos.
```

> **STATUS não explica a regra. Ele guarda o resultado atual da regra e da ficção.**