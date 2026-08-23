# Operação

Status: APROVADO

Esta pasta responde à pergunta:

> **Em que ordem o sistema é aplicado enquanto o RPG está rodando e como operações administrativas são executadas?**

`operacao/` organiza fluxo e procedimentos. Ela não redefine personagem, resolução, agência, narração ou persistência.

## Estrutura canônica

```text
operacao/
├── README.md
├── ciclo-de-cena.md
├── janelas-e-interrupcoes.md
├── turnos-de-combate.md
└── comandos-administrativos.md
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

Fluxo fora de combate: intenção ampla, passagem de tempo, interrupção, competência evidente e abertura de nova janela.

### `turnos-de-combate.md`

Combate em turnos simultâneos de até 10 segundos, com oportunidade para todas as peças e limite temporal da sentença.

As fórmulas de Dano, Cura, Energia, efeitos e demais mecânicas continuam em `../resolucao/`.

### `comandos-administrativos.md`

Procedimentos administrativos fora da ficção, incluindo exclusão de campanha com confirmação destrutiva obrigatória.

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
como executar manutenção?        → comandos-administrativos.md
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

## Arquivos legados aguardando limpeza

```text
../modo-rpg.md
../checklist-do-narrador.md
../comandos-administrativos.md
```

Seu conteúdo operacional útil já possui destino canônico. Não usar esses arquivos como regra atual. A exclusão depende de confirmação explícita.

## Porta de entrada geral

```text
NOVA CAMPANHA
→ sistema/criacao/README.md

CONTINUAR
→ campanhas/<nome>/README.md
```

`sistema/00-LEIA-PRIMEIRO.md` é o roteador geral.

## Regra final

> **README roteia. Arquivos especializados guardam as regras. `ciclo-de-cena.md` define a ordem; `janelas-e-interrupcoes.md` governa o fluxo normal; `turnos-de-combate.md` governa o combate; `comandos-administrativos.md` governa manutenção fora da ficção.**