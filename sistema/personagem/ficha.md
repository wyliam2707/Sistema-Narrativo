# Ficha de Personagem

Status: APROVADO

A ficha é o **dossiê consolidado da personagem**.

Ela responde:

> **Quem é esta personagem e o que precisa permanecer disponível para interpretá-la e usar suas capacidades?**

A ficha não é o procedimento de criação, não é o STATUS atual e não é a regra de autoridade da mesa.

## O que a ficha pode registrar

Quando relevantes:

- identidade;
- Importância;
- `CONTROLE` como metadado;
- idade, aparência e estilo;
- Conceito e descrição;
- Patamar;
- Traços;
- Atributos permanentes;
- Vida Máxima;
- Mana Máxima;
- Perícias;
- Poderes possuídos;
- RECURSOS consolidados;
- relações recorrentes (`REL`);
- personalidade e tendências;
- desejos e objetivos relevantes;
- medos e limites;
- conhecimento atual relevante;
- história consolidada necessária à continuidade.

O critério do que merece permanecer na ficha pertence a `../persistencia/relevancia-da-ficha.md`.

## Ficha não é estado atual

Não entram na ficha apenas por estarem ativos agora:

- Vida atual;
- Mana atual;
- Trama atual;
- Dano atual;
- Status e condições temporárias;
- Barreiras;
- efeitos ativos;
- alterações temporárias de Atributo;
- localização;
- ferimentos transitórios;
- consequências causais ainda não incorporadas à personagem.

Esses elementos pertencem a `../persistencia/`.

> **Ficha = quem a personagem é. Estado = como ela está agora.**

## Modelo-base

```text
# Nome

Status:
Importância:
CONTROLE:
Patamar: [ ]

Nome real:
Idade:
Aparência:
Estilo:
Conceito:
Descrição:

TRAÇOS:

ATR:
Corpo  → Potência [ ] | Controle [ ] | Resistência [ ]
Mente  → Intelecto [ ] | Presença [ ] | Vontade [ ]

Vida Máxima [ ] | Mana Máxima [ ]

PERÍCIAS:
PODERES:
RECURSOS:

## Personalidade e tendências
## Desejos / objetivos atuais
## Medos / limites relevantes
## Amigos
## Inimigos
## Romance
## Conhecimento atual relevante
## História consolidada relevante
```

A organização visual detalhada pertence a `organizacao-visual.md`.

O procedimento para preencher e aprovar esse modelo pertence a `../criacao/personagem.md`.

## Campo desconhecido fica em branco

Zero é valor mecânico real.

```text
Controle [ ] → não definido
Controle [0] → definido como zero
```

A mesma regra vale para qualquer Atributo.

Perícias não usam `[+0]`; uma Perícia ausente não é registrada como valor zero.

Em fichas rápidas, ausência de um campo também não estabelece zero.

## Patamar

```text
Patamar: [1] a [7]
```

A regra completa pertence a `patamar.md`.

Patamar organiza desenvolvimento mecânico, limites de criação e `[X]` dos Poderes. Não mede Importância e não altera a Dificuldade do cenário.

## Atributos

A ficha completa usa:

```text
CORPO
Potência
Controle
Resistência

MENTE
Intelecto
Presença
Vontade
```

Escala permanente normal:

> **[-2] a [7]**

A regra completa pertence a `atributos.md`.

`Controle` é Atributo corporal. `CONTROLE` é metadado da ficha; são conceitos diferentes.

## Perícias

Perícias aparecem somente pelo nome:

```text
PERÍCIAS:
- Medicina
- Investigar
- Ocultismo
```

Não possuem graduação numérica.

Quando realmente relevantes para uma resolução, concedem `+1d` conforme `pericias.md` e `../resolucao/`.

## Poderes

A ficha registra **quais Poderes pertencem ao arsenal funcional** da personagem:

```text
PODERES:
- Teleporte
- Proteção
- Ilusão
```

Não existe grau genérico `[1–5]`.

A posse e o conceito pertencem a `poderes.md`; Hubs, custos e efeitos concretos pertencem a `../resolucao/poderes/`.

Quando um Poder usar `[X]`:

