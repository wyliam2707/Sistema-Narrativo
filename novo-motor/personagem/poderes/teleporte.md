# Teleporte

## HUD

```text
Teleporte [X]
Alcance: Toque
Alvo: Si mesmo > Toque [+1]
Distância: Cidade > Estado [+1] > País [+2] > Planeta [+3]
Local: Conhecido > Visitado [+1] > Descrição [+2]
Defesa: Foco × Vontade → somente se o alvo resistir
Duração: Instantâneo
```

## Resolução

`[X]` é o máximo de Mana que pode ser gasto neste Poder em uma única utilização.

```text
Mínimo: [1]
Máximo: [5]
```

O efeito-base custa `0 Mana`.

Cada passo de uma progressão aumenta o custo em `+1 Mana`. O valor `[+X]` indica o custo total daquele nível, não a soma dos níveis anteriores.

Ampliações de linhas diferentes podem ser combinadas, mas a soma de Mana gasta no uso não pode ultrapassar `[X]`.

Em uma mesma linha, usa-se apenas um dos níveis disponíveis.

### Defesa

Se o alvo aceitar o Teleporte, não há teste de Defesa.

Se o alvo resistir, resolver `Foco × Vontade`.

- Foco vence ou empata: o alvo é transportado.
- Vontade vence: o alvo não é transportado.

O narrador nunca escolhe automaticamente uma ampliação que consuma Mana. Quando a intenção declarada exigir uma ampliação, informa o custo e aguarda confirmação antes de gastar Mana.