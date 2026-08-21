# Escalas de Capacidade

Status: EM REVISÃO

Este arquivo consolida as escalas numéricas usadas na definição de personagens.

## Escala universal de atributos e poderes — 0 a 5

A mesma escala conceitual é usada para atributos e poderes.

| Grau | Referência narrativa |
|---|---|
| **0** | Humano |
| **1** | Além do humano |
| **2** | Super-humano claro |
| **3** | Poderoso |
| **4** | Extremo |
| **5** | Ápice daquela capacidade |

O grau não é uma medida física exata.

Não existe obrigação de converter, por exemplo, `FOR [3]` em toneladas ou `Sentidos [4]` em uma distância fixa.

O número informa o grau de excepcionalidade daquela capacidade dentro de sua própria categoria.

Exemplos herdados da regra antiga:

- `FOR [5]` = força em patamar extremo de referência, como Superman/Hulk;
- `Cura [5]` = cura em patamar igualmente extremo, se o conceito do poder permitir;
- `Sentidos Ampliados [5]` = percepção em escala extrema;
- `Portal [5]` = capacidade de portais em escala extrema.

> **5 sempre precisa parecer 5.**

Duas capacidades no mesmo grau não fazem a mesma coisa. Elas apenas ocupam posição semelhante de excepcionalidade dentro das próprias categorias.

## Escala de perícias — +0 a +5

Perícias usam uma escala própria:

| Grau | Referência |
|---|---|
| **[+0]** | leigo / sem conhecimento ou treinamento relevante |
| **[+1]** | básico / treinado |
| **[+2]** | profissional |
| **[+3]** | especialista |
| **[+4]** | mestre |
| **[+5]** | ápice daquela área |

O sinal `+` diferencia visualmente perícias das capacidades graduadas na escala universal.

Uma perícia não listada é normalmente tratada como `[+0]` quando for necessário avaliar aquele campo.

## Zero é um valor real

Durante criação ou revisão, um campo ainda desconhecido deve ficar em branco.

> **Nunca usar `[0]` ou `[+0]` como marcador de informação ainda não definida.**

`[0]` e `[+0]` possuem significado mecânico próprio.

## Calibração conservadora

Quando houver dúvida real entre dois graus adjacentes durante a conversão de uma capacidade, usar o menor.

Exemplos:

```text
dúvida entre [2] e [3] → [2]
dúvida entre [3] e [4] → [3]
```

A mesma lógica vale para atributos, perícias, poderes e especializações quando aplicável.

`[5]` permanece reservado ao verdadeiro ápice da categoria.

A regra completa de conversão está em `calibracao.md`.
