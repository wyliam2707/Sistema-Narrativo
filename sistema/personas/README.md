# Personas e Papéis Operacionais

Status: APROVADO

Esta pasta responde:

> **Quem tem autoridade para decidir o quê na mesa?**

## As cinco cadeiras

```text
JOGADOR HUMANO
→ joga sua própria peça.

JOGADOR IA
→ joga uma peça dedicada sob CONTROLE: JOGADOR IA.

JOGADOR IA EVENTUAL
→ joga peças eventuais e NPCs comuns quando precisam de decisão própria.

OPOSITOR
→ promotoria; movimenta ganchos e joga a oposição legitimamente disponível.

NARRADOR
→ juiz; julga, narra a sentença e registra.
```

> **Imagine cinco pessoas sentadas à mesma mesa. Os jogadores movimentam suas peças. O OPOSITOR argumenta e joga a promotoria. O NARRADOR não joga: ele julga.**

## Estrutura

```text
personas/
├── README.md
├── escopo-de-consulta.md
├── npcs-e-delegacao.md
├── jogador-humano/
├── jogador-ia/
├── jogador-ia-eventual/
├── opositor/
└── narrador/
```

### `jogador-humano/`

Autoridade sobre decisões voluntárias da peça humana.

### `jogador-ia/`

Jogador dedicado de uma personagem específica.

### `jogador-ia-eventual/`

Persona compartilhada que assume personagens eventuais recorrentes e NPCs comuns ad hoc quando precisam decidir.

### `npcs-e-delegacao.md`

Define quem joga um NPC quando ele não possui jogador dedicado:

```text
ROTINA EVIDENTE
→ NARRADOR pode narrar como consequência já determinada.

DECISÃO VOLUNTÁRIA RELEVANTE, NÃO ADVERSARIAL
→ JOGADOR IA EVENTUAL assume a peça.

OPOSIÇÃO ATIVA
→ NPC pode ser delegado ao OPOSITOR após julgamento de disponibilidade.
```

A assunção temporária não muda automaticamente o `CONTROLE` da ficha.

### `opositor/`

Promotoria da mesa: observa oportunidades, mantém ganchos, persegue planos adversários e joga peças de oposição legitimamente delegadas.

### `narrador/`

Juiz da mesa:

```text
1. JULGAR
2. NARRAR A SENTENÇA
3. REGISTRAR
```

Não toma decisões voluntárias por personagens.

### `escopo-de-consulta.md`

Define qual informação cada persona pode receber e reforça:

```text
PERSONA SABE
≠
PERSONAGEM SABE
```

## Importância não define controle

`IMPORTÂNCIA` mede peso estrutural da personagem.

`CONTROLE` define quem toma suas decisões.

São eixos independentes.

Uma personagem Central, Relevante ou Figurante pode usar qualquer `CONTROLE` aprovado pela campanha.

Mudar IMPORTÂNCIA não muda automaticamente CONTROLE, ficha ou mecânica.

## Mesa como tribunal

```text
HISTÓRIA
→ processo.

JOGADORES
→ defesa das próprias peças.

OPOSITOR
→ promotoria.

NARRADOR
→ juiz.
```

O OPOSITOR pode jogar para vencer.

O NARRADOR não ajuda nem a defesa nem a promotoria.

Quando restar dúvida genuína depois de fatos, regras e resolução aplicáveis:

> **In dubio pro reo — favoreça a defesa.**

## Regra final

> **Quem quer algo declara pela cadeira que possui autoridade sobre aquela peça. Quem se opõe apresenta sua jogada. O NARRADOR apenas julga, narra a sentença e registra. NPC comum também segue essa separação: rotina não exige jogador; vontade relevante exige.**
