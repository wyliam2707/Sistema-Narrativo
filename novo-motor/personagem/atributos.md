# Atributos

Status: EM DESENVOLVIMENTO

O `novo-motor/` usa seis Atributos organizados em dois domínios espelhados: Corpo e Mente.

```text
Corpo — POD [X] | HAB [X] | RES [X]
Mente — POD [X] | HAB [X] | RES [X]
```

Cada domínio usa as mesmas três funções:

```text
POD → Poder: intensidade e potência.
HAB → Habilidade: execução, precisão e controle.
RES → Resistência: capacidade de suportar e resistir.
```

O domínio define a natureza da capacidade:

```text
Corpo → capacidades físicas.
Mente → capacidades mentais, sociais, psíquicas ou mágicas quando pertinente.
```

## Corpo

### POD Corpo

Representa potência física.

Pode determinar, conforme a regra usada:

- força aplicada;
- potência de ataques corporais;
- dano de Poderes físicos que acrescentem POD Corpo;
- capacidade física exigida por uma ação ou manifestação.

### HAB Corpo

Representa execução física.

Inclui, quando pertinente:

- precisão;
- coordenação;
- reflexos;
- mobilidade;
- equilíbrio;
- técnica corporal;
- acerto de ataques físicos.

### RES Corpo

Representa resistência física.

Inclui, quando pertinente:

- suportar impacto e dano;
- fadiga e esforço prolongado;
- veneno, doença e outros efeitos corporais;
- continuar funcionando sob desgaste físico.

## Mente

### POD Mente

Representa potência mental, social, psíquica ou mágica quando a capacidade depender da força do personagem.

Pode determinar, conforme a regra usada:

- intensidade de uma imposição mental;
- potência de efeitos mágicos ou psíquicos;
- dano de Poderes que acrescentem POD Mente;
- capacidade de sustentar uma manifestação mental ou mágica.

### HAB Mente

Representa execução mental.

Inclui, quando pertinente:

- percepção;
- raciocínio;
- análise;
- controle;
- precisão mental;
- acerto ou aplicação de efeitos mágicos e psíquicos.

### RES Mente

Representa resistência mental.

Inclui, quando pertinente:

- medo;
- dominação;
- pressão psicológica;
- manipulação mental;
- manutenção da própria integridade mental sob efeitos externos.

## Escala de Poder e pontos de Atributo

A Escala de Poder do personagem determina dois limites durante a criação:

1. quantos pontos totais podem ser distribuídos entre os seis Atributos;
2. qual é o valor máximo permitido em cada Atributo.

A Escala de Poder não é um Atributo e não entra diretamente em testes. Ela serve como referência de construção do personagem.

| Escala de Poder | Pontos de Atributo | Máximo por Atributo |
|---|---:|---:|
| **[0]** | 1 | 1 |
| **[1]** | 4 | 1 |
| **[2]** | 8 | 2 |
| **[3]** | 12 | 3 |
| **[4]** | 16 | 4 |
| **[5]** | 20 | 5 |
| **[6]** | 25 | 6 |
| **[7]** | 30 | 7 |

Regra geral:

```text
Máximo por Atributo = Escala de Poder
```

A única exceção é a Escala de Poder `[0]`, que possui 1 ponto de Atributo e permite valor máximo `[1]` para que esse ponto possa ser distribuído.

Os pontos podem ser distribuídos livremente entre:

```text
POD Corpo
HAB Corpo
RES Corpo
POD Mente
HAB Mente
RES Mente
```

desde que o total disponível e o limite individual da Escala de Poder sejam respeitados.

Exemplo de Escala de Poder `[7]`:

```text
Corpo — POD [7] | HAB [5] | RES [6]
Mente — POD [5] | HAB [4] | RES [3]

Total: 30 pontos
```

A Escala de Poder `[7]` permite chegar a `[7]` em um Atributo, mas não obriga nenhum Atributo a atingir esse valor.

`[0]` é um valor real e representa capacidade comum dentro da escala; não significa campo desconhecido.

Campos ainda não definidos permanecem vazios na ficha.

## Função mecânica

A separação central é:

```text
POD → quanto consegue produzir ou impor.
HAB → quão bem consegue executar ou aplicar.
RES → quanto consegue suportar ou resistir.
```

POD e HAB não devem ser somados automaticamente para cumprir a mesma função.

Exemplo conceitual:

```text
Acerto físico → HAB Corpo.
Dano físico dependente do usuário → POD Corpo.
Acerto mágico → HAB Mente.
Potência de efeito mágico → POD Mente.
```

As fórmulas de testes, Defesas e combate pertencem à camada de `../resolucao/` e só devem ser aplicadas quando estiverem compatíveis com a arquitetura consolidada do novo motor.

> **Poder determina intensidade. Habilidade determina execução. Resistência determina oposição. Corpo e Mente determinam a natureza da capacidade.**
