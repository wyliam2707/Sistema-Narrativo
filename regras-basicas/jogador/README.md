# Jogador

Status: REFORMULAÇÃO / NÃO IMPLEMENTADO

Esta pasta reúne as regras necessárias para **criar, ler e usar uma personagem durante a sessão**.

Ela serve tanto para personagens de jogadores quanto para NPCs, porque todos usam a mesma lógica básica de ficha.

```text
jogador/
├── README.md
├── 1.0-descricao-da-ficha.md
├── 1.1-atributos-pericias-poderes.md
└── 1.2-poderes-e-equipamentos.md
```

## `1.0-descricao-da-ficha.md`

Define a estrutura conceitual da ficha:

- o que a ficha representa;
- diferença entre Ficha e Estado Atual;
- Estado da Ficha;
- Importância;
- Controle;
- identidade e descrição;
- personalidade;
- objetivos, medos e limites;
- relações;
- conhecimento;
- ficha completa, rápida e mínima;
- uso da mesma lógica para jogadores e NPCs.

## `1.1-atributos-pericias-poderes.md`

Define a base de Atributos, Perícias e Patamares.

As partes antigas sobre construção e uso de Poderes permanecem em consolidação. Para **Pontos de Poder, custo por abrangência, Poder como opção de ação e equipamentos permanentes**, prevalece `1.2-poderes-e-equipamentos.md`.

## `1.2-poderes-e-equipamentos.md`

Define a regra simples de Poderes:

- Poder é uma opção de ação;
- graduação `[1]` a `[3]` mede a força da capacidade;
- abrangência serve apenas para calcular custo na criação;
- simples custa graduação ×1;
- abrangente custa graduação ×2;
- extremo custa graduação ×3;
- Patamares possuem `3 / 6 / 9 / 12 / 15` Pontos de Poder;
- equipamentos usam a mesma regra;
- o que é comprado com Pontos de Poder pertence permanentemente à ficha;
- perda ou indisponibilidade na cena não apaga o investimento.

## Princípio

```text
FICHA
→ quem a personagem é
→ capacidades consolidadas
→ interface principal de uso

ESTADO ATUAL
→ como ela está agora
→ pertence ao Registro da campanha
```

> **Complexidade na construção; simplicidade na mesa. Poderes ampliam o que a personagem pode fazer sem criar um subsistema novo para cada capacidade.**
