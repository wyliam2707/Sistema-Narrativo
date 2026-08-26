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
Vida atual / máxima
Mana atual / máxima
Status e condições temporárias
Efeitos Ativos
Barreiras atuais
alterações temporárias de Atributo
Local / posição relevante
outros estados temporários que ainda possam alterar a continuidade
```

Nem todo campo precisa existir para toda peça.

> **STATUS guarda somente o que ainda pode importar agora.**

## Vida e Mana

STATUS registra apenas os valores atuais já determinados pelas regras correspondentes.

As regras de Vida e incapacidade pertencem a:

```text
../resolucao/vida.md
```

As regras de Dano pertencem a:

```text
../resolucao/combate-e-dano.md
```

A recuperação natural e Medicina pertencem a:

```text
../resolucao/recuperacao-da-vida.md
```

A regra de Mana e recuperação pertence a:

```text
../resolucao/mana.md
```

Exemplo:

```text
Vida [18/29]
Mana [9/24]
```

`ENERGIA` e `Bateria [1–5]` são nomenclaturas/regras legadas e não devem ser usadas em novos registros universais.

O STATUS não recalcula Vida ou Mana; apenas preserva o resultado atual.

## Status e condições

Status nocivos, condições e outros estados temporários descrevem aquilo que continua mecanicamente ou ficcionalmente relevante.

Exemplos possíveis:

```text
Cego
Imóvel
Apavorado
Exausto
Atordoado
Caído
```

A consequência vem da regra que criou o Status ou daquilo que foi estabelecido pela cena.

Nem toda descrição momentânea precisa ser registrada. Só permanece no STATUS aquilo que ainda puder alterar decisões ou resoluções futuras.

Quando a migração das famílias de Status estiver concluída, suas regras específicas passam a ser a fonte mecânica; persistência continua apenas registrando o estado atual.

## Efeitos Ativos

Efeito Ativo registra uma manifestação temporária que continua existindo ou produzindo consequência.

Preservar somente as informações necessárias para continuidade, como:

- origem ou Poder responsável;
- duração restante;
- configuração que continue relevante;
- alvo ou área;
- valor de Barreira;
- alteração temporária de Atributo;
- outro dado necessário.

O STATUS não define como esses valores são calculados.

## Barreiras

Quando uma Barreira precisar persistir entre resoluções, registrar seus PV atuais.

Exemplo:

```text
Barreira [7/15]
```

A criação e o cálculo da Barreira pertencem à regra que a produziu.

## Alterações temporárias de Atributo

Quando um Atributo estiver temporariamente diferente de seu valor permanente e isso ainda importar, registrar a alteração no STATUS.

Exemplo:

```text
Potência +2 temporário — Cena
Controle -1 temporário — 3 Turnos
```

Essas alterações não recalculam Vida Máxima ou Mana Máxima.

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
→ um novo estado relevante passa a existir

MUDA
→ um estado existente se altera de forma relevante

SAI
→ o estado deixa de existir ou deixa de importar
```

Quando algo deixa de ser relevante, remover do STATUS em vez de manter histórico.

## Atualização imediata

Assim que uma consequência é estabelecida, o STATUS é atualizado.

Mana muda quando um custo é efetivamente pago. Vida muda quando Dano ou recuperação são resolvidos. Status, Barreiras e Efeitos Ativos entram, mudam ou saem quando a cena estabelece isso.

> **Resolveu, atualizou. STATUS representa o presente.**

## Autoridade

STATUS registra fatos estabelecidos, nunca intenções, previsões ou resultados ainda não resolvidos.

```text
JOGADORES / OPOSITOR
→ declaram intenções conforme sua autoridade

NARRADOR
→ julga o que se torna verdade

PERSISTÊNCIA
→ registra o resultado atual
```

Uma declaração por si só não altera STATUS.

## Fronteiras

STATUS não substitui:

```text
FICHA
→ capacidades e informações consolidadas da peça

RESOLUÇÃO
→ regras que determinam resultados e valores

LIVRO
→ histórico do que aconteceu

PROGRESSÃO
→ fatos passados que continuam causalmente vivos
```

> **STATUS não explica a regra. Ele guarda o resultado atual da regra e da ficção.**
