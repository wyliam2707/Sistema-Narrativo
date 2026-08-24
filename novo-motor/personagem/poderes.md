# Poderes

Status: EM DESENVOLVIMENTO

No `novo-motor/`, Poderes são efeitos ativos autocontidos. Cada Poder possui seu próprio arquivo com tudo o que é necessário para usá-lo.

> **A ficha diz quais Poderes o personagem possui. O arquivo do Poder diz exatamente como ele funciona.**

## Estrutura geral

Um Poder é registrado pelo nome e por um valor entre colchetes:

```text
Teleporte [5]
Golpe [2]
Explosão [3]
```

O valor `[X]` representa o **máximo de Energia que pode ser investido naquele Poder em um único uso**.

O uso padrão de um Poder custa `0` Energia quando sua descrição possuir um efeito-base gratuito.

Sempre que o jogador escolher uma ampliação acima de `0`, gasta a quantidade correspondente de Energia.

Cada Poder define sua própria lógica. Ele pode usar:

- POD;
- HAB;
- valores fixos;
- dados;
- alcance;
- número de alvos;
- área;
- duração;
- outras propriedades próprias.

Não existe uma fórmula universal obrigatória para todos os Poderes.

## Ampliações

As ampliações aparecem diretamente ao lado do parâmetro que modificam.

Exemplo:

```text
Teleporte [5]

Alvo: 1 alvo > [+1 POD alvos] [+2 POD ×2 alvos]
Destino: Local conhecido > [+1 Visitado] [+2 Descrição]
Distância: até 100 km > [+1 500 km] [+2 Ilimitado]
```

Ampliações de linhas diferentes podem ser combinadas, desde que a soma total de Energia investida não ultrapasse `[X]`.

Exemplo:

```text
+2 POD ×2 alvos
+2 Descrição
+1 500 km
Total: 5 Energia
```

## Fluxo de uso

Quando o jogador declara que deseja usar um Poder:

```text
1. consultar a ficha;
2. listar apenas os Poderes disponíveis ao personagem;
3. o jogador escolhe um Poder;
4. consultar somente o arquivo desse Poder;
5. mostrar o efeito-base e suas ampliações;
6. o jogador declara o uso pretendido;
7. verificar se o uso cabe no efeito-base;
8. se couber, resolver sem gasto de Energia;
9. se exigir ampliação, informar exatamente qual custo é necessário;
10. o jogador confirma ou recusa o gasto;
11. somente após a confirmação, gastar Energia e resolver.
```

> **O narrador não escolhe automaticamente uma ampliação que consuma Energia. Ele informa o custo necessário e aguarda a confirmação do jogador.**

## Poderes ativos e Passivos

Poderes são capacidades ativas escolhidas durante a cena e consultadas sob demanda.

Passivos são diferentes: alteram valores estáveis da ficha e não precisam ser abertos durante cada uso.

Exemplos de Passivos:

```text
RD [3]
Vida Extra [30]
Proteção [2]
```

Os Passivos ficam registrados diretamente na ficha e são consolidados nos valores derivados do personagem.

As regras dos Passivos ficam em `passivos.md`.

## Arquivos individuais

Cada Poder ativo deve possuir um arquivo próprio dentro de:

```text
personagem/poderes/
```

O arquivo deve ser curto, direto e suficiente para resolver o Poder sem consultar uma cadeia de regras externas.

Poderes já registrados nesta etapa:

- `golpe.md`
- `disparo.md`
- `magia.md`
- `explosao.md`
- `ampliacao-golpe.md`
- `barreira.md`
- `teleporte.md`
