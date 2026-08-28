# Jogador

Status: REFORMULAÇÃO / NÃO IMPLEMENTADO

Esta pasta reúne as regras necessárias para **criar, ler e usar uma personagem durante a sessão**.

Ela serve tanto para personagens de jogadores quanto para NPCs, porque todos usam a mesma lógica básica de ficha.

```text
jogador/
├── README.md
├── 1.0-descricao-da-ficha.md
└── 1.1-atributos-pericias-poderes.md
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

Define a estrutura mecânica básica da personagem:

- seis Atributos;
- doze Perícias gerais;
- graduação de Atributos, Perícias e Poderes;
- uso de Poderes na mesma posição mecânica das Perícias;
- Valor de Ação;
- cinco Patamares;
- orçamentos separados de Atributos, Perícias e Poderes.

Vida, Mana, recursos e combate serão consolidados em arquivos seguintes.

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

> **O Jogador decide o que sua personagem tenta fazer e usa a ficha como interface principal. NPCs usam a mesma lógica, com o nível de detalhe necessário para funcionar.**
