# Vida

Status: APROVADO

Vida representa quanto dano e desgaste físico a personagem consegue suportar antes de ficar Incapacitada.

A Vida Máxima é um valor derivado dos Atributos permanentes da personagem.

---

## 1. Vida Máxima

A fórmula é:

> **Vida = 10 + (Resistência × 4) + (Potência × 2) + (Controle × 2) + Intelecto + Presença + Vontade**

Para esse cálculo, **Atributos negativos contam como 0**.

Isso significa que valores negativos nunca reduzem a Vida abaixo da base por causa do próprio valor negativo.

Exemplo:

```text
Potência [1]
Controle [2]
Resistência [3]
Intelecto [0]
Presença [-1]
Vontade [1]

Vida
= 10 + (3×4) + (1×2) + (2×2) + 0 + 0 + 1
= 29
```

Um personagem com todos os Atributos em `[0]` possui:

> **Vida 10**

---

## 2. Alterações permanentes e temporárias

Quando um Atributo permanente que entra na fórmula mudar, a Vida Máxima deve ser recalculada.

Alterações temporárias de Atributo **não recalculam a Vida Máxima**.

```text
mudança permanente de Atributo
→ recalcula Vida Máxima

mudança temporária de Atributo
→ não recalcula Vida Máxima
```

A Vida atual permanece uma informação de STATUS. A ficha registra o valor máximo ou de referência quando necessário para consulta.

---

## 3. 0 Vida

Ao chegar a:

> **0 Vida**

A personagem fica:

> **Incapacitada**

Incapacitada significa que ela não consegue continuar agindo normalmente naquela situação.

A forma concreta da incapacidade depende da ficção e pode representar, por exemplo:

- inconsciência;
- colapso;
- ferimento grave;
- incapacidade física de continuar;
- outra consequência coerente com o que aconteceu.

> **Chegar a 0 Vida não significa morte automática.**

---

## 4. Vida não substitui consequências evidentes

Vida não funciona como proteção absoluta contra uma situação cuja consequência já seja claramente determinada pela ficção.

Se uma situação for evidentemente letal e não existir mecanismo real para sobreviver a ela, a resolução não precisa fabricar várias aplicações de dano apenas para reduzir a Vida até 0.

Da mesma forma, quando a situação não determina claramente a morte, chegar a 0 Vida significa apenas **Incapacitado**.

```text
consequência evidentemente letal
→ aplicar a consequência coerente

situação não define morte de forma evidente
→ 0 Vida = Incapacitado
```

---

## 5. Dano e proteções

A ordem completa de aplicação de Dano, Defesa, RD e Barreira pertence a `combate-e-dano.md`.

Este arquivo define apenas:

- Vida Máxima;
- quando recalcular seu valor;
- o significado de 0 Vida;
- a relação entre Vida e consequências evidentes da ficção.

A recuperação pertence a `recuperacao-da-vida.md`.

---

## Regra final

> **Vida é derivada dos Atributos permanentes. Atributos negativos contam como 0 para esse cálculo. Chegar a 0 Vida deixa a personagem Incapacitada, mas não determina morte automática. A ficção evidente continua prevalecendo sobre uma redução artificial de pontos.**
