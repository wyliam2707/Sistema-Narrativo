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
├── rotina-de-trama-em-combate.md
└── comandos-administrativos.md
```

### `ciclo-de-cena.md`

Organiza a sequência geral das cadeiras fora das regras específicas de combate:

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

Define a Rodada global, o Turno pessoal e a **ordem fixa de Iniciativa** do combate.

Cada participante rola uma única vez no início:

```text
Iniciativa = 4d6 + Controle
```

A ordem resultante é reutilizada até o fim do combate.

### `ordem-de-resolucao-do-combate.md`

Define a aplicação prática dessa ordem:

```text
Iniciativa
→ peça ativa
→ declaração
→ Hub quando aplicável
→ resolução e Defesa/Resistência
→ atualização imediata
→ próximo da Iniciativa
```

Ele consulta `../resolucao/`; não contém um segundo motor mecânico.

### `rotina-de-trama-em-combate.md`

Define as janelas obrigatórias em que o combate deve devolver ao JOGADOR HUMANO a decisão de usar Trama.

```text
antes de rolagem elegível
→ checar Trama

Mana faltante em configuração válida
→ checar Trama

Dano prestes a atingir Vida
→ checar Trama
```

A checagem é obrigatória. O gasto continua opcional.

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
→ rotina-de-trama-em-combate.md sempre que surgir uma janela válida
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

> **`operacao/` organiza janelas, Rodadas, Turnos, sequência e decisões obrigatórias de fluxo. Em combate, a Iniciativa é rolada uma vez, sua ordem permanece até o confronto terminar e toda janela válida de Trama deve ser aberta ao JOGADOR HUMANO antes de prosseguir. As outras pastas continuam donas de suas próprias regras.**
