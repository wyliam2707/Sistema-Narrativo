# Passivos

Status: EM DESENVOLVIMENTO

Passivos são efeitos permanentes ou estáveis que já fazem parte do personagem. Eles não são escolhidos a cada ação e não consomem Energia para funcionar, salvo se a própria descrição disser o contrário.

> **Poder ativo é escolhido e usado. Passivo já está incorporado ao personagem.**

Um Passivo pode ter um valor entre colchetes quando sua própria regra precisar de uma graduação ou valor fixo. Diferente dos Poderes ativos, o valor `[X]` de um Passivo **não representa limite de Energia por uso**.

## RD [X]

```text
RD [X]
Efeito: reduz em X o dano recebido.
```

Exemplo:

```text
RD [3]
→ reduz em 3 o dano recebido.
```

## Vida Extra [X]

```text
Vida Extra [X]
Efeito: +X à Vida máxima.
```

Exemplo:

```text
Vida Extra [30]
→ +30 Vida.
```

## Proteção [X]

```text
Proteção [X]
Efeito:
+X à Esquiva
+X à Percepção
```

Exemplo:

```text
Proteção [2]
→ +2 Esquiva
→ +2 Percepção
```

## Sentido-Aranha

```text
Sentido-Aranha
Efeito: o personagem não pode ser pego desprevenido.
```

Esse Passivo representa percepção antecipada de perigo. Sua origem narrativa pode ser precognição, instinto sobrenatural, sentidos ampliados ou outra justificativa coerente.

## Imortalidade

```text
Imortalidade
Efeito: o personagem não morre de velhice.
```

Imortalidade não impede dano, ferimentos ou morte por outras causas. Ela apenas elimina a morte causada pelo envelhecimento.

## Regeneração [X]

```text
Regeneração [X]
Efeito: recupera X de Vida por hora.
```

Exemplo:

```text
Regeneração [2]
→ recupera 2 de Vida por hora.
```

## Consolidação

Os Passivos aparecem diretamente na ficha. Quando alteram valores derivados, seus efeitos já entram no valor final.

Exemplo:

```text
Passivos
RD [3]
Vida Extra [30]
Proteção [2]
Sentido-Aranha
Imortalidade
Regeneração [2]

Derivados
Vida: [base + 30]
Esquiva: [base + 2]
Percepção: [base + 2]
RD: 3
```

Passivos que não alteram um número derivado permanecem registrados como propriedades do personagem e são consultados somente quando a situação correspondente surgir.

A origem narrativa do Passivo não altera sua mecânica. `RD [3]`, por exemplo, pode representar armadura, pele sobrenatural, traje tecnológico, campo místico ou qualquer outra justificativa coerente com o personagem.
