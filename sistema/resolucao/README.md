# Resolução

Status: APROVADO

Esta pasta responde à pergunta:

> **Dadas as intenções, capacidades, circunstâncias e oposição, como descobrimos o que acontece?**

`resolucao/` calcula e interpreta resultados. Ela não decide quem controla uma peça, não organiza a ordem das cadeiras e não define como a cena é escrita.

## Estrutura principal

- `principio-de-resolucao.md` — quando estabelecer diretamente e quando resolver incerteza;
- `leitura-da-ficha-na-resolucao.md` — como Atributos, Perícias, Poderes, meios, situação e conhecimento entram na resolução;
- `comparacao-e-disputa.md` — comparação qualitativa, estratégia, preparação e disputas equilibradas;
- `motor-de-disputa.md` — Potência, Resistência, Exigência, progresso, tempo, custo e contenção sustentada;
- `escalas-de-efeito.md` — tabelas de referência dos efeitos;
- `geral.md` — manifestações narrativas, utilitárias e cotidianas sem efeito prático de combate;
- `consolidacao.md` — Alcance, Alvos, Área/Tamanho, Duração, Ampliação, custo e estrutura de efeitos persistentes;
- `combate-e-dano.md` — fonte de Dano, Perícia efetiva, Ataque efetivo, Dano aplicado e defesa;
- `ordem-de-resolucao-do-combate.md` — ordem de processamento do turno, HUD do JOGADOR HUMANO, confirmações, configuração, interferência e fechamento do combate;
- `energia.md` — Reserva, custos, Ampliação, Bateria e recuperação;
- `recuperacao-da-vida.md` — recuperação natural, Regeneração, Cura e Medicina;
- `resolucao-social.md` — influência social e preservação de agência;
- `informacao-e-investigacao.md` — percepção, interpretação, investigação e Informação.

## Atalho de combate

Quando houver combate, consultar primeiro:

```text
ordem-de-resolucao-do-combate.md
```

Atalho operacional:

```text
HUD → declaração → confirmação, se necessária → IAs/Opositor → resolver → atualizar → novo HUD
```

## Entrada

```text
RESULTADO EVIDENTE
→ estabelecer.

IMPOSSIBILIDADE EVIDENTE
→ estabelecer.

INCERTEZA REAL
→ usar a regra específica adequada.
```

A resolução não fabrica dúvida quando o resultado já está claro.

## Motor geral

Quando necessário:

```text
Perícia efetiva = Perícia de aplicação − Perícia de oposição

Efeito efetivo = Potência usada + 1 + (Perícia efetiva × 0,2)

Progresso por aplicação = 2^(Efeito efetivo − Resistência efetiva)
```

Quando a tarefa permite acúmulo:

```text
Aplicações necessárias = teto(Exigência ÷ Progresso por aplicação)
```

A escala temporal padrão é definida em `motor-de-disputa.md`:

```text
10 segundos → aplicação imediata
1 minuto    → aplicação curta
1 hora      → aplicação prolongada
1 dia       → aplicação extensa
```

Durante combate, a aplicação imediata de 10 segundos usa o mesmo relógio de `../operacao/turnos-de-combate.md`.

## Regras especializadas

Dano, Cura, Energia, Proteção, Dissipar, Geral, efeitos persistentes, Invocação, contenção e demais efeitos continuam sendo calculados pelos arquivos especializados desta pasta.

`README.md` não substitui essas regras.

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

> **A ficção determina quais valores entram. A resolução determina a consequência.**

> **A Resistência pode transformar dificuldade em tempo, custo e oportunidade de reação.**

> **O plano não vence o patamar; o plano pode mudar o problema.**