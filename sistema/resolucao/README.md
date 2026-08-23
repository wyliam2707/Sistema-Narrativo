# Resolução

Status: APROVADO

Esta pasta responde à pergunta:

> **Dadas as intenções, capacidades, circunstâncias e oposição, como descobrimos o que acontece?**

`resolucao/` calcula e interpreta resultados. Ela não decide quem controla uma peça, não organiza a ordem das cadeiras e não define como a cena é escrita.

## Estrutura principal

- `principio-de-resolucao.md` — quando estabelecer diretamente, quando resolver incerteza e como tratar dúvida restante;
- `leitura-da-ficha-na-resolucao.md` — quais capacidades, meios, situação e oposição realmente entram;
- `motor-de-disputa.md` — Potência, Resistência, Exigência, Progresso, Tempo e Custo;
- `efeitos/` — uma página curta para cada efeito central;
- `escalas-de-efeito.md` — índice de compatibilidade que aponta para `efeitos/`;
- `fonte-e-vida-estrutural.md` — Fonte da manifestação, Atributo estrutural e Vida dos efeitos persistentes;
- `geral.md` — manifestações narrativas, utilitárias e cotidianas sem efeito prático de combate;
- `consolidacao.md` — Alcance, Alvos, Área/Tamanho, Duração e Ampliação;
- `combate-e-dano.md` — Fonte do Dano, Perícia efetiva, Ataque efetivo, Defesa, Dano e VIDA;
- `ordem-de-resolucao-do-combate.md` — ordem operacional de resolução do combate;
- `energia.md` — Reserva, custo, recuperação e Bateria;
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
HUD → declaração → escolhas faltantes → IAs/Opositor → resolver → atualizar → novo HUD
```

## Entrada

```text
RESULTADO EVIDENTE
→ estabelecer.

IMPOSSIBILIDADE EVIDENTE
→ estabelecer.

INCERTEZA REAL
→ usar somente a regra específica necessária.
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

A escala temporal pertence a `motor-de-disputa.md`.

## Efeitos

Para um efeito específico, consultar diretamente sua página em `efeitos/`.

`efeitos/README.md` contém apenas as regras compartilhadas entre efeitos persistentes e o índice das páginas.

`README.md` e `escalas-de-efeito.md` não substituem a página específica do efeito.

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

> **Na dúvida real restante, escolha a solução coerente que melhor faça a cena continuar.**
