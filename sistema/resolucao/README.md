# Resolução

Status: APROVADO

Esta pasta responde à pergunta:

> **Dadas as capacidades, circunstâncias e oposição, qual é o resultado mecânico?**

`resolucao/` contém regras de cálculo e interpretação mecânica. Ela não distribui autoridade, não organiza a sequência da mesa, não escreve a cena e não decide onde salvar o resultado.

## Estrutura

- `principio-de-resolucao.md` — quando estabelecer diretamente, quando testar e como tratar impossibilidade;
- `leitura-da-ficha-na-resolucao.md` — quais partes da ficha entram numa resolução;
- `motor-de-disputa.md` — motor universal contra cenário e oposição ativa;
- `combate-e-dano.md` — ataque, Defesa, Dano, RD, Barreira, Trama e Vida;
- `vida.md` — Vida Máxima e Incapacitado;
- `recuperacao-da-vida.md` — recuperação natural e Medicina;
- `mana.md` — Mana Máxima, recuperação e `[X]`;
- `poderes/` — Hubs e mecânicas concretas de Poder;
- `status/` — condições temporárias e sobreposição;
- `resolucao-social.md` — incerteza social sem substituir agência;
- `informacao-e-investigacao.md` — informação, repertório e investigação.

A sequência operacional de combate pertence a `../operacao/ordem-de-resolucao-do-combate.md`.

## Entrada

```text
RESULTADO EVIDENTE
→ estabelecer

IMPOSSIBILIDADE EVIDENTE
→ estabelecer

INCERTEZA REAL
→ aplicar somente a resolução necessária
```

A resolução não fabrica dúvida quando o resultado já está claro.

## Motor universal

Todo teste termina com:

> **resultado de 4 dados mantidos + Atributo**

```text
normal → 4d6, mantém 4
+1d    → 5d6, mantém 4 melhores
+2d    → 6d6, mantém 4 melhores
-1d    → 5d6, mantém 4 piores
-2d    → 6d6, mantém 4 piores
```

Bônus e penalidades se cancelam. O modificador final não ultrapassa `-2d` a `+2d`.

Perícia relevante concede `+1d`; várias Perícias aplicáveis continuam concedendo no máximo `+1d` por Perícias.

Outros dados vêm apenas de regras explícitas, como Poder, Status, Traço, Trama ou outra fonte que determine `+Xd/-Xd`.

## Contra o cenário

```text
4 dados mantidos + Atributo
×
Dificuldade
```

A Dificuldade varia normalmente de `10` a `24`.

```text
resultado ≥ Dificuldade → sucesso
resultado < Dificuldade → falha
```

A Dificuldade descreve a tentativa concreta, incluindo circunstâncias comuns que realmente a tornam mais fácil ou difícil.

Não acompanha Patamar e não é ajustada para balancear personagens.

> **A Dificuldade descreve o problema. A ficha descreve quem tenta resolvê-lo.**

## Oposição ativa

```text
4 dados mantidos + Atributo
×
4 dados mantidos + Atributo
```

Cada lado usa o Atributo coerente com sua própria ação ou reação.

Quando um lado possui vantagem ficcional **óbvia e inegável** naquela oposição:

> **+1d ao lado favorecido**

Se a vantagem já tornar o resultado evidente, não se rola.

Em empate, vence quem iniciou a ação; a resposta precisa superar o iniciador para impedi-lo.

## Tarefas demoradas

Tempo por si só não cria várias rolagens nem barra de progresso.

```text
resultado evidente com tempo suficiente
→ estabelecer resultado e tempo coerente

impossibilidade evidente
→ estabelecer impossibilidade

incerteza real
→ uma resolução adequada
```

Nova rolagem só existe se surgir nova incerteza relevante.

## Combate

A mecânica de ataque, Defesa e Dano pertence a `combate-e-dano.md`.

A ordem da mesa durante combate pertence a:

```text
../operacao/turnos-de-combate.md
../operacao/ordem-de-resolucao-do-combate.md
```

`resolucao/` não cria iniciativa, fila fixa, HUD ou economia universal de ações.

## Poderes

A posse de Poderes pertence a `../personagem/poderes.md`.

A mecânica concreta pertence a `poderes/`.

Cada Hub define somente as dimensões necessárias ao Poder; `[X]` representa Patamar e normalmente limita o máximo de Mana por uso.

## Status

`status/` define as condições mecânicas temporárias.

`../persistencia/` apenas registra quais condições continuam ativas; não recalcula seus efeitos.

## Fronteiras

```text
quem a personagem é?            → ../personagem/
quem decide?                     → ../personas/
como vontades continuam?         → ../agencia/
em que ordem aplicar?            → ../operacao/
como apresentar?                 → ../narracao/
o que permanece?                 → ../persistencia/
como calcular?                   → resolucao/
```

## Regra final

> **`resolucao/` existe para determinar resultados mecânicos quando a ficção ainda deixa mais de uma possibilidade plausível. Todo procedimento de mesa permanece em `operacao/`.**
