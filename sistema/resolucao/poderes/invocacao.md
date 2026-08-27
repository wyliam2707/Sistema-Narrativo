# Invocação [X]

Invocação cria, manifesta ou traz criaturas auxiliares para agir de acordo com sua natureza e com os comandos recebidos.

A forma ficcional da Invocação é livre dentro do Conceito da personagem.

Exemplos igualmente válidos:

- criatura extraplanar;
- elemental;
- morto-vivo;
- construto;
- robô ou drone;
- animal criado ou chamado;
- duplicata temporária do próprio invocador.

> **A forma ficcional muda o que a manifestação é. A regra de Invocação define como ela funciona mecanicamente.**

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
- **Ataque básico:** `4d6 + ND` contra a Defesa fixa coerente com a natureza do ataque, normalmente DF para um ataque físico.
- **Defesa do ataque:** Total; resultado abaixo da Defesa fixa não causa Dano.
- **Dano:** `1d4 + ND`.

Como todos os Atributos da ficha-base são iguais ao ND, suas Defesas fixas também resultam normalmente em:

```text
DF = 14 + ND
RF = 14 + ND
DM = 14 + ND
RM = 14 + ND
```

Uma natureza ou regra específica pode alterar qual Defesa é usada por determinada ação.

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

## Duplicação como Invocação

Invocação pode representar a criação de **duplicatas temporárias do próprio invocador**.

Nesse caso:

- a duplicata pode ter aparência, voz, memória funcional e comportamento coerentes com a origem da duplicação;
- mecanicamente, continua usando a ficha-base de Invocação determinada pelo ND;
- parecer uma cópia não concede automaticamente todos os Atributos, Poderes, Recursos ou efeitos da ficha original;
- qualquer capacidade especial que a duplicata realmente possa reproduzir precisa estar autorizada por uma regra específica, por seu modelo de Invocação ou por outra capacidade registrada.

Assim, duplicação não exige um Poder universal separado quando sua função mecânica já for satisfeita por Invocação.

## Comandos

Ao ser invocada, a criatura recebe um **comando inicial**.

Ela age de forma autônoma para cumprir esse comando, interpretando-o conforme sua natureza e inteligência.

Durante a vez do invocador, ele pode manter o comando atual ou fornecer **um novo comando breve**, como:

- “Ataque aquele homem.”
- “Proteja a porta.”
- “Siga ela.”
- “Volte para mim.”

Isso não cria uma ação extra nem consome uma unidade abstrata de ação, porque o sistema não possui economia universal de uma ação por turno.

Para receber um novo comando, a criatura precisa estar em **Alcance Médio** do invocador. Fora desse alcance, continua seguindo o último comando recebido.

## Momento de agir em combate

Uma criatura invocada que participe ativamente do combate é uma peça da Iniciativa.

Quando surgir depois do início do confronto, aplicar a regra de **entrada posterior** de `../../operacao/turnos-de-combate.md`:

```text
criatura surge
→ rola Iniciativa uma vez
→ entra na posição correspondente
→ mantém essa posição enquanto permanecer no combate
```

Se sua nova posição ainda não tiver sido processada na Rodada atual, ela poderá agir quando essa posição chegar.

Se essa posição já tiver passado, sua primeira vez ocorrerá na Rodada seguinte.

A criatura resolve sua própria vez seguindo o comando vigente, sua natureza e o estado atual da cena.

Invocação não cria uma fila paralela nem altera a Iniciativa das peças que já estavam presentes.

## Fim da Invocação

Quando a duração da Invocação termina, a criatura **deixa de permanecer ativa na cena**.

Mecanicamente, ela simplesmente desaparece. A forma como isso acontece é determinada pela origem e pela descrição da própria Invocação.

Da mesma forma, quando uma criatura invocada chega a **0 Vida**, ela não fica Incapacitada: **deixa a cena imediatamente**.

Exemplos:

- uma criatura extraplanar pode **retornar ao seu plano de origem**;
- um robô invocado pode **se autodestruir ou se desmontar**;
- um golem formado de areia pode **voltar a ser areia**;
- uma criatura feita de sombras pode **se dissipar**;
- uma duplicata pode **fundir-se ao original, desfazer-se ou desaparecer**, conforme sua origem.

> **A regra é o desaparecimento da Invocação; a ficção determina como esse desaparecimento se manifesta.**

## Exemplos

Um **pássaro ND 0** possui todos os Atributos em `[0]`, 5 PV e Deslocamento Curto voando. Ele pode levar uma mensagem até um destino coerente com sua descrição. Isso não exige teste se o resultado for evidente; tempestade, predadores, interceptação ou outras incertezas podem exigir resolução mecânica.

Um **lobo ND 2** possui todos os Atributos em `[2]`, 15 PV, Deslocamento Curto correndo, Ataque `4d6 + 2` e Dano `1d4 + 2`.

## Regra final

> **Invocação cria manifestações temporárias mecanicamente definidas por ND. A manifestação pode ser criatura, construto, drone, morto-vivo ou duplicata. Em combate, ela entra na Iniciativa como peça ativa conforme a regra de entrada posterior e age em sua própria vez seguindo o comando vigente.**
