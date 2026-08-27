# Defesas em Faixas

Status: RASCUNHO / NÃO IMPLEMENTADO

## Ideia central

As Defesas são valores fixos e já calculados na ficha. O jogador não recalcula Atributos durante o combate.

Uma Defesa pode possuir **dois limiares** derivados de um Atributo apropriado.

Exemplo em estudo:

```text
DEFESA
8 + DES
12 + DES
```

A Defesa é usada contra ataques físicos baseados em FOR ou DES, conforme o Poder ou ataque utilizado.

## Leitura preliminar das faixas

Uma única rolagem de ataque determina a eficiência do golpe conforme o limiar alcançado.

```text
resultado abaixo de 8 + DES
→ sem Dano

resultado de 8 + DES até 11 + DES
→ metade do Dano

resultado igual ou superior a 12 + DES
→ Dano normal
```

Assim, a Defesa possui apenas três resultados relevantes:

```text
falha
→ 0 Dano

acerto parcial
→ 1/2 Dano

acerto completo
→ Dano normal
```

## Exemplo

Personagem com DES 4:

```text
Defesa
12 / 16
```

Ataque total 11 ou menos
→ sem Dano

Ataque total 12–15
→ metade do Dano

Ataque total 16+
→ Dano normal
```

## Objetivo

A ideia busca substituir múltiplas etapas defensivas por uma única comparação:

```text
rola ataque uma vez
→ compara com os dois limiares já impressos na ficha
→ identifica a faixa alcançada
→ aplica diretamente a consequência
```

Isso permite que Defesa, Reflexos, Fortitude e Vontade sigam uma lógica semelhante, cada uma com Atributo-base e uso próprios a definir.

## Relação com Poderes

Cada Poder já deve indicar:

- qual Atributo usa para sua rolagem;
- qual Defesa ou Resistência enfrenta;
- seu Dano ou Efeito;
- qual consequência ocorre nas faixas, quando houver exceção à regra geral.

Exemplo conceitual:

```text
Bola de Fogo
Atributo: INT
Ataque: 1d20 + INT
Resistência: Reflexos
Dano: 3d6 + INT
```

A rolagem contra Reflexos determina se o alvo evita o efeito, sofre efeito reduzido ou sofre o efeito normal.

## Questões em aberto

- definir os Atributos-base de Defesa, Reflexos, Fortitude e Vontade;
- confirmar se todos usam os mesmos deslocamentos `8 / 12`;
- decidir se existe crítico ou efeito máximo acima do Dano normal;
- definir como poderes sem Dano usam as faixas parcial/total;
- verificar matematicamente probabilidades entre Atributos de 0 a 10.

> **Este documento registra apenas uma hipótese de motor. Não altera as regras aprovadas.**
