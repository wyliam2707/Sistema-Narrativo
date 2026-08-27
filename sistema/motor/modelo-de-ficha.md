# Modelo de Ficha — Rascunho

Status: RASCUNHO / NÃO IMPLEMENTADO

Objetivo: testar uma ficha física de uma página em que os valores usados durante a sessão já estejam calculados. Os Atributos servem de base para construir os demais números, mas não são rolados diretamente.

## Estrutura proposta

```text
BLOCO [1]
┌─────────────────────────────────────────────────────────────────────┐
│ NOME __________________________  CONTROLE _________________________ │
│ IMPORTÂNCIA ___________________  PATAMAR [   ]                     │
└─────────────────────────────────────────────────────────────────────┘

ATRIBUTOS
┌────────┬────────┬────────┬────────┬────────┬────────┐
│ FOR    │ DES    │ VIG    │ INT    │ SAB    │ CAR    │
│ [   ]  │ [   ]  │ [   ]  │ [   ]  │ [   ]  │ [   ]  │
└────────┴────────┴────────┴────────┴────────┴────────┘

RECURSOS
Vida Atual [      ] / Máxima [      ]
Vida Máxima em estudo: Patamar × (5 + VIG)
Mana Atual [      ] / Máxima [      ]

DEFESAS / RESISTÊNCIAS
                    REDUZIDO     COMPLETO
Defesa              [      ]     [      ]
Reflexos             [      ]     [      ]
Fortitude            [      ]     [      ]
Vontade              [      ]     [      ]

Leitura em estudo:
resultado < Reduzido       → sem dano/efeito
resultado ≥ Reduzido       → metade/reduzido
resultado ≥ Completo       → dano/efeito completo

Defesa física em estudo:
Reduzido = 8 + DES
Completo = 12 + DES

PERÍCIAS
                               BÔNUS    PASSIVO
FOR  Esportes                  [   ]    [   ]
DES  Furtividade               [   ]    [   ]
DES  Crime                     [   ]    [   ]
VIG  Resistência               [   ]    [   ]
INT  Ciência                   [   ]    [   ]
INT  Investigação              [   ]    [   ]
INT  Ocultismo                 [   ]    [   ]
SAB  Percepção                 [   ]    [   ]
SAB  Medicina                  [   ]    [   ]
SAB  Sobrevivência             [   ]    [   ]
CAR  Influência                [   ]    [   ]
CAR  Manipulação               [   ]    [   ]
CAR  Expressão                 [   ]    [   ]

Teste de Perícia: 1d20 + Bônus
Passivo: 8 + Bônus
Se CD ≤ Passivo, não há teste.

PONTOS DE PERÍCIA
Total em estudo:
(INT × 4) + (SAB × 2) + (CAR × 2) + FOR + DES + VIG + (Patamar × 2)

Somente valores permanentes dos Atributos entram nesse cálculo.

PODERES
┌─────────────────────────────────────────────────────────────────────┐
│ NOME DO PODER                                                       │
│ Atributo: ____   Custo: ____   Alcance: ____   Alvo/Área: ______ │
│ Acerto/Efeito: _________________________________________________ │
│ Dano/Cura/Proteção: ____________________________________________ │
│ Defesa/Resistência alvo: _______________________________________ │
│ Efeito especial / observações: _________________________________ │
└─────────────────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────────────────┐
│ NOME DO PODER                                                       │
│ Atributo: ____   Custo: ____   Alcance: ____   Alvo/Área: ______ │
│ Acerto/Efeito: _________________________________________________ │
│ Dano/Cura/Proteção: ____________________________________________ │
│ Defesa/Resistência alvo: _______________________________________ │
│ Efeito especial / observações: _________________________________ │
└─────────────────────────────────────────────────────────────────────┘

CONDIÇÕES / ANOTAÇÕES
___________________________________________________________________
___________________________________________________________________
___________________________________________________________________
```

## Princípio da ficha

A ficha deve mostrar diretamente os números usados em sessão.

```text
Atributos
→ bases de construção
→ não são rolados diretamente

Perícias
→ bônus final já calculado
→ passivo já calculado

Defesas
→ limiares já calculados

Poderes
→ fórmula e Atributo definidos na própria habilidade
```

A intenção é que o jogador não precise consultar fórmulas durante uma ação comum.

## Questões ainda abertas

- fórmula final de Vida;
- existência e fórmula de Mana;
- fórmulas de Reflexos, Fortitude e Vontade;
- quantidade de Poderes que deve caber na primeira página;
- necessidade de uma segunda página para equipamento, histórico e poderes adicionais;
- como mostrar alterações temporárias sem modificar os valores permanentes usados na criação de Perícias.

> Este documento é apenas um wireframe para teste e não altera regras aprovadas.
