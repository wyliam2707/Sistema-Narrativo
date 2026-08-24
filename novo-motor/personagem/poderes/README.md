# Poderes Ativos

Status: EM DESENVOLVIMENTO

Esta pasta contém os Poderes ativos do `novo-motor/`.

Cada Poder possui um arquivo próprio e autocontido. Durante o jogo, o narrador consulta apenas o arquivo do Poder escolhido pelo jogador.

## Regra de leitura

```text
Nome [X]
```

Nos Poderes ativos, `[X]` é o máximo de Energia que pode ser investido naquele Poder em um único uso.

O arquivo do Poder registra apenas o necessário para resolver seu uso: efeito-base, alcance, alvo, ação, duração, dano, ampliações e regras específicas quando aplicáveis.

Ampliações que gastam Energia nunca são escolhidas automaticamente pelo narrador. Se a intenção exigir uma ampliação, o narrador informa o custo e aguarda confirmação.

## Poderes registrados

- [Golpe](golpe.md)
- [Disparo](disparo.md)
- [Magia](magia.md)
- [Explosão](explosao.md)
- [Ampliação — Golpe](ampliacao-golpe.md)
- [Barreira](barreira.md)
- [Teleporte](teleporte.md)
- [Utilidade](utilidade.md)

Novos Poderes devem seguir a mesma ideia: regra curta, completa e consultável isoladamente.
