# Resolução

Status: APROVADO

Esta pasta responde à pergunta:

> **Dadas as intenções, capacidades, circunstâncias e oposição, como descobrimos o que acontece?**

`resolucao/` calcula e interpreta resultados. Ela não decide quem controla uma peça, não organiza a ordem das cadeiras e não define como a cena é escrita.

---

## Estrutura principal

- `principio-de-resolucao.md` — quando estabelecer diretamente, quando testar e como tratar impossibilidade;
- `leitura-da-ficha-na-resolucao.md` — como identificar Atributo, Perícia, meio, situação e oposição aplicáveis;
- `motor-de-disputa.md` — motor universal contra cenário e oposição ativa;
- `combate-e-dano.md` — ataque, Defesa, Dano, RD, Barreira e aplicação em Vida;
- `vida.md` — Vida Máxima e Incapacitado;
- `recuperacao-da-vida.md` — recuperação natural e Medicina;
- `mana.md` — Mana Máxima, recuperação e `[X]`;
- `poderes/` — Hubs e regras concretas dos Poderes;
- `status/` — famílias de condições temporárias e sobreposição;
- `ordem-de-resolucao-do-combate.md` — ordem operacional de consulta durante combate;
- `resolucao-social.md` — resolução social sem substituir agência;
- `informacao-e-investigacao.md` — informação, repertório e investigação.

Traços e Trama pertencem à definição mecânica da personagem em `../personagem/`, embora possam modificar uma resolução quando suas regras disserem isso explicitamente.

---

## Entrada

```text
RESULTADO EVIDENTE
→ estabelecer

IMPOSSIBILIDADE EVIDENTE
→ estabelecer

INCERTEZA REAL
→ usar somente a regra necessária
```

A resolução não fabrica dúvida quando o resultado já está claro.

---

## Motor universal

Todo teste termina com o resultado de **4 dados mantidos + Atributo**.

Teste normal:

```text
4d6 + Atributo
```

Bônus:

```text
+1d → rola 5d6 e mantém os 4 melhores
+2d → rola 6d6 e mantém os 4 melhores
```

Penalidades:

```text
-1d → rola 5d6 e mantém os 4 piores
-2d → rola 6d6 e mantém os 4 piores
```

Bônus e penalidades se cancelam antes da rolagem. O modificador final nunca ultrapassa `-2d` a `+2d`.

Perícia relevante concede `+1d`. Várias Perícias aplicáveis continuam concedendo no máximo `+1d`.

Dados adicionais ou removidos vêm de fontes mecânicas explícitas, como Perícia, Poder, Status, Traço, Trama ou outra regra que diga diretamente `+Xd` ou `-Xd`.

---

## Contra o cenário

Quando a incerteza vem de uma dificuldade fixa da situação:

```text
4 dados mantidos + Atributo × Dificuldade
```

A Dificuldade varia normalmente de `10` a `24`.

```text
resultado ≥ Dificuldade → sucesso
resultado < Dificuldade → falha
```

Igualar a Dificuldade é sucesso.

A Dificuldade representa a realidade concreta da tentativa, não o Patamar da campanha nem uma tentativa de balanceamento.

Circunstâncias comuns da cena podem aumentar ou reduzir a Dificuldade quando realmente alterarem a tarefa. Não existe incremento fixo obrigatório: o NARRADOR escolhe o valor que melhor represente a situação.

> **A Dificuldade descreve o problema. A ficha descreve quem tenta resolvê-lo.**

---

## Oposição ativa

Quando outra personagem ou entidade se opõe ativamente:

```text
4 dados mantidos + Atributo
×
4 dados mantidos + Atributo
```

Cada lado usa o Atributo coerente com sua própria ação ou reação.

Quando a ficção conceder a um lado uma vantagem **óbvia e inegável** naquela oposição, esse lado recebe `+1d`.

Se a vantagem já tornar o resultado evidente, não se rola.

Em oposição, empate favorece quem iniciou a ação. A resposta precisa superar o resultado da ação para impedi-la.

---

## Tarefas demoradas

O antigo sistema de `Exigência`, `Progresso por aplicação` e `Aplicações necessárias` não faz parte do motor atual.

Uma tarefa não recebe várias rolagens apenas porque demora.

```text
resultado evidente com tempo suficiente
→ estabelecer resultado e tempo coerente

impossibilidade evidente
→ estabelecer a impossibilidade

incerteza real contra a situação
→ um teste contra Dificuldade

oposição ativa
→ uma oposição comum quando necessário
```

Rolagens adicionais só existem quando a ficção cria uma nova incerteza relevante depois da resolução anterior.

---

## Combate

Quando houver combate, consultar:

```text
ordem-de-resolucao-do-combate.md
```

Atalho operacional:

```text
HUD
→ declaração
→ escolhas mecânicas realmente faltantes
→ demais declarações
→ julgar interferência e precedência
→ resolver
→ atualizar
→ novo HUD
```

A simultaneidade e o intervalo de até 10 segundos pertencem a `../operacao/turnos-de-combate.md`.

`resolucao/` não cria iniciativa, fila fixa nem economia universal de uma ação por turno.

---

## Poderes

Para uso configurável ou capacidade extraordinária, consultar `poderes/`.

O Hub individual substitui a antiga regra universal de Ampliação. Não existe mais uma fórmula geral `patamar + Ampliação` aplicada a todos os efeitos.

Mana é o recurso técnico universal de Poderes e `[X]` é igual ao Patamar da personagem.

---

## Status

Condições temporárias mecânicas pertencem a `status/`.

Dentro da mesma família, vale o efeito mais forte conforme a regra de sobreposição. Famílias diferentes podem coexistir.

Persistência apenas registra o Status ativo; não recalcula sua mecânica.

---

## Fronteiras

```text
quem decide?                    → ../personas/
quem move oposição?             → ../personas/opositor/
ordem e turnos?                 → ../operacao/
como mostrar o resultado?       → ../narracao/
o que permanece depois?         → ../persistencia/
quem a personagem é?            → ../personagem/
como calcular o resultado?      → resolucao/
```

## Princípios finais

> **A ficção decide se existe teste, qual Atributo é pertinente e qual é a dificuldade real.**

> **A resolução usa o menor número possível de rolagens.**

> **Importância dramática e Patamar não alteram artificialmente a Dificuldade.**
