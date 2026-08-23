# Operação

Status: APROVADO

Esta pasta responde à pergunta:

> **Em que ordem o sistema é aplicado enquanto o RPG está rodando?**

`operacao/` organiza o fluxo. Ela não redefine personagem, resolução, agência, narração ou persistência.

## Estrutura canônica

```text
operacao/
├── README.md
├── ciclo-de-cena.md
├── janelas-e-interrupcoes.md
└── turnos-de-combate.md
```

### `ciclo-de-cena.md`

Sequência central das cinco cadeiras:

```text
JOGADORES
→ OPOSITOR
→ NARRADOR JULGA
→ NARRADOR NARRA A SENTENÇA
→ NARRADOR REGISTRA
```

### `janelas-e-interrupcoes.md`

Usar fora de combate para:

- intenção ampla;
- passagem de tempo;
- ponto real de interrupção;
- devolução de controle;
- competência evidente;
- abertura de nova janela.

### `turnos-de-combate.md`

Usar durante combate para:

- turnos simultâneos de até 10 segundos;
- oportunidade de declaração para todas as peças;
- precedência dentro do mesmo intervalo;
- limite temporal da sentença;
- fechamento do estado antes do turno seguinte.

As fórmulas de Dano, Cura, Energia, efeitos e demais mecânicas continuam em `../resolucao/`.

## Imagem mental

```text
JOGADORES
→ defesa das próprias peças.

OPOSITOR
→ promotoria.

NARRADOR
→ juiz.
```

> **O NARRADOR não move a disputa. Ele julga, narra a sentença e registra.**

## Roteamento

```text
como criar campanha?             → ../criacao/
quem é / do que é capaz?         → ../personagem/
quem decide?                     → ../personas/
como preservar vontade própria?  → ../agencia/
como calcular o resultado?       → ../resolucao/
como apresentar a cena?          → ../narracao/
o que permanece e onde salvar?   → ../persistencia/
como aplicar tudo em sequência?  → operacao/
```

## Entrada durante o jogo

```text
fora de combate
→ ciclo-de-cena.md
→ janelas-e-interrupcoes.md

combate
→ ciclo-de-cena.md
→ turnos-de-combate.md
→ ../resolucao/ quando houver cálculo
```

## Registro

O retrato operacional principal da campanha é:

```text
campanhas/<nome>/estado/atual.md
```

Ganchos atuais do OPOSITOR podem ficar em:

```text
campanhas/<nome>/mestre/ganchos-do-opositor.md
```

A persistência concreta segue `../persistencia/`.

## Arquivos legados

Os arquivos:

```text
../modo-rpg.md
../checklist-do-narrador.md
```

permanecem temporariamente preservados apenas como legado.

> **Não usar esses arquivos como regra operacional.**

Seu conteúdo útil foi migrado para as áreas canônicas. Eles só devem ser apagados após confirmação explícita.

## Porta de entrada geral

```text
NOVA CAMPANHA
→ sistema/criacao/README.md

CONTINUAR
→ campanhas/<nome>/README.md
```

`sistema/00-LEIA-PRIMEIRO.md` continua sendo o roteador geral.

## Regra final

> **README roteia. Arquivos especializados guardam as regras. `ciclo-de-cena.md` define a ordem; `janelas-e-interrupcoes.md` governa o fluxo normal; `turnos-de-combate.md` governa o combate.**