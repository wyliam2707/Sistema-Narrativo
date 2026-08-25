# Poderes

Esta pasta reúne a estrutura básica dos **Poderes** do novo motor.

Por enquanto, este arquivo registra apenas a base já aprovada para não misturar resolução, alcance, área e ampliações antes de cada parte ser definida.

## Estrutura geral

Um Poder pode possuir **Dano**, **Efeito** ou ambos.

Esses dois componentes são resolvidos de forma separada.

### Dano

**Dano:** `Controle × Controle`

- O usuário usa **Controle** para acertar o alvo.
- O alvo usa **Controle** para evitar o ataque.
- Se o usuário vencer, o Dano do Poder é aplicado.

### Efeito

**Efeito:** `Potência × Resistência`

- O usuário usa **Potência** para impor o efeito.
- O alvo usa **Resistência** para suportar ou impedir o efeito.
- Se o usuário vencer, o Efeito do Poder é aplicado.

### Dano e Efeito no mesmo Poder

Um mesmo Poder pode possuir os dois componentes.

Nesse caso, o Dano e o Efeito são verificados separadamente:

1. `Controle × Controle` resolve o Dano.
2. `Potência × Resistência` resolve o Efeito.

É possível, portanto, que um Poder cause Dano sem conseguir impor o Efeito, imponha o Efeito sem causar Dano, consiga ambos ou falhe nos dois componentes, conforme as resoluções.

## Função dos Atributos

- **Controle** representa a capacidade de acertar ou evitar um ataque.
- **Potência** representa a capacidade de impor a intensidade de um efeito.
- **Resistência** representa a capacidade de suportar ou resistir ao efeito recebido.
- O **maior Atributo Físico** do personagem será usado como referência para limitar o gasto de Mana/Energia do Poder; essa regra ainda será detalhada em seção própria.

## Progressões já definidas

Alguns campos dos Poderes usam progressões. O primeiro passo da progressão não aumenta o custo; cada avanço posterior acrescenta `+1` ao custo.

### Alcance

`Toque → Próximo → Curto → Médio → Longo`

### Dano

`1d8 → 2d8 → 3d8 → 4d8 → 5d8`

As limitações exatas dessas progressões pelos Atributos ainda serão definidas.

## Campos de um Poder

A estrutura planejada para cada Poder básico é:

- **Ação**
- **Alcance**
- **Alvos**
- **Efeito**
- **Acerto**
- **Defesa**
- **Observação**

Esses campos serão detalhados um por vez.
