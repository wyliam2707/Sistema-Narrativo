# Poderes

Status: EM DESENVOLVIMENTO

Poderes são efeitos ativos autocontidos. A ficha registra apenas o nome do Poder e seu limite `[X]`; a regra completa fica no arquivo individual em `poderes/`.

> **A ficha diz quais Poderes o personagem possui. O arquivo do Poder diz exatamente como ele funciona.**

## `[X]` nos Poderes

```text
Nome [X]
```

`[X]` é o máximo de Energia que pode ser investido naquele Poder em um único uso.

Um Poder pode possuir efeito-base em `0` Energia. Quando a intenção do jogador exigir uma ampliação, o custo correspondente é gasto somente após confirmação.

Cada Poder define sua própria lógica e pode usar, conforme sua descrição:

- POD;
- HAB;
- dados;
- valores fixos;
- alcance;
- alvo;
- área;
- duração;
- ampliações próprias.

Não existe fórmula universal obrigatória para todos os Poderes.

## Formato operacional

Sempre que possível, a base e as ampliações aparecem na mesma linha:

```text
Teleporte [5]

Alvo: 1 alvo > [+1 POD alvos] [+2 POD ×2 alvos]
Destino: Local conhecido > [+1 Visitado] [+2 Descrição]
Distância: até 100 km > [+1 500 km] [+2 Ilimitado]
```

Ampliações de parâmetros diferentes podem ser combinadas desde que o custo total não ultrapasse `[X]`.

## Fluxo de uso

```text
1. jogador declara que quer usar um Poder;
2. narrador lista os Poderes disponíveis;
3. jogador escolhe um;
4. narrador abre apenas o arquivo escolhido;
5. mostra efeito-base e ampliações;
6. jogador declara a intenção;
7. se couber na base, resolve;
8. se exigir ampliação, informa o custo;
9. jogador confirma ou recusa;
10. somente após confirmação, gastar Energia e resolver.
```

> **O narrador não escolhe automaticamente uma ampliação que consuma Energia.**

## Poderes e manifestação narrativa

A mecânica pertence ao Poder; a aparência pertence à ficção.

```text
Golpe → soco, espada, garra, bastão.
Disparo → arco, pistola, batarang, laser.
Explosão → granada, carga, magia explosiva.
```

Não criar uma regra de item separada quando a função já estiver representada por um Poder.

## Arquivos individuais

Poderes registrados em `poderes/`:

- `golpe.md`
- `disparo.md`
- `magia.md`
- `explosao.md`
- `ampliacao-golpe.md`
- `barreira.md`
- `teleporte.md`
- `utilidade.md`

Novos Poderes devem ter arquivo próprio, curto e suficiente para resolver seu uso sem depender de uma cadeia extensa de consultas.

## Separação de Passivos

Passivos não seguem a regra de gasto máximo de Energia dos Poderes ativos. Eles ficam em `passivos.md` e `passivos/`.
