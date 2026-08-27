# Modelo de Ficha — Rascunho

Status: RASCUNHO / NÃO IMPLEMENTADO

Objetivo: usar este arquivo como modelo de dados para preencher personagens depois. Os campos aparecem apenas com `[X]`, sem linhas, caixas ou espaços de formulário.

## Estrutura proposta

### Bloco 1

Nome [X]
Controle [X]
Importância [X]
Patamar [X]

### Atributos

FOR [X]
DES [X]
VIG [X]
INT [X]
SAB [X]
CAR [X]

### Recursos

Vida Atual [X]
Vida Máxima [X]
Mana Atual [X]
Mana Máxima [X]

### Defesas / Resistências

Defesa — Reduzido [X] / Completo [X]
Reflexos — Reduzido [X] / Completo [X]
Fortitude — Reduzido [X] / Completo [X]
Vontade — Reduzido [X] / Completo [X]

### Perícias

FOR — Esportes: Bônus [X] / Passivo [X]

DES — Furtividade: Bônus [X] / Passivo [X]
DES — Crime: Bônus [X] / Passivo [X]

VIG — Resistência: Bônus [X] / Passivo [X]

INT — Ciência: Bônus [X] / Passivo [X]
INT — Investigação: Bônus [X] / Passivo [X]
INT — Ocultismo: Bônus [X] / Passivo [X]

SAB — Percepção: Bônus [X] / Passivo [X]
SAB — Medicina: Bônus [X] / Passivo [X]
SAB — Sobrevivência: Bônus [X] / Passivo [X]

CAR — Influência: Bônus [X] / Passivo [X]
CAR — Manipulação: Bônus [X] / Passivo [X]
CAR — Expressão: Bônus [X] / Passivo [X]

### Pontos de Perícia

Total [X]

### Poderes

Nome [X]
Atributo [X]
Custo [X]
Alcance [X]
Alvo/Área [X]
Acerto/Efeito [X]
Dano/Cura/Proteção [X]
Defesa/Resistência alvo [X]
Efeito especial / observações [X]

### Condições / Anotações

[X]

## Regras em estudo relacionadas ao modelo

Teste de Perícia: `1d20 + Bônus`

Passivo: `8 + Bônus`

Se `CD ≤ Passivo`, não há teste.

Vida Máxima em estudo: `Patamar × (5 + VIG)`

Defesa física em estudo:
- Reduzido = `8 + DES`
- Completo = `12 + DES`

Leitura das Defesas em estudo:
- resultado abaixo de Reduzido → sem dano/efeito;
- resultado entre Reduzido e Completo → metade/reduzido;
- resultado igual ou acima de Completo → dano/efeito completo.

Pontos de Perícia em estudo:

`(INT × 4) + (SAB × 2) + (CAR × 2) + FOR + DES + VIG + (Patamar × 2)`

Somente valores permanentes dos Atributos entram no cálculo de Pontos de Perícia.

## Princípio da ficha

Os Atributos são bases de construção e não são rolados diretamente.

Perícias, Defesas, Recursos e Poderes devem aparecer com seus valores já calculados para uso em sessão.

> Este documento é apenas um modelo em teste e não altera regras aprovadas.
