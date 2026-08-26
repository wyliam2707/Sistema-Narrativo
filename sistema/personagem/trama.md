# Pontos de Trama

Status: APROVADO

Trama é uma reserva mecânica disponível, por regra geral, apenas para a personagem com:

> **CONTROLE: JOGADOR HUMANO**

A autoridade associada a esse `CONTROLE` pertence a `../personas/`. Este arquivo define somente **a reserva e seus usos mecânicos**.

## Reserva inicial

```text
Trama inicial = 30
```

Trama nunca fica negativa.

O valor atual pertence ao estado persistente, não à ficha consolidada.

## Recuperação diária

A cada novo dia da campanha:

> **+5 Trama**

Além disso, podem ser obtidos até:

> **+5 Trama adicionais por dia**

por complicações reais de Traços voluntariamente aceitas pela personagem elegível.

Cada complicação válida concede normalmente:

> **+1 Trama**

Evitar, resistir ou contornar a complicação não concede esse ponto.

A decisão voluntária continua pertencendo à cadeira definida em `../personas/`.

## Melhorar uma rolagem

Antes de resolver um teste:

```text
5 Trama  → +1d
10 Trama → +2d
```

O limite universal final continua `±2d`, conforme `../resolucao/motor-de-disputa.md`.

## Reduzir penalidade de dados

```text
5 Trama  → reduz penalidade em 1d
10 Trama → reduz penalidade em 2d
```

Isso não torna possível uma ação objetivamente impossível.

## Reduzir Dano

Depois que Defesa, RD e Barreira determinarem quanto Dano realmente alcançaria a personagem e antes de aplicar esse valor à Vida:

> **1 Trama = reduz 1 ponto do Dano restante**

O gasto pode reduzir o Dano a `0`.

A ordem completa pertence a `../resolucao/combate-e-dano.md`.

## Substituir Mana faltante

Quando uma configuração válida de Poder estiver dentro de `[X]`, mas faltar Mana:

> **1 Trama substitui 1 Mana faltante**

Pode-se pagar parte com Mana e somente a diferença com Trama.

Trama não:

- aumenta Patamar;
- aumenta `[X]`;
- permite configuração acima do limite normal;
- cria Poder que a personagem não possui.

## Código

Quando a personagem possuir o Traço **Código** e decidir violá-lo claramente:

> **quebrar o Código custa 5 Trama**

A escolha deve ser informada antes da conclusão quando o custo ainda puder alterar a decisão.

Se houver menos de 5 Trama, perde apenas o que possuir. Ter `0` Trama não impede a violação.

A forma de abrir essa escolha pertence à operação e à autoridade das personas; este arquivo apenas define o custo.

## Limite desta regra

Trama atual **não concede** por regra geral:

- reescrita retroativa de consequência já narrada;
- mudança retroativa de reação social;
- transformação automática de morte em sobrevivência;
- abertura narrativa de possibilidade que não existia;
- correção retroativa de descoberta ou oportunidade perdida.

> **Trama modifica dados, Dano e Mana. Ela não reescreve cânone.**

## Persistência

Registrar a reserva atual conforme:

```text
../persistencia/status.md
../persistencia/estado-atual.md
```

A ficha pode indicar que a personagem é elegível à regra por seu `CONTROLE`, mas não guarda o saldo atual como característica permanente.

## Regra final

> **Trama é um recurso mecânico da personagem humana: melhora dados, reduz penalidades, absorve Dano e substitui Mana dentro de `[X]`. Autoridade e registro pertencem às áreas responsáveis.**
