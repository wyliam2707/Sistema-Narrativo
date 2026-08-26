# Poderes

Status: APROVADO

Um **Poder** representa parte do arsenal funcional da personagem.

A ficha registra **quais Poderes ela possui**. A mecânica concreta de cada Poder pertence a `../resolucao/poderes/`.

> **`personagem/poderes.md` define posse e função do arsenal; `resolucao/poderes/` define uso, Hub, custo e efeito.**

## Poder não usa grau genérico

Não existe escala universal:

```text
Poder [1] [2] [3] [4] [5]
```

A ficha registra apenas os Poderes existentes:

```text
PODERES:
- Teleporte
- Proteção
- Ilusão
```

Ausência significa que aquela capacidade não faz parte do arsenal registrado. Não usar `Poder [0]`.

## Ações comuns não exigem Poder

Ações ordinárias ficcionalmente possíveis usam Atributos, Perícias, equipamento e resolução comum.

```text
socar
correr
escalar
empurrar
usar ferramenta comum
→ não exigem um Poder homônimo
```

Poder é necessário para uma função especial que a personagem não produz apenas pelos meios comuns.

```text
teleportar
invocar
criar Barreira extraordinária
produzir disparo especial
impor domínio mental sobrenatural
```

## Hub

Cada Poder possui regra concreta em `../resolucao/poderes/`.

Um Hub pode organizar, conforme necessário:

- Alcance;
- Alvos;
- Área;
- Dano;
- Efeito;
- Defesa;
- Duração;
- Conjuração;
- Tipo;
- Modo;
- Distância;
- Escopo;
- Tamanho;
- outras propriedades próprias.

Nem todo Poder usa todos os campos.

## Patamar e [X]

Quando uma regra usar `[X]`:

> **[X] = Patamar da personagem**

`[X]` normalmente limita a Mana máxima investida num único uso, conforme `../resolucao/mana.md` e `patamar.md`.

O custo concreto pertence ao Hub correspondente.

## Quem escolhe a configuração

Se um uso de Poder possui escolhas voluntárias de alvo, forma, alcance, intensidade ou outra configuração, a decisão pertence a quem tiver autoridade sobre a peça conforme `../personas/`.

A sequência para pedir escolhas faltantes durante o jogo pertence a `../operacao/ordem-de-resolucao-do-combate.md` quando estiver em combate.

Este arquivo não redefine autoridade nem procedimento.

## Ataques comuns e Poderes ofensivos

Uma personagem sem Poder ofensivo ainda pode realizar ataque comum.

A regra de ataque e Dano pertence a `../resolucao/combate-e-dano.md`.

Poderes ofensivos podem definir Dano, Defesa, Resistência, Efeito, alcance, Área e outras propriedades próprias.

## Atributo, Perícia e Poder são coisas diferentes

```text
ATRIBUTO
→ capacidade fundamental

PERÍCIA
→ treinamento e experiência

PODER
→ função especial do arsenal
```

Eles não são somados automaticamente.

## Capacidade natural

Uma capacidade já adequadamente representada por Atributo ou Traço não precisa virar Poder apenas para ser repetida.

```text
Potência [5]
→ já pode representar força natural extraordinária
```

Uma função ativa, configurável ou com efeito próprio pode justificar um Poder.

## Forma narrativa

A aparência não cria automaticamente um Poder novo.

A mesma função mecânica pode se manifestar de formas diferentes quando Conceito e regra permitirem.

> **A ficção descreve a forma. O Hub descreve a função mecânica.**

## Calibração

A escolha inicial do arsenal segue `../criacao/calibracao.md`.

Não adicionar ou retirar Poder para equilibrar automaticamente personagens, garantir vencedor ou recuperar dificuldade depois de uma solução válida.

## Regra final

> **A ficha registra quais Poderes a personagem possui. Toda mecânica concreta de uso pertence a `resolucao/poderes/`; toda autoridade de escolha pertence a `personas/`.**
