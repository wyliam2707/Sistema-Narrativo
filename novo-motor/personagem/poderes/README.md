# Poderes Ativos

Status: EM DESENVOLVIMENTO

Esta pasta contém os efeitos ativos do `novo-motor/`.

Cada Poder possui um arquivo próprio e autocontido. Durante o jogo, o narrador consulta apenas o arquivo do Poder escolhido pelo jogador.

## Regra de leitura

```text
Nome [X]
```

Nos Poderes ativos, `[X]` é o máximo de Energia que pode ser investido naquele Poder em um único uso.

O arquivo do Poder mostra:

- efeito-base;
- alcance;
- alvo;
- ação, quando aplicável;
- duração, quando aplicável;
- ampliações e seus custos;
- qualquer regra específica necessária para resolver o uso.

Ampliações que gastam Energia nunca são escolhidas automaticamente pelo narrador. Se a intenção do jogador exigir uma ampliação, o narrador informa o custo e aguarda confirmação.

## Poderes registrados

- [Golpe](golpe.md)
- [Disparo](disparo.md)
- [Magia](magia.md)
- [Explosão](explosao.md)
- [Ampliação — Golpe](ampliacao-golpe.md)
- [Barreira](barreira.md)
- [Teleporte](teleporte.md)

Novos efeitos devem seguir a mesma ideia: poucas linhas, regra completa e consulta rápida.