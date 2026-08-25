# Poderes

Esta pasta reúne a estrutura básica dos **Poderes** do novo motor.

Por enquanto, este arquivo registra apenas a base já aprovada para não misturar resolução, alcance, área e ampliações antes de cada parte ser definida.

## Estrutura geral

Um Poder pode possuir **Dano**, **Efeito** ou ambos.

Esses componentes são resolvidos em etapas próprias.

A sequência padrão dos Poderes ofensivos é:

> **Defesa → Dano → Resistência → Efeito**

Nem todo Poder precisa usar todas essas etapas. Poderes como **Portal, Invocação, Teleporte, Barreira, Cura, Detecção** e outros efeitos não ofensivos usam apenas as etapas que fizerem sentido para sua própria natureza.

## Distâncias narrativas

As distâncias dos Poderes são tratadas de forma **narrativa**. Os valores em metros são médias de referência para ajudar o Narrador a interpretar a cena com consistência, e não uma régua rígida.

A escala é:

- **Si Mesmo** — apenas o próprio usuário.
- **Toque** — exige contato físico.
- **Próximo** — cerca de **3 m**; poucos passos, alcance imediato dentro da cena.
- **Curto** — cerca de **20 m**; uma distância pequena e claramente próxima dentro da cena.
- **Médio** — cerca de **45 m**; uma distância significativa, mas ainda claramente presente na cena.
- **Longo** — cerca de **90 m**; uma distância distante dentro da cena.

Acima de **Longo**, a distância deixa de ser tratada como alcance comum e passa a depender de Poderes próprios, como **Teleporte**, **Portal** ou outros efeitos capazes de atravessar grandes distâncias.

Quando uma dessas categorias aparecer em **Alcance** ou **Área**, o Narrador usa essa média como referência e interpreta a posição real conforme a ficção.

## Defesa

A Defesa é resolvida antes do Dano e da Resistência do Efeito.

Quando houver uma disputa defensiva, a base é:

**Defesa:** `Controle × Controle`

- O usuário usa **Controle** para acertar ou aplicar o ataque.
- O alvo usa **Controle** para evitar ou se defender da ação.

Cada Poder indica qual tipo de Defesa possui.

### Defesa [Absoluta]

Se a defesa vencer:

- o alvo **não sofre Dano**;
- o **Efeito é anulado** e não segue para a etapa de Resistência.

Representa uma defesa capaz de evitar completamente o ataque.

### Defesa [Total]

Se a defesa vencer:

- o alvo **não sofre Dano**;
- o **Efeito ainda segue para a etapa de Resistência**.

### Defesa [Parcial]

Se a defesa vencer:

- o alvo sofre **metade do Dano**;
- o **Efeito ainda segue para a etapa de Resistência**.

### Defesa [Nula]

Não existe defesa aplicável nessa etapa.

- o Dano é aplicado normalmente;
- o **Efeito segue para a etapa de Resistência**.

**Defesa [Nula] não significa que toda ação é automaticamente possível.** A ficção ainda determina se existe alvo, alcance, linha de ação ou qualquer outra condição necessária para o Poder funcionar.

## Dano

O Dano é aplicado depois da Defesa.

O resultado da Defesa determina se o alvo sofre:

- **Dano normal**;
- **metade do Dano**;
- **nenhum Dano**.

A progressão básica de Dano é:

`1d8 → 2d8 → 3d8 → 4d8 → 5d8`

O primeiro passo da progressão não aumenta o custo. Cada avanço posterior acrescenta `+1` ao custo.

## Resistência do Efeito

Se o Efeito não tiver sido anulado pela Defesa, ele segue para uma resolução própria.

Quando houver Resistência, a base é:

**Efeito:** `Potência × Resistência`

- o usuário usa **Potência** para impor o Efeito;
- o alvo usa **Resistência** para suportar ou reduzir o Efeito.

A Resistência só é resolvida depois da Defesa.

Cada Poder indica qual tipo de Resistência seu Efeito possui.

### Efeito [Total]

Se a Resistência vencer, o **Efeito é anulado**.

Nenhum efeito da progressão é aplicado.

### Efeito [Parcial]

Se a Resistência vencer, o Efeito é reduzido em **uma posição na progressão**.

Exemplo:

**Contenção:** `Lento → Imóvel → Paralisado`

Se o Poder tentar aplicar **Paralisado** e a Resistência vencer, aplica **Imóvel**.

Se o Poder tentar aplicar **Imóvel** e a Resistência vencer, aplica **Lento**.

Se o Poder tentar aplicar o primeiro efeito da progressão e a Resistência vencer, **nenhum Efeito é aplicado**.

### Efeito [Nula]

Não existe Resistência aplicável nessa etapa.

Se o Efeito chegar a essa etapa da resolução, ele é aplicado conforme sua própria definição e progressão.

**Efeito [Nula] não ignora as exigências da ficção.** O Poder ainda precisa possuir alvo, alcance e demais condições necessárias para produzir o Efeito.

## Efeito

O Efeito utiliza as famílias e progressões apropriadas do sistema.

Quando a Resistência não vencer, o efeito pretendido é aplicado normalmente.

Quando o Poder possuir **Efeito [Parcial]**, uma Resistência bem-sucedida reduz o resultado em uma posição da progressão. Quando possuir **Efeito [Total]**, uma Resistência bem-sucedida anula o resultado. Em **Efeito [Nula]**, não existe essa etapa de Resistência.

## Dano e Efeito no mesmo Poder

Um mesmo Poder pode possuir Dano e Efeito.

A resolução segue a ordem:

1. resolve-se a **Defesa**;
2. aplica-se o **Dano** conforme o tipo de Defesa e seu resultado;
3. se o Efeito ainda puder ocorrer e possuir Resistência, resolve-se `Potência × Resistência`;
4. aplica-se o **Efeito** conforme seu tipo de Resistência e o resultado obtido.

Assim, um Poder pode causar Dano sem conseguir impor o Efeito, pode não causar Dano mas ainda tentar impor o Efeito, ou pode ter ambos anulados por uma Defesa apropriada.

## Função dos Atributos

- **Controle** representa a capacidade de acertar ou evitar um ataque.
- **Potência** representa a capacidade de impor a intensidade de um Efeito.
- **Resistência** representa a capacidade de suportar ou resistir ao Efeito recebido.
- O **maior Atributo Físico** do personagem é a referência para limitar o gasto de Mana/Energia do Poder. Essa regra ainda será detalhada em seção própria.

## Progressões já definidas

Alguns campos dos Poderes usam progressões. O primeiro passo da progressão não aumenta o custo; cada avanço posterior acrescenta `+1` ao custo.

### Alcance

`Si Mesmo → Toque → Próximo → Curto → Médio → Longo`

As posições usadas e seus custos dependem da progressão apresentada em cada Poder.

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
