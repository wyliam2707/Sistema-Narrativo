# Passivos

Status: EM DESENVOLVIMENTO

Passivos são efeitos permanentes ou estáveis já incorporados ao personagem. Eles não são escolhidos a cada ação e não usam a regra de limite de Energia dos Poderes ativos.

> **Poder ativo é escolhido e usado. Passivo já faz parte do personagem.**

## `[X]` nos Passivos

Quando um Passivo possui um valor entre colchetes, o próprio arquivo define o significado desse valor.

```text
RD [3] → reduz 3 de dano.
Vida Extra [30] → +30 Vida máxima.
Proteção [2] → +2 Esquiva e +2 Percepção.
Regeneração [2] → recupera 2 de Vida por hora.
```

`[X]` em Passivos não representa máximo de Energia por uso.

## Consolidação na ficha

Passivos que alteram valores derivados já entram no total final mostrado em `Derivados`.

```text
Passivos
RD [3]
Vida Extra [30]
Proteção [2]

Derivados
Vida: [base + 30]
Esquiva: [base + 2]
Percepção: [base + 2]
RD: 3
```

Passivos que não alteram um número permanecem registrados na ficha e são consultados quando a situação correspondente surgir.

## Arquivos individuais

Cada Passivo possui arquivo próprio em `passivos/`:

- `rd.md`
- `vida-extra.md`
- `protecao.md`
- `sentido-aranha.md`
- `imortalidade.md`
- `regeneracao.md`

A origem narrativa do Passivo não altera sua mecânica. Um mesmo efeito pode representar armadura, mutação, magia, tecnologia, treinamento ou outra justificativa coerente.
