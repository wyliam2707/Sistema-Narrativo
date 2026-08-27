# Defesas em Faixas

Status: RASCUNHO / NÃO IMPLEMENTADO

## Ideia central

As Defesas são valores fixos e já calculados na ficha. O jogador não recalcula Atributos durante o combate.

Uma Defesa pode possuir três limiares derivados de um Atributo apropriado.

Exemplo em estudo:

```text
DEFESA
8 + DES
10 + DES
12 + DES
```

A Defesa é usada contra ataques físicos baseados em FOR ou DES, conforme o Poder ou ataque utilizado.

## Leitura preliminar das faixas

A proposta discutida é que uma única rolagem de ataque determine a eficiência do golpe conforme o limiar alcançado.

```text
resultado abaixo de 8 + DES
→ falha completa

resultado alcança 8 + DES, mas não 10 + DES
→ defesa suficiente para não sofrer Dano

resultado alcança 10 + DES, mas não 12 + DES
→ sofre metade do Dano

resultado alcança 12 + DES ou mais
→ sofre Dano normal
```

A faixa de `8 + DES` precisa ter uma função distinta da falha completa para justificar existir. Ela pode representar contato defendido, bloqueio, raspão sem Dano ou outro resultado ficcional/mecânico. Caso essa distinção não seja útil, os limiares podem ser simplificados posteriormente.

## Exemplo

Personagem com DES 4:

```text
Defesa
12 / 14 / 16
```

Ataque total 11
→ falha completa

Ataque total 12–13
→ atinge a primeira faixa, mas não causa Dano

Ataque total 14–15
→ metade do Dano

Ataque total 16+
→ Dano normal
```

## Objetivo

A ideia busca substituir múltiplas etapas defensivas por uma única comparação:

```text
rola ataque uma vez
→ compara com os limiares já impressos na ficha
→ identifica a faixa alcançada
→ aplica diretamente a consequência
```

Isso permite que Defesa, Reflexos, Fortitude e Vontade sigam uma lógica semelhante, cada uma com Atributo-base e uso próprios a definir.

## Relação com Poderes

Cada Poder já deve indicar:

- qual Atributo usa para sua rolagem;
- qual Defesa ou Resistência enfrenta;
- seu Dano ou Efeito;
- qual consequência ocorre em cada faixa, quando houver exceção à regra geral.

Exemplo conceitual:

```text
Bola de Fogo
Atributo: INT
Ataque: 1d20 + INT
Resistência: Reflexos
Dano: 3d6 + INT
```

A rolagem contra Reflexos determina se o alvo evita, sofre efeito reduzido ou sofre o efeito normal.

## Questões em aberto

- confirmar se a primeira faixa (`8 + atributo`) produz contato sem Dano ou se deve ser removida;
- definir os Atributos-base de Defesa, Reflexos, Fortitude e Vontade;
- definir se todos usam os mesmos deslocamentos `8 / 10 / 12`;
- decidir se existe uma faixa acima do Dano normal para crítico/efeito máximo;
- definir como ataques sem Dano interagem com a primeira faixa;
- verificar matematicamente probabilidades entre Atributos de 0 a 10.

> **Este documento registra apenas uma hipótese de motor. Não altera as regras aprovadas.**
