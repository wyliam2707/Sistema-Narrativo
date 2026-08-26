# STATUS

Status: APROVADO

STATUS registra **como a peça está agora**.

Ele não redefine mecânicas. Sua função é preservar o estado atual já estabelecido pela ficção e pelas regras apropriadas.

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
Trama atual, somente quando a peça possuir essa reserva
Status e condições temporárias
Efeitos Ativos
Barreiras atuais
alterações temporárias de Atributo
Local / posição relevante
outros estados temporários que ainda possam alterar a continuidade
```

Nem todo campo precisa existir para toda peça.

> **STATUS guarda somente o que ainda pode importar agora.**

---

## Vida, Mana e Trama

STATUS registra apenas os valores atuais já determinados pelas regras correspondentes.

Fontes mecânicas:

```text
Vida e incapacidade
→ ../resolucao/vida.md

Dano
→ ../resolucao/combate-e-dano.md

recuperação natural e Medicina
→ ../resolucao/recuperacao-da-vida.md

Mana e recuperação
→ ../resolucao/mana.md

Trama do protagonista humano
→ ../personagem/trama.md
```

Exemplo:

```text
Vida [18/29]
Mana [9/24]
Trama [27]
```

Trama só aparece quando a personagem realmente possuir essa reserva pelas regras aplicáveis.

`ENERGIA` e `Bateria [1–5]` não são campos universais do motor atual.

O STATUS não recalcula Vida, Mana ou Trama; apenas preserva seus valores atuais.

---

## Status e condições

As famílias mecânicas de Status pertencem a:

```text
../resolucao/status/
```

O STATUS persistente apenas registra quais condições continuam ativas e, quando necessário, sua duração ou outra informação operacional.

Exemplos:

```text
Cego — Cena
Imóvel — 2 Turnos
Apavorado — Cena
Atordoado — 1 Turno
Caído
```

Nem toda descrição momentânea precisa ser registrada. Só permanece no STATUS aquilo que ainda puder alterar decisões, continuidade ou resoluções futuras.

---

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

---

## Barreiras

Quando uma Barreira precisar persistir entre resoluções, registrar seus PV atuais.

```text
Barreira [7/15]
```

A criação e o cálculo da Barreira pertencem à regra que a produziu.

---

## Alterações temporárias de Atributo

Quando um Atributo estiver temporariamente diferente de seu valor permanente e isso ainda importar, registrar a alteração.

```text
Potência +2 temporário — Cena
Controle -1 temporário — 3 Turnos
```

Essas alterações não recalculam Vida Máxima ou Mana Máxima.

---

## Localização

Local registra onde a peça está apenas no nível necessário para evitar confusão de continuidade ou alterar uma resolução futura.

```text
Local: Biblioteca do Castelo
Local: Telhado da Torre Norte
Local: corredor, junto à saída
```

Posição exata só precisa ser registrada enquanto continuar relevante.

---

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

---

## Atualização imediata

Assim que uma consequência é estabelecida, o STATUS é atualizado.

Mana muda quando um custo é efetivamente pago. Trama muda quando é gasta ou recebida. Vida muda quando Dano ou recuperação são resolvidos. Status, Barreiras e Efeitos Ativos entram, mudam ou saem quando a cena estabelece isso.

> **Resolveu, atualizou. STATUS representa o presente.**

---

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

---

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
