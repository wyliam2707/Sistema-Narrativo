# Personagem

Status: APROVADO

Esta pasta responde à pergunta:

> **Quem é esta personagem e do que ela é capaz?**

`personagem/` define a estrutura estável da peça. Ela guarda o modelo de ficha e as regras que descrevem capacidades consolidadas. Não conduz etapas de criação, não decide autoridade, não resolve ações e não guarda o estado momentâneo.

## Responsabilidades

Pertencem a esta área:

- estrutura da ficha;
- Patamar;
- Atributos;
- Perícias;
- Poderes possuídos;
- Traços e seus catálogos;
- Trama como recurso disponível ao protagonista humano;
- relações recorrentes;
- RECURSOS consolidados;
- Importância como metadado da ficha;
- `CONTROLE` apenas como campo registrado;
- representação mecânica compacta de NPCs;
- organização visual da ficha.

## O que não pertence aqui

```text
como criar ou revisar uma ficha?
→ ../criacao/personagem.md

como calibrar conceito em valores/capacidades?
→ ../criacao/calibracao.md

como parear informações entre fichas?
→ ../criacao/pareamento.md

quem decide pela peça?
→ ../personas/

como a vontade continua fora de cena?
→ ../agencia/

como calcular uma ação?
→ ../resolucao/

em que ordem aplicar as regras?
→ ../operacao/

como apresentar a cena?
→ ../narracao/

como e onde salvar mudanças?
→ ../persistencia/
```

> **A ficha registra `CONTROLE`; `personas/` define o que esse controle significa operacionalmente.**

## Base mecânica

```text
Patamar
→ [1] a [7]

Atributos permanentes
→ Potência
→ Controle
→ Resistência
→ Intelecto
→ Presença
→ Vontade
→ escala normal [-2] a [7]

Perícias
→ sem graduação
→ relevante = +1d

Poderes
→ arsenal funcional
→ sem grau genérico [1–5]
→ mecânica concreta em ../resolucao/poderes/

Traços
→ positivos [1–3]
→ Vícios [-1]
→ Corrupções [-1/-2]

Vida Máxima e Mana Máxima
→ derivadas dos Atributos permanentes

Trama
→ regra disponível apenas para CONTROLE: JOGADOR HUMANO
→ valor atual pertence ao estado persistente
```

## Ficha não é estado atual

A ficha registra aquilo que precisa permanecer disponível para definir e interpretar a personagem.

Não pertencem à ficha apenas por estarem acontecendo agora:

- Vida atual;
- Mana atual;
- Trama atual;
- Status;
- Barreiras;
- efeitos ativos;
- alterações temporárias de Atributo;
- localização;
- condições passageiras.

Essas informações pertencem a `../persistencia/`.

> **Personagem define quem a peça é. Persistência guarda como ela está.**

## NPCs

NPC não possui mecânica própria. Usa Patamar, Atributos, Perícias, Poderes, Traços, Vida e Mana como qualquer personagem.

`npcs.md` define apenas como representar mecanicamente NPCs de forma completa, rápida ou mínima.

Autoridade e delegação pertencem a `../personas/npcs-e-delegacao.md`. Continuidade fora de cena pertence a `../agencia/continuidade-de-npcs.md`. Destino persistente pertence a `../persistencia/material-reservado.md`.

## Arquivos principais

- `ficha.md` — estrutura consolidada da personagem;
- `organizacao-visual.md` — apresentação da ficha;
- `escala.md` — visão geral das escalas atuais;
- `patamar.md` — Patamar, pontos e limites;
- `atributos.md` — seis Atributos;
- `pericias.md` — lista canônica e `+1d` por relevância;
- `poderes.md` — posse e conceito de arsenal funcional;
- `tracos.md` — regra geral dos Traços;
- `tracos/` — catálogos de Traços;
- `trama.md` — usos mecânicos de Trama;
- `relacoes.md` — relações recorrentes;
- `npcs.md` — representação mecânica de NPCs.

## Compatibilidade

Não usar em fichas novas:

```text
FIS / RES / MEN / VON
Perícia [+0..+5]
Poder [1..5]
ENERGIA como reserva universal
Vida escolhida por função narrativa
```

## Regra final

> **`personagem/` descreve a peça. Procedimentos ficam em `criacao/`, autoridade em `personas/`, cálculo em `resolucao/` e estado em `persistencia/`.**
