# Dissipar

Dissipar causa dano estrutural a efeitos persistentes dentro de seu repertório.

## Manifestação-base

`Dissipar → Médio / 1 alvo / Pontual / Instantâneo / 1 STATUS`

## Quantidade de STATUS

`1 STATUS [base] → +0` | `2 → +1` | `4 → +2` | `6 → +3` | `16 → +4` | `32 → +5`

STATUS, Alvos e Área são dimensões diferentes. STATUS indica quantas instâncias persistentes podem ser atacadas pela aplicação.

## Resolução

Cada STATUS atingido resolve separadamente.

`Dissipar efetivo = patamar de Dissipar usado + 1 + (Perícia aplicável × 0,2)`

Sem Perícia aplicável:

`Dissipar efetivo = patamar de Dissipar usado + 1`

A resistência é o `D` da instância persistente atingida:

`Dano estrutural = 2^(Dissipar efetivo − D do efeito)`

O Dano estrutural reduz diretamente o `V` atual da instância.

`V ≤ 0 → efeito termina`

Cada STATUS resolve com seus próprios valores de `D` e `V`. Pode atingir efeitos benéficos ou prejudiciais, desde que o repertório da capacidade permita.

## Persistência

Dissipar é instantâneo. Depois da aplicação permanece apenas a redução de `V` ou o encerramento da instância atingida; não existe um efeito persistente de Dissipar.

Ampliações gerais usam `../consolidacao.md`.