> **[X] = Patamar**

## Traços

A ficha registra Traços consolidados conforme `tracos.md` e `tracos/`.

Cada Traço positivo ocupa **1 espaço de Traço** na criação.

Se um Traço possuir número, nível, estágio ou categoria interna, isso faz parte do efeito específico daquele Traço e não representa custo de aquisição nem bônus genérico de teste.

Vícios e Corrupções continuam sendo Traços da personagem, não Status temporários.

## Vida Máxima

A ficha pode registrar o resultado derivado para consulta rápida.

Fonte canônica: `../resolucao/vida.md`.

```text
Vida = 10
+ Resistência ×4
+ Potência ×2
+ Controle ×2
+ Intelecto
+ Presença
+ Vontade
```

Para Vida, Atributos negativos contam como `0`.

Alteração permanente de Atributo recalcula Vida Máxima; alteração temporária não.

## Mana Máxima

Fonte canônica: `../resolucao/mana.md`.

```text
Mana = 10 + 2 × soma dos seis Atributos
```

Atributos negativos contam normalmente.

Alteração permanente de Atributo recalcula Mana Máxima; alteração temporária não.

## Importância

`IMPORTÂNCIA` registra o peso estrutural da personagem na campanha:

```text
Central
Relevante
Figurante
```

Ela não determina automaticamente:

- CONTROLE;
- tamanho da ficha;
- Patamar;
- Atributos;
- Perícias;
- Poderes;
- Traços;
- Vida;
- Mana;
- dificuldade;
- proteção narrativa.

Mudança de Importância é mudança estrutural da campanha e segue as regras de aprovação/persistência aplicáveis; não recalibra mecanicamente a ficha por si só.

## CONTROLE

A ficha registra um dos valores estruturais aplicáveis, por exemplo:

```text
CONTROLE: JOGADOR HUMANO
CONTROLE: JOGADOR IA
CONTROLE: JOGADOR IA EVENTUAL
CONTROLE: NPC
```

Este arquivo **não define a autoridade operacional desses valores**.

A regra canônica pertence a `../personas/`.

> **A ficha registra quem é a peça e qual CONTROLE está associado a ela; `personas/` define quem decide o quê.**

## RECURSOS

`RECURSOS` registra meios externos estáveis ou recorrentes que precisam permanecer disponíveis para continuidade, como:

- instalações;
- organizações;
- objetos únicos;
- acesso estabelecido;
- preparações recorrentes;
- infraestrutura relevante.

Não é um inventário obrigatório nem concede bônus automático.

Uma informação circunstancial ainda não consolidada pode pertencer ao estado ou às consequências persistentes em vez da ficha.

## REL

`REL` registra relações recorrentes que precisam permanecer disponíveis para interpretação e continuidade.

A definição pertence a `relacoes.md`.

Durante a criação, a consistência cruzada entre fichas é verificada por `../criacao/pareamento.md`.

Relação não é bônus mecânico automático.

## NPCs e fichas compactas

As regras para representação completa, rápida ou mínima de NPCs pertencem a `npcs.md`.

Informação omitida em ficha compacta não significa zero.

## Criação e revisão

Este arquivo define **o modelo e significado dos campos**.

A sequência de proposta, discussão, aprovação e preenchimento pertence a:

```text
../criacao/personagem.md
```

A ficha pode nascer com estrutura completa e campos vazios durante esse processo, mas essa é uma regra de criação, não uma segunda função deste arquivo.

## Alterações posteriores

Depois de criada, a ficha só muda quando uma transformação estável for consolidada conforme:

```text
../persistencia/atualizacao-de-ficha.md
```

Não existe evolução automática por missão, capítulo ou tempo apenas por ser conveniente.

## Formatos legados

Não usar em fichas atuais:

```text
FIS / RES / MEN / VON
Perícia [+0..+5]
Poder [1..5]
ENERGIA como reserva universal
Vida escolhida por função narrativa
```

## Regra final

> **`ficha.md` define o dossiê consolidado da personagem. Criação preenche; personas atribuem autoridade; resolução usa capacidades; persistência atualiza o que mudou.**
