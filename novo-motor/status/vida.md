# Vida

Vida representa quanto dano e desgaste físico o personagem consegue suportar antes de sofrer as consequências definidas pela regra de Vida.

## Vida Máxima

A Vida Máxima de um personagem é calculada por:

> **Vida = 10 + (Resistência × 4) + (Potência × 2) + (Controle × 2) + Intelecto + Presença + Vontade**

Para esse cálculo, **Atributos negativos contam como 0**. Eles nunca reduzem a Vida abaixo da base por causa de um valor negativo.

Os Atributos contribuem de maneira diferente:

- **Resistência ×4** — principal fator de sobrevivência e durabilidade;
- **Potência ×2** — vigor e capacidade física geral;
- **Controle ×2** — domínio corporal, reação e capacidade de evitar que danos se agravem;
- **Intelecto ×1** — contribuição mental geral;
- **Presença ×1** — contribuição mental geral;
- **Vontade ×1** — contribuição mental geral.

Assim, um personagem com todos os Atributos em `[0]` possui **10 de Vida**.

A Vida Máxima é recalculada quando uma regra permanente alterar os Atributos que entram na fórmula. A interação com alterações temporárias ainda será definida pela regra geral de Atributos temporários.

## 0 Vida

Ao chegar a **0 Vida**, o personagem fica **Incapacitado**.

Incapacitado significa que ele não consegue continuar agindo normalmente na situação. A forma concreta dessa incapacidade depende daquilo que aconteceu na ficção: pode representar inconsciência, colapso, ferimentos graves, imobilização pelo estado físico ou outra consequência coerente.

Chegar a 0 Vida **não significa morte automática**.

## Vida e consequências narrativas

Vida não substitui consequências evidentes da ficção e não funciona como proteção automática contra situações inevitavelmente letais.

Se a própria situação determinar de forma clara que o personagem morreu, a morte pode ocorrer como consequência narrativa, mesmo sem uma regra adicional de dano ou uma redução gradual até 0 Vida.

Exemplo: cair de um avião sem qualquer meio aparente de se salvar ou sobreviver pode ser uma consequência mortal determinada pela própria ficção; não é necessário transformar uma situação evidentemente fatal em sucessivas rolagens de dano apenas para consumir Vida.

Da mesma forma, quando a situação não determinar claramente a morte, chegar a 0 Vida significa **Incapacitado**, e não morto.

## Recuperação natural

Com **descanso válido**, o personagem recupera Vida uma vez por dia conforme sua Resistência:

> **Recuperação diária = Resistência × 2, mínimo 2 de Vida**

A recuperação nunca ultrapassa a Vida Máxima.

Valores baixos ou negativos de Resistência não reduzem essa recuperação abaixo do mínimo de **2 Vida por dia**.

Exemplos:

- Resistência `[-2]`, `[-1]`, `[0]` ou `[1]` → **2 Vida por dia**;
- Resistência `[2]` → **4 Vida por dia**;
- Resistência `[3]` → **6 Vida por dia**;
- Resistência `[4]` → **8 Vida por dia**.

Um descanso só conta quando for válido para aquele personagem. Traços ou condições que definam exigências especiais de repouso, como **Repouso Especial**, também determinam quando essa recuperação pode ocorrer.

## Medicina

Um tratamento realizado através da Perícia **Medicina** pode recuperar Vida conforme o resultado final do teste.

A cada **5 pontos de resultado**, recupera-se **+1 Vida**, até o máximo de **+5 Vida**:

| Resultado do teste | Vida recuperada |
|---:|---:|
| 5 | +1 Vida |
| 10 | +2 Vida |
| 15 | +3 Vida |
| 20 | +4 Vida |
| 25 ou mais | +5 Vida |

Resultados intermediários utilizam o último patamar alcançado. Exemplo: resultado `17` recupera **3 Vida**.

A recuperação por Medicina nunca pode elevar a Vida acima da Vida Máxima.

## Poderes e Traços de recuperação

Poderes e Traços podem recuperar Vida quando sua própria descrição estabelecer isso.

> **Não existe uma quantidade universal de Vida recuperada por Poderes ou Traços. A fonte define sua própria recuperação.**

Assim, um **Poder de Cura** utiliza a quantidade indicada em seu Hub ou descrição, enquanto um **Traço de Recuperação** segue a regra escrita no próprio Traço.

Essas fontes nunca elevam a Vida acima da Vida Máxima, salvo se alguma regra específica declarar expressamente o contrário.

## Dano, arredondamento, Redução de Dano e Barreira

Quando uma regra produzir uma fração, **arredonde sempre para baixo**.

Quando um dano chegar à etapa final de aplicação, ele causa no mínimo **1 ponto de dano**. Reduções não podem diminuir um dano que chegou a essa etapa abaixo de 1.

A ordem completa de aplicação do dano é:

> **Defesa → redução causada pela Defesa → RD → Barreira → Vida**

Assim, quando uma **Defesa [Parcial]** for bem-sucedida, primeiro reduza o dano pela metade e arredonde para baixo. Depois aplique a maior RD válida. O dano restante atinge primeiro qualquer **Barreira** aplicável e somente depois reduz a **Vida**.

Se a Barreira absorver todo o dano restante, a Vida não é reduzida. Se a Barreira chegar a 0 e ainda houver dano excedente, apenas esse excedente passa para a Vida.

Exemplo: um ataque causa `9` de dano contra um alvo que vence uma Defesa [Parcial], possui RD `2` e uma Barreira com `1 PV`:

1. `9 ÷ 2 = 4,5` → arredonda para **4**;
2. `4 - 2 = 2`;
3. a Barreira absorve **1** e é destruída;
4. o **1** excedente reduz a Vida.

Se a RD reduzisse o resultado a `0` ou menos, o dano final ainda seria **1**, desde que o ataque tenha chegado à etapa de dano. Esse dano seria então aplicado primeiro à Barreira, se houver, e depois à Vida.