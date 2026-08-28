# Exemplo Operacional do Mestre

Status: REFORMULAÇÃO / NÃO IMPLEMENTADO

Este arquivo demonstra o fluxo do `NARRADOR` sem criar regra nova.

## Exemplo 1 — intenção longa interrompida por outra personagem

Situação estabelecida:

```text
Helena está no escritório.
Raul está em casa.
Raul possui rotina e objetivos próprios.
```

Jogador Humano:

```text
Helena
→ vou estudar estes documentos durante a semana.
```

Isso estabelece:

```text
INTENÇÃO
→ estudar.

HORIZONTE MÁXIMO
→ uma semana.
```

Não estabelece que uma semana inteira passará.

Cinco minutos depois, Raul possui motivo próprio para entrar no escritório e conversar.

O Narrador cruza as intenções:

```text
Helena
→ continua estudando.

Raul
→ entra com café e inicia uma conversa.
```

Sentença possível:

> Helena mal havia avançado algumas páginas quando Raul apareceu à porta com duas canecas. Ele deixou uma delas perto dos documentos e puxou a cadeira do outro lado da mesa.
>
> — Preciso falar com você sobre ontem.

O Narrador para ali.

```text
TEMPO PASSADO
→ cerca de 5 minutos.

NOVA DECISÃO HUMANA
→ responder, ignorar, continuar estudando ou outra escolha.
```

Não narrar automaticamente que Helena fecha os documentos ou aceita conversar.

---

## Exemplo 2 — declaração humana não fixa outra personagem

Situação:

```text
Helena acredita que Raul está no quarto.
Raul possui autonomia própria.
```

Jogador Humano:

```text
→ vou ao quarto e abraço Raul.
```

A declaração significa:

```text
Helena pretende ir ao quarto
+
se houver oportunidade
→ pretende abraçá-lo.
```

O Narrador primeiro confere o estado real.

Se Raul já saiu legitimamente antes, a sentença pode ser:

> Helena atravessou o corredor e abriu a porta. O quarto estava vazio.

Isso não contradiz a declaração: o pressuposto de que Raul ainda estava lá nunca foi fato estabelecido.

Também não seria válido decidir retroativamente que Raul saiu apenas porque a IA leu que Helena queria encontrá-lo.

---

## Exemplo 3 — capacidade secreta não altera decisão alheia

Situação:

```text
Raul quer esconder onde esteve.
Raul não sabe que Helena consegue detectar mentiras.
```

Jogador IA — Raul:

```text
→ digo que passei a noite em casa.
```

A IA técnica sabe que Helena possui detecção de mentiras, mas Raul não sabe.

Portanto sua decisão permanece.

Depois:

```text
NARRADOR
→ verifica se a detecção de Helena se aplica.
→ resolve percepção ou efeito necessário.
```

Nunca fazer:

```text
IA sabe que Helena detectará a mentira
→ Raul decide subitamente não mentir.
```

---

## Exemplo 4 — meio próprio

Situação:

```text
Raul quer chegar ao observatório.
Raul possui teleporte.
Helena também consegue abrir portais.
```

Se Raul não possui motivo para depender de Helena:

```text
JOGADOR IA — Raul
→ pode usar seu próprio teleporte.
```

Não transformar automaticamente a personagem em alguém que espera Helena resolver apenas porque ela é a protagonista humana.

Esperar ou pedir ajuda continua possível quando isso nascer de um motivo real de Raul.

## Fluxo resumido

```text
INTENÇÕES + ESTADO
→ conferir pressupostos
→ preservar decisões independentes
→ julgar possibilidade e oposição
→ resolver somente o necessário
→ cruzar tudo no tempo
→ parar na primeira nova decisão humana
→ narrar
→ registrar
```

> **O exemplo correto preserva duas autonomias ao mesmo tempo: o mundo não espera o protagonista, e o Narrador não decide pelo protagonista.**
