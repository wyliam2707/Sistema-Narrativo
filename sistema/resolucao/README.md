# Resolução

Status: APROVADO

Esta pasta responde à pergunta:

> **Dadas as intenções, capacidades, circunstâncias e oposição, como descobrimos o que acontece?**

`resolucao/` calcula e interpreta resultados. Ela não decide quem controla uma peça, não organiza a ordem das cadeiras e não define como a cena é escrita.

## Estrutura principal

- `principio-de-resolucao.md` — quando estabelecer diretamente, quando resolver incerteza e como tratar dúvida restante;
- `leitura-da-ficha-na-resolucao.md` — como identificar Atributo, Perícia, meio, situação e oposição realmente aplicáveis;
- `motor-de-disputa.md` — motor universal de testes contra cenário e oposição ativa;
- `efeitos/` — páginas de efeitos específicos;
- `escalas-de-efeito.md` — índice de compatibilidade que aponta para `efeitos/`;
- `fonte-e-vida-estrutural.md` — Fonte da manifestação, Atributo estrutural e Vida dos efeitos persistentes;
- `consolidacao.md` — Alcance, Alvos, Área/Tamanho, Duração e configuração de efeitos;
- `combate-e-dano.md` — regras específicas de combate e Dano;
- `ordem-de-resolucao-do-combate.md` — ordem operacional de resolução do combate;
- `energia.md` — recurso legado ainda aguardando migração para Mana;
- `recuperacao-da-vida.md` — recuperação e Medicina;
- `resolucao-social.md` — influência social e preservação de agência;
- `informacao-e-investigacao.md` — percepção, repertório e investigação normal.

## Entrada

```text
RESULTADO EVIDENTE
→ estabelecer.

IMPOSSIBILIDADE EVIDENTE
→ estabelecer.

INCERTEZA REAL
→ usar somente a regra necessária.
```

A resolução não fabrica dúvida quando o resultado já está claro.

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

Dados adicionais ou removidos vêm de fontes mecânicas explícitas, como Perícia, Poder, Status, Trama ou outra regra que diga diretamente `+Xd` ou `-Xd`.

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

## Tarefas demoradas

O antigo sistema de `Exigência`, `Progresso por aplicação` e `Aplicações necessárias` não faz mais parte do motor universal.

Uma tarefa não recebe várias rolagens apenas porque demora.

```text
resultado evidente com tempo suficiente
→ estabelecer o resultado e o tempo coerente.

impossibilidade evidente
→ estabelecer a impossibilidade.

incerteza real contra a situação
→ um teste contra Dificuldade.

oposição ativa
→ uma oposição comum quando necessário.
```

Rolagens adicionais só existem quando a ficção realmente cria uma nova incerteza relevante depois da resolução anterior.

## Atalho de combate

Quando houver combate, consultar primeiro:

```text
ordem-de-resolucao-do-combate.md
```

Atalho operacional:

```text
HUD → declaração → escolhas faltantes → IAs/Opositor → resolver → atualizar → novo HUD
```

A operação dos turnos continua pertencendo a `../operacao/`. O motor universal apenas resolve as incertezas que surgem dentro desse fluxo.

## Efeitos

Para um efeito específico, consultar diretamente sua página em `efeitos/` enquanto essa área não for migrada para a estrutura final de Poderes e Status.

Regras específicas podem acrescentar etapas próprias, mas não recriam o antigo motor de Base/Suporte/Progresso.

## Fronteiras

```text
quem decide?                    → ../personas/
quem move oposição?             → ../personas/opositor/
ordem e turnos?                 → ../operacao/
como mostrar o resultado?       → ../narracao/
o que permanece depois?         → ../persistencia/
como calcular o resultado?      → resolucao/
```

## Princípios finais

> **A ficção decide se existe teste, qual Atributo é pertinente e qual é a dificuldade real.**

> **A resolução usa o menor número possível de rolagens.**

> **Importância dramática e Patamar não alteram artificialmente a Dificuldade.**
