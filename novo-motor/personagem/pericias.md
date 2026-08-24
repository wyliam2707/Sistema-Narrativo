# Perícias

Status: EM DESENVOLVIMENTO

Perícias representam treinamento, conhecimento, experiência e capacidade prática aplicada às ações do personagem.

Todas as Perícias começam em `[0]`.

`[0]` não significa incapacidade. Representa aquilo que uma pessoa comum pode realizar com conhecimento cotidiano, improvisação ou experiência básica.

```text
1 ponto de Perícia = +1 nível na Perícia
Máximo absoluto de uma Perícia = [5]
```

As Perícias são divididas em três categorias, cada uma com 8 Perícias:

```text
NÃO TREINADAS
TREINADAS
COMBATE
```

## Não Treinadas

São áreas em que o uso cotidiano continua plausível mesmo em `[0]`. Níveis maiores representam experiência, prática e treinamento crescente.

### Esportes
Capacidade de correr, saltar, nadar, escalar e realizar esforços físicos com técnica.

### Exploração
Orientar-se, atravessar ambientes, procurar caminhos e lidar com obstáculos do terreno.

### Expressão
Comunicar ideias, emoções e intenções por fala, atuação, arte ou presença.

### Sociedade
Lidar com pessoas, costumes, etiqueta, negociação e situações sociais.

### Investigação
Procurar pistas, relacionar informações e reconstruir o que aconteceu.

### Crime
Conhecer práticas clandestinas, segurança, furtividade, invasão e atividades criminosas.

### Ofícios
Criar, reparar e manipular objetos por meio de trabalhos e técnicas manuais.

### Idiomas
Compreender, falar, ler ou interpretar línguas e formas de comunicação.

## Treinadas

Em `[0]`, permitem apenas aquilo que uma pessoa comum poderia plausivelmente fazer no cotidiano. Ações realmente técnicas ou especializadas exigem níveis maiores.

### Arcano
Conhecimento técnico sobre magia, seus princípios, estruturas e funcionamento.

### Ocultismo
Conhecimento sobre fenômenos sobrenaturais, entidades, rituais, símbolos e tradições ocultas.

### Natureza
Conhecimento especializado sobre animais, plantas, ecossistemas e fenômenos naturais.

### Medicina
Conhecimento sobre corpo, ferimentos, doenças, diagnóstico e tratamento.

Em `[0]`, ainda permite cuidados cotidianos simples, como limpar um ferimento, trocar um curativo ou aplicar antisséptico.

### Engenharia
Projetar, compreender, construir e reparar estruturas, máquinas e sistemas mecânicos.

### Ciência
Aplicar conhecimento científico, análise técnica, experimentação e teoria.

### Tecnologia
Compreender, operar, programar e manipular sistemas eletrônicos e digitais.

### História
Conhecer acontecimentos, culturas, povos, organizações e registros do passado.

## Combate

Perícias de Combate representam treinamento aplicado diretamente a ataques, concentração e defesas.

### Luta
Treinamento para executar e enfrentar ataques corpo a corpo.

### Disparo
Treinamento para executar ataques à distância com armas ou efeitos equivalentes.

### Magia
Treinamento para executar efeitos mágicos diretos, como raios, projéteis, explosões, barreiras ou outras manifestações mágicas aplicadas de forma imediata.

### Foco
Capacidade de concentração e controle mental usada para sustentar efeitos que exigem atenção contínua e para aplicar efeitos que atuam diretamente sobre a mente.

Inclui, quando pertinente:

- manter magias de concentração;
- telepatia;
- controle mental;
- influência psíquica;
- invasão ou pressão mental;
- outros efeitos que dependam de concentração contínua.

### Esquiva
Treinamento para evitar ataques, áreas perigosas e ameaças físicas imediatas.

### Percepção
Capacidade treinada de detectar ameaças, emboscadas, furtividade e perigos ocultos.

### Fortitude
Capacidade de resistir a efeitos que atacam ou debilitam o corpo.

### Vontade
Capacidade de resistir a medo, controle, influência e agressões mentais.

## Escala de Poder e pontos de Perícia

A Escala de Poder determina três pacotes de pontos de Perícia.

O jogador decide qual dos três pacotes será destinado a cada categoria:

```text
Não Treinadas
Treinadas
Combate
```

Cada categoria deve receber exatamente um dos pacotes disponíveis para a Escala do personagem.

| Escala de Poder | Pacotes disponíveis | Máximo por Perícia |
|---|---:|---:|
| **[0]** | 2 / 1 / 0 | 1 |
| **[1]** | 4 / 3 / 2 | 1 |
| **[2]** | 8 / 6 / 4 | 2 |
| **[3]** | 12 / 9 / 6 | 3 |
| **[4]** | 16 / 12 / 8 | 4 |
| **[5]** | 20 / 15 / 10 | 5 |
| **[6]** | 24 / 18 / 12 | 5 |
| **[7]** | 28 / 21 / 14 | 5 |

Exemplo para um personagem de Escala `[5]`:

```text
Pacotes disponíveis: 20 / 15 / 10

Jogador escolhe:
Não Treinadas → 15
Treinadas     → 10
Combate       → 20
```

Os pontos são então distribuídos livremente entre as 8 Perícias da respectiva categoria, respeitando o limite individual da Escala.

A regra de limite é:

```text
Escala [0] → máximo [1]
Escala [1] → máximo [1]
Escala [2] → máximo [2]
Escala [3] → máximo [3]
Escala [4] → máximo [4]
Escala [5] → máximo [5]
Escala [6] → máximo [5]
Escala [7] → máximo [5]
```

Escalas `[6]` e `[7]` aumentam a amplitude de treinamento do personagem, permitindo distribuir mais pontos entre as Perícias, mas não criam Perícias `[6]` ou `[7]`.

## Uma ação pode aceitar Perícias diferentes

Não existe a regra `ação X = Perícia X`.

A situação apresenta um problema. A abordagem do personagem determina quais Perícias podem ser coerentes.

Exemplo:

```text
Seguir rastros

Exploração
→ acompanhar terreno, direção, deslocamento e sinais de passagem.

Investigação
→ analisar marcas, padrões, interrupções e inconsistências.

Natureza
→ interpretar vegetação, pegadas, comportamento animal e sinais naturais.
```

> **A ação define o problema. A abordagem define a Perícia aplicável.**

## Atributo e Perícia

A Perícia não fica presa permanentemente a um único Atributo. O Atributo usado depende da natureza da ação.

Exemplo:

```text
Esportes + POD Corpo
→ aplicar potência física com técnica.

Esportes + HAB Corpo
→ correr, saltar, nadar ou executar movimento técnico.

Esportes + RES Corpo
→ sustentar esforço prolongado.
```

As fórmulas específicas de ataque, defesa e resolução pertencem à camada de `../resolucao/` e aos Valores Derivados correspondentes.
