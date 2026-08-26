# Operação

Status: APROVADO

Esta pasta responde à pergunta:

> **Em que ordem o sistema é aplicado enquanto o RPG está rodando?**

`operacao/` organiza fluxo, janelas, turnos, aplicação das etapas e comandos administrativos. Ela não redefine personagem, autoridade, fórmulas, narração ou persistência.

## Estrutura

```text
operacao/
├── README.md
├── ciclo-de-cena.md
├── janelas-e-interrupcoes.md
├── turnos-de-combate.md
├── ordem-de-resolucao-do-combate.md
└── comandos-administrativos.md
```

### `ciclo-de-cena.md`

Organiza a sequência geral das cadeiras:

```text
JOGADORES
→ OPOSITOR
→ NARRADOR JULGA
→ NARRADOR NARRA A SENTENÇA
→ NARRADOR REGISTRA
```

### `janelas-e-interrupcoes.md`

Governa o fluxo normal fora de combate, passagem de tempo, interrupções e abertura de novas decisões.

### `turnos-de-combate.md`

Define o relógio simultâneo de combate: intervalos compartilhados de até 10 segundos.

### `ordem-de-resolucao-do-combate.md`

Define a aplicação prática dentro desse intervalo:

```text
HUD
→ declarações
→ interferência/precedência
→ resolução necessária
→ atualização
→ apresentação
→ novo HUD
```

Ele consulta `../resolucao/`; não contém um segundo motor mecânico.

### `comandos-administrativos.md`

Procedimentos fora da ficção, como manutenção e operações destrutivas que exigem confirmação.

## Fronteiras

```text
como criar?                       → ../criacao/
quem a personagem é?              → ../personagem/
quem decide?                       → ../personas/
como vontades continuam?           → ../agencia/
como calcular o resultado?         → ../resolucao/
como apresentar a cena?            → ../narracao/
o que permanece e onde salvar?     → ../persistencia/
qual sequência aplicar na mesa?     → operacao/
```

> **Operação não calcula. Ela determina quando e em que sequência consultar quem calcula.**

## Entrada durante o jogo

Fora de combate:

```text
ciclo-de-cena.md
→ janelas-e-interrupcoes.md
→ ../resolucao/ apenas quando surgir incerteza real
```

Em combate:

```text
ciclo-de-cena.md
→ turnos-de-combate.md
→ ordem-de-resolucao-do-combate.md
→ ../resolucao/ para cada cálculo necessário
```

## Registro

A operação pode determinar **quando** atualizar o presente, mas a regra de onde e como salvar pertence a `../persistencia/`.

O retrato operacional principal da campanha é:

```text
campanhas/<nome>/estado/atual.md
```

## Porta de entrada

```text
NOVA CAMPANHA
→ ../criacao/README.md

CONTINUAR CAMPANHA
→ campanhas/<nome>/README.md
```

O roteador geral permanece `../00-LEIA-PRIMEIRO.md`.

## Regra final

> **`operacao/` é o procedimento da mesa: organiza janelas, turnos e sequência de aplicação. As outras pastas continuam donas de suas próprias regras.**
