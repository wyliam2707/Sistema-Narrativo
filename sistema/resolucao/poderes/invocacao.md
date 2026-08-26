# Invocação [X]

Invocação cria ou traz criaturas auxiliares para agir de acordo com sua natureza e com os comandos recebidos.

## Hub

- **Alcance:** Próximo `+0` → Curto `+1` → Médio `+2`
- **Conjuração:** Cena `+0` → Turno `+1` → Instante `+2`
- **Invocações:** 1 `+0` → 2 `+1` → 4 `+2`
- **Criatura:** ND 0 `+0` → ND 1 `+1` → ND 2 `+2` → ND 3 `+3` → ND 4 `+4`
- **Defesa:** Nula
- **Efeito:** Nula
- **Duração:** Cena `+0` → Hora `+1` → Dia `+2`

## Criatura Invocada

A criatura criada por este Poder é uma **manifestação temporária de Invocação**. Seu modelo por ND é uma regra específica deste Poder e não substitui as regras gerais de NPCs ou personagens.

Toda criatura invocada usa uma ficha-base determinada pelo seu ND:

- **Atributos:** todos os Atributos são iguais ao ND.
- **Vida:** `5 + (ND × 5)` PV.
- **Deslocamento:** Curto, de acordo com a natureza e a descrição da criatura.
- **Ataque:** `4d6 + ND` contra a Defesa do alvo.
- **Defesa do ataque:** Total; se a Defesa vencer, o ataque não causa dano.
- **Dano:** `1d4 + ND`.

O **ND representa a capacidade mecânica da manifestação**, não limita aquilo que sua natureza permite fazer na ficção. Uma criatura pode realizar ações evidentes para sua forma e descrição sem teste; só há teste quando existir incerteza real.

### Referência por ND

| ND | Atributos | Vida | Dano |
|---|---:|---:|---:|
| 0 | 0 | 5 PV | `1d4` |
| 1 | 1 | 10 PV | `1d4 + 1` |
| 2 | 2 | 15 PV | `1d4 + 2` |
| 3 | 3 | 20 PV | `1d4 + 3` |
| 4 | 4 | 25 PV | `1d4 + 4` |

Se uma criatura deixar de ser uma manifestação temporária e passar a existir como personagem independente e persistente, sua construção passa a seguir as regras normais de `../../personagem/`.

## Comandos

Ao ser invocada, a criatura recebe um **comando inicial**.

Ela age de forma autônoma para cumprir esse comando, interpretando-o conforme sua natureza e inteligência.

Durante a formação das declarações de cada turno simultâneo, o invocador pode manter o comando atual ou fornecer **um novo comando breve**, como:

- “Ataque aquele homem.”
- “Proteja a porta.”
- “Siga ela.”
- “Volte para mim.”

Isso não cria uma ação extra nem consome uma unidade abstrata de ação, porque o sistema não possui economia universal de uma ação por turno.

Para receber um novo comando, a criatura precisa estar em **Alcance Médio** do invocador. Fora desse alcance, continua seguindo o último comando recebido.

## Momento de agir

A criatura **não possui iniciativa separada nem posição fixa numa fila**.

Ela participa do mesmo intervalo simultâneo de até 10 segundos que as demais peças e tenta cumprir seu comando dentro desse intervalo.

Quando a ação da criatura interferir diretamente com outra intenção e a ficção não estabelecer precedência evidente, aplicar as regras normais de interferência e oposição de `../../operacao/turnos-de-combate.md` e `../motor-de-disputa.md`.

> **Invocação não cria uma ordem própria de iniciativa. A manifestação age dentro do turno simultâneo.**

## Fim da Invocação

Quando a duração da Invocação termina, a criatura **deixa de permanecer ativa na cena**.

Mecanicamente, ela simplesmente desaparece. A forma como isso acontece é determinada pela origem e pela descrição da própria Invocação.

Da mesma forma, quando uma criatura invocada chega a **0 Vida**, ela não fica Incapacitada: **deixa a cena imediatamente**.

Exemplos:

- uma criatura extraplanar pode **retornar ao seu plano de origem**;
- um robô invocado pode **se autodestruir ou se desmontar**;
- um golem formado de areia pode **voltar a ser areia**;
- uma criatura feita de sombras pode **se dissipar**.

> **A regra é o desaparecimento da Invocação; a ficção determina como esse desaparecimento se manifesta.**

## Exemplos

Um **pássaro ND 0** possui todos os Atributos em `[0]`, 5 PV e Deslocamento Curto voando. Ele pode levar uma mensagem até um destino coerente com sua descrição. Isso não exige teste se o resultado for evidente; tempestade, predadores, interceptação ou outras incertezas podem exigir resolução mecânica.

Um **lobo ND 2** possui todos os Atributos em `[2]`, 15 PV, Deslocamento Curto correndo, Ataque `4d6 + 2` e Dano `1d4 + 2`.