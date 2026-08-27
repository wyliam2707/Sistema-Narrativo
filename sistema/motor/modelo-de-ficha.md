# Modelo de Ficha — Rascunho

Status: RASCUNHO / NÃO IMPLEMENTADO

Objetivo: usar este arquivo como modelo de dados para preencher personagens depois. Os campos aparecem apenas com `[X]`, sem linhas, caixas ou espaços de formulário.

## Estrutura proposta

### Bloco 1

Nome [X]
Controle [X]
Importância [X]
Patamar [X]

### Bloco 2

FOR [X] | DES [X] | VIG [X] | INT [X] | SAB [X] | CAR [X]

### Bloco 3

Esportes [X] + FOR = [+X] | Furtividade [X] + DES = [+X] | Crime [X] + DES = [+X]
Resistência [X] + VIG = [+X] | Ciência [X] + INT = [+X] | Investigação [X] + INT = [+X]
Ocultismo [X] + INT = [+X] | Percepção [X] + SAB = [+X] | Medicina [X] + SAB = [+X]
Sobrevivência [X] + SAB = [+X] | Manipulação [X] + CAR = [+X] | Expressão [X] + CAR = [+X]

### Bloco 4

Traços Positivos [X]
Traços Negativos [X]

### Bloco 5 — Estatísticas

Pontos de Vida [X] | Pontos de Mana [X] | Defesa [X/Y]
Reflexos [X/Y] | Fortitude [X/Y] | Vontade [X/Y]

Defesa:
- X = 8 + ATR
- Y = 12 + ATR

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

Leitura da Defesa em estudo:
- resultado abaixo de X → sem dano/efeito;
- resultado entre X e Y → metade/reduzido;
- resultado igual ou acima de Y → dano/efeito completo.

Pontos de Perícia em estudo:

`(INT × 4) + (SAB × 2) + (CAR × 2) + FOR + DES + VIG + (Patamar × 2)`

Somente valores permanentes dos Atributos entram no cálculo de Pontos de Perícia.

## Princípio da ficha

Os Atributos são bases de construção e não são rolados diretamente.

Perícias, Defesas, Recursos e Poderes devem aparecer com seus valores já calculados para uso em sessão.

> Este documento é apenas um modelo em teste e não altera regras aprovadas.
