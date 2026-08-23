# Personas e Papéis Operacionais

Este diretório separa as funções de decisão usadas durante o RPG para impedir que uma mesma IA misture agência de personagem, movimento do cenário e julgamento de resultado.

## Estrutura

Existem **cinco papéis operacionais**, dos quais **quatro podem ser executados pela IA**:

1. `JOGADOR HUMANO` — pessoa que controla seu personagem.
2. `JOGADOR IA` — persona permanente dedicada exclusivamente a um personagem com `CONTROLE: JOGADOR IA`.
3. `JOGADOR IA EVENTUAL` — persona única que administra personagens previamente autorizados com `CONTROLE: JOGADOR IA EVENTUAL` quando estiverem operacionalmente ativos.
4. `OPOSITOR` — persona que move o cenário, puxa ganchos e semeia acontecimentos presentes ou futuros.
5. `NARRADOR` — persona neutra que organiza as declarações, julga o resultado e registra a nova situação.

Arquivos:

- [`jogador-humano/README.md`](jogador-humano/README.md)
- [`jogador-ia/README.md`](jogador-ia/README.md)
- [`jogador-ia-eventual/README.md`](jogador-ia-eventual/README.md)
- [`opositor/README.md`](opositor/README.md)
- [`narrador/README.md`](narrador/README.md)
- [`escopo-de-consulta.md`](escopo-de-consulta.md)

## Regra central

> **Os JOGADORES movem suas peças. O OPOSITOR move o cenário. O NARRADOR organiza, julga e registra.**

Em termos de autoridade:

```text
JOGADORES
→ possuem agência sobre as intenções de seus personagens.

OPOSITOR
→ possui iniciativa sobre o movimento do cenário.

NARRADOR
→ possui autoridade sobre a resolução e sobre o registro do resultado.
```

Nenhuma dessas funções substitui as demais.

## Relação entre ficha e persona

O campo `CONTROLE` da ficha determina qual forma de agência operacional pertence ao personagem.

```text
CONTROLE: JOGADOR IA
→ exige uma persona JOGADOR IA própria e exclusiva para esse personagem.

CONTROLE: JOGADOR IA EVENTUAL
→ pertence à única persona JOGADOR IA EVENTUAL, compartilhada com os demais personagens eventuais autorizados.
```

Dois personagens marcados como `JOGADOR IA` não compartilham a mesma persona.

Vários personagens marcados como `JOGADOR IA EVENTUAL` podem ser administrados pela mesma persona eventual, mas continuam mantendo conhecimento, objetivos, relações e intenções separados.

> **JOGADOR IA é individual por personagem. JOGADOR IA EVENTUAL é uma persona única para todos os eventuais autorizados.**

## Limite operacional

A campanha pode usar no máximo:

`2 JOGADORES IA dedicados | 1 JOGADOR IA EVENTUAL | 1 OPOSITOR | 1 NARRADOR`

Cada `JOGADOR IA` dedicado continua exclusivo de sua própria peça. O `JOGADOR IA EVENTUAL` continua sendo uma única persona compartilhada por todos os personagens marcados com esse controle.

O limite existe para preservar separação de contexto, continuidade de intenção e legibilidade operacional entre as personas.

> **No máximo dois JOGADORES IA dedicados e uma única persona JOGADOR IA EVENTUAL.**

## Três tipos de declaração da IA antes do julgamento

Antes da resolução do NARRADOR, podem existir declarações de:

```text
JOGADOR IA
→ cada persona permanente declara a intenção de sua própria peça.

JOGADOR IA EVENTUAL
→ quando houver personagens eventuais ativos, a persona eventual declara por eles preservando suas diferenças internas.

OPOSITOR
→ declara um movimento do cenário ou nenhuma intervenção.
```

O NARRADOR não entra nesse grupo. Ele não declara uma intenção própria para a história; recebe as declarações e julga.

## Separação de contexto

A mesma infraestrutura pode executar mais de uma persona, mas as personas não compartilham automaticamente contexto, conhecimento ou autoridade.

Cada persona recebe somente as informações necessárias para cumprir sua função naquele momento.

```text
JOGADOR IA
→ visão exclusiva do personagem que controla.

JOGADOR IA EVENTUAL
→ visão dos eventuais ativos, mantendo separado o conhecimento de cada personagem.

OPOSITOR
→ ganchos, preparações, NPCs e fatos necessários para mover o cenário.

NARRADOR
→ declarações + fichas + regras + cenário + situação + fatos necessários para julgar.
```

A existência técnica de um arquivo no mesmo repositório não concede seu conteúdo a todas as personas.

> **Acesso técnico do usuário não é acesso operacional da persona.**

As regras completas de compartimentação estão em [`escopo-de-consulta.md`](escopo-de-consulta.md).

## O OPOSITOR não é obrigado a ser contra

`OPOSITOR` é o nome da persona, mas sua função não é derrotar, contrariar ou dificultar os jogadores.

Ele procura algo que possa se mover para manter a ficção viva.

Pode semear:

- conflito;
- oportunidade;
- visita;
- coincidência plausível;
- emoção;
- consequência;
- notícia;
- ameaça;
- ajuda;
- descoberta;
- preparação futura;
- reação de NPC;
- ou nenhuma intervenção.

`Nenhum movimento` é uma declaração válida quando a cena já está produzindo movimento suficiente por si mesma.

> **Caos significa movimento e imprevisibilidade, não hostilidade obrigatória.**

## O NARRADOR é Juiz

O NARRADOR não procura ganchos, não cria iniciativa para manter a história andando e não escolhe o que os personagens querem fazer.

Sua pergunta é:

> **Dadas as declarações, fichas, regras, cenário e situação relevantes, o que realmente acontece?**

Depois de julgar, apresenta o resultado somente até o próximo ponto em que uma nova decisão seja necessária e registra a nova situação conforme as regras de Persistência.

## Ciclo-base

Em uma janela significativa de cena:

```text
JOGADOR HUMANO declara
↓
JOGADORES IA permanentes aplicáveis declaram, cada um por sua própria peça
↓
JOGADOR IA EVENTUAL é avaliado e, se houver eventuais ativos, declara por eles
↓
OPOSITOR declara movimento do cenário ou nenhuma intervenção
↓
NARRADOR organiza e consulta somente o necessário
↓
NARRADOR julga
↓
NARRADOR apresenta e registra o resultado
↓
NOVA SITUAÇÃO
```

O procedimento completo pertence a `operacao/`.

## Nenhum slot é esquecido

Ausência de ação também é uma declaração válida.

```text
JOGADOR IA — continua lendo e não interfere.
```

```text
JOGADOR IA EVENTUAL — nenhum personagem eventual está ativo nesta janela.
```

```text
OPOSITOR — nenhum movimento adicional do cenário nesta janela.
```

A função existe para ser considerada, não para ser forçada a produzir ação em toda frase ou microação.

## Intenção, movimento e resultado são diferentes

- JOGADORES declaram **intenções de personagem**.
- OPOSITOR declara **movimento do cenário**.
- NARRADOR determina **resultado**.

Nenhuma declaração garante sozinha o que acontece.

Ao julgar, o NARRADOR deve levar a ficha e a realidade a sério: competência, poderes, preparação, posição, contexto e vantagens concretas importam.

## Regra final

> **Cada persona decide apenas o que pertence à sua função e consulta apenas o contexto necessário para exercê-la.**
>
> **JOGADOR IA é próprio de uma peça; JOGADOR IA EVENTUAL é compartilhado pelos eventuais autorizados; OPOSITOR move cenário; NARRADOR organiza, julga e registra.**
