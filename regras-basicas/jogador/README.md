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

Define exclusivamente:

- os seis Atributos;
- as quatorze Perícias;
- graduações de `0` a `+3`;
- testes com `Atributo + Perícia`;
- orçamentos de Atributos `6 / 8 / 10 / 12 / 14`;
- orçamentos de Perícias `6 / 9 / 12 / 15 / 18`;
- Patamares de construção.

Poderes e equipamentos não são definidos neste arquivo.

## `1.2-poderes-e-equipamentos.md`

Define a regra de Poderes e equipamentos:

- Poder é uma opção de ação;
- graduação `[1]` a `[3]` mede a força da capacidade;
- testes continuam usando `Atributo + Perícia`;
- Poder não é somado ao teste técnico;
- quando sua força importa, a graduação entra depois na Potência ou Resistência conforme o Núcleo;
- nunca usar `Atributo + Perícia + Poder`;
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

> **Complexidade na construção; simplicidade na mesa. Testes usam Atributo + Perícia; Poderes ampliam o que a personagem pode fazer e entram na força do efeito sem criar um terceiro fator no teste.**
