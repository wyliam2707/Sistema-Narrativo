# Rotina de Trama em Combate

Status: APROVADO

Este arquivo define **quando a decisão de usar Trama deve obrigatoriamente ser aberta ao JOGADOR HUMANO durante combate**.

A reserva e os custos de Trama pertencem a `../personagem/trama.md`. Este arquivo define somente a rotina operacional.

> **A checagem de Trama é obrigatória sempre que uma janela válida de gasto surgir.**

## Princípio

O NARRADOR não gasta Trama pelo jogador e não presume que ele deseja economizá-la.

Quando uma resolução alcançar um ponto em que Trama pode legitimamente alterar o resultado, a sequência deve parar antes desse ponto e devolver a decisão ao JOGADOR HUMANO.

```text
janela válida de Trama
→ gasto já foi declarado?
→ sim: aplicar e continuar
→ não: abrir decisão ao JOGADOR HUMANO
→ receber resposta
→ registrar gasto, se houver
→ continuar a resolução
```

A rotina é obrigatória. O gasto continua opcional.

## 1. Trama antes de uma rolagem

Quando o JOGADOR HUMANO estiver prestes a fazer uma rolagem que possa receber Trama:

```text
declaração
→ configuração, se houver
→ NARRADOR determina rolagem, Atributo, modificadores e alvo
→ abrir decisão de Trama
→ jogador decide
→ aplicar gasto, se houver
→ rolar
→ resolver
```

Forma visível preferida:

```text
Acerto: 4d6 + CON [1] | DF [16]
Trama: 30/30 — usar Trama?
```

Se o jogador já tiver declarado o gasto junto da ação, não perguntar novamente.

O NARRADOR nunca rola primeiro para depois oferecer Trama de melhoria daquele teste.

## 2. Trama para substituir Mana

Quando um Poder estiver validamente configurado dentro de `[X]`, mas a Mana disponível não cobrir o custo:

```text
configuração válida
→ custo conhecido
→ Mana insuficiente
→ calcular Mana faltante
→ abrir decisão de Trama
→ jogador decide quanto substituir
→ pagar Mana + Trama
→ resolver
```

Forma visível preferida:

```text
Custo: 4 Mana | Mana: 2/18 | faltam 2
Trama: 30/30 — substituir Mana com Trama?
```

Trama não pode tornar válida uma configuração acima de `[X]`.

Se houver Mana suficiente, esta janela não existe.

## 3. Trama para reduzir Dano

Sempre que Dano realmente alcançar a etapa em que seria aplicado à Vida do JOGADOR HUMANO:

```text
Dano bruto
→ redução da Defesa, quando houver
→ RD
→ mínimo final, quando aplicável
→ Escudo
→ determinar Dano restante
→ abrir decisão de Trama
→ jogador decide
→ reduzir Dano com Trama, se houver
→ aplicar restante à Vida
```

Forma visível preferida:

```text
Dano à Vida: 7
Vida: 8/20 | Trama: 30/30
Usar Trama para reduzir o Dano?
```

O NARRADOR não reduz a Vida antes dessa decisão.

Se nenhum Dano alcançar a Vida, esta janela não existe.

## 4. Quando não perguntar

Não criar uma pergunta de Trama quando:

- o jogador já declarou claramente o gasto aplicável;
- a personagem está com `0` Trama e aquele uso exige gasto positivo;
- não existe uso de Trama válido naquele ponto;
- a resolução já passou legitimamente da janela de uso;
- a ação é de outra peça e não produz uma janela de Trama para o JOGADOR HUMANO.

Isso não torna a rotina opcional. Significa apenas que a checagem concluiu que não existe decisão real a apresentar.

## 5. Não agrupar janelas diferentes

Uma decisão de Trama vale somente para a janela em que foi declarada.

```text
Trama usada para pagar Mana
≠ autorização para melhorar a rolagem

Trama usada para melhorar a rolagem
≠ autorização para reduzir Dano depois
```

Se uma mesma sequência produzir mais de uma janela válida, cada uma é tratada no seu ponto causal.

## 6. Registro imediato

Todo gasto de Trama é registrado assim que for confirmado.

```text
jogador declara gasto
→ reduzir Trama atual
→ aplicar efeito do gasto
→ continuar resolução
```

A HUD e qualquer apresentação posterior usam o novo saldo.

## Atalho obrigatório

```text
ANTES DE ROLAR
→ checar Trama

MANA FALTANTE EM CONFIGURAÇÃO VÁLIDA
→ checar Trama

DANO PRESTES A ATINGIR VIDA
→ checar Trama
```

> **Não avançar além de uma janela válida de Trama sem que o JOGADOR HUMANO tenha tido a oportunidade de decidir.**

## Regra final

> **Em combate, Trama possui uma rotina obrigatória de decisão. Antes de uma rolagem elegível, diante de Mana faltante em uma configuração válida e antes de Dano restante atingir a Vida, o fluxo para e oferece a escolha ao JOGADOR HUMANO. A rotina é obrigatória; gastar Trama nunca é.**
