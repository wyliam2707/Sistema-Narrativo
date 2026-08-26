# Relações

Status: APROVADO

`REL` registra vínculos **recorrentes e consolidados** que fazem parte da vida atual da personagem.

> **Relação descreve o vínculo; não decide comportamento, não concede obediência e não é bônus automático.**

## Forma

```text
REL: Nome [grau] — natureza do vínculo
```

Exemplos:

```text
REL: Alfred [+4] — família / confiança
REL: Gordon [+3] — aliado / confiança
REL: Liga dos Assassinos [-3] — hostilidade
```

## O que o grau representa

O grau registra:

- direção predominante;
- intensidade do vínculo.

A natureza permanece narrativa.

| Grau | Referência |
|---|---|
| **-5** | vínculo hostil extremo |
| **-4** | hostilidade profunda |
| **-3** | hostilidade forte |
| **-2** | vínculo desfavorável |
| **-1** | vínculo levemente desfavorável |
| **0** | neutro |
| **+1** | vínculo levemente favorável |
| **+2** | vínculo favorável |
| **+3** | vínculo forte |
| **+4** | vínculo profundo |
| **+5** | vínculo positivo máximo |

Um mesmo grau pode representar amizade, família, amor, rivalidade, lealdade, medo ou outra forma de vínculo.

## Ambivalência

Uma relação pode conter sentimentos contraditórios:

```text
REL: Selina [+3] — afeto / atração / desconfiança
REL: Irmão [+4] — amor / ressentimento
```

Não é necessário criar dois valores apenas porque o vínculo é complexo.

## Relações são direcionais

```text
A → B [+4]
B → A [+2]
```

A relação de A com B não precisa ser igual à de B com A.

Durante a criação, a consistência entre as duas fichas é verificada por `../criacao/pareamento.md`.

## Pessoas e organizações

`REL` pode registrar pessoa ou organização quando o vínculo for recorrente e relevante.

```text
REL: Polícia de Gotham [+2] — cooperação
```

Quando o alvo é uma organização, o grau representa a relação predominante com o grupo; não obriga todos os indivíduos daquela organização a reagirem da mesma maneira.

## REL não controla comportamento

Um grau favorável pode criar contexto, confiança ou oportunidade quando a ficção realmente sustentar isso, mas não concede automaticamente:

- acesso;
- favor;
- autoridade;
- obediência;
- sucesso social;
- controle sobre decisão alheia.

Resolução social pertence a `../resolucao/resolucao-social.md`.

Autoridade e decisões voluntárias pertencem a `../personas/`.

## O que entra em REL

Usar `REL` principalmente para vínculos que realmente fazem parte da vida recorrente da personagem:

- família importante;
- amizades recorrentes;
- parceiros;
- rivais permanentes;
- inimigos ativos recorrentes;
- organizações importantes;
- outros vínculos consolidados.

Uma reação circunstancial não vira automaticamente `REL`.

Se uma consequência ainda é apenas causalmente viva, mas não se tornou vínculo recorrente, sua persistência pertence a `../persistencia/progressao.md`.

`REL [0]` só precisa aparecer quando a relação neutra ainda for relevante; relações sem utilidade futura podem simplesmente não ocupar a ficha.

## Pressão e continuidade

Este arquivo não define como relações são usadas para movimentar oposição ou continuidade fora de cena.

Usar:

```text
pressões e ganchos → ../agencia/
quem decide        → ../personas/
onde salvar        → ../persistencia/
```

## Regra final

> **`REL` descreve direção, intensidade e natureza de um vínculo recorrente. A relação informa a ficção; outras áreas determinam agência, resolução e persistência.**
