# Pontos de Perícia

Status: RASCUNHO / NÃO IMPLEMENTADO

## Ideia central

Os Atributos são usados como base para calcular o orçamento total de Pontos de Perícia durante a criação e evolução da personagem.

Uma fórmula em estudo é:

```text
Pontos de Perícia = (INT × 4) + (SAB × 2) + (CAR × 2) + FOR + DES + VIG + (Patamar × 2)
```

## Valores permanentes

Somente os **valores permanentes dos Atributos** entram nesse cálculo.

Bônus temporários ou circunstanciais não aumentam o total de Pontos de Perícia.

Exemplos que não contam para o cálculo:

- magia;
- equipamento;
- transformação temporária;
- bônus de condição;
- melhoria de curta duração;
- qualquer outro aumento que não altere permanentemente o Atributo da personagem.

Em termos conceituais:

```text
Atributo permanente
→ pode alimentar Pontos de Perícia

Atributo temporariamente aumentado
→ não altera Pontos de Perícia
```

## Motivo de design

Pontos de Perícia representam aprendizado, experiência, treinamento e repertório adquirido da personagem. Um aumento temporário de capacidade não concede automaticamente novas competências aprendidas.

Isso também evita que efeitos temporários alterem retroativamente a construção da ficha.

## Questões em aberto

- confirmar os multiplicadores finais de cada Atributo;
- verificar se INT × 4 cria peso excessivo em comparação aos demais Atributos;
- definir os valores máximos de treinamento em cada Perícia;
- definir como aumentos permanentes posteriores de Atributos afetam novos Pontos de Perícia;
- definir se Pontos de Perícia não gastos podem ser guardados.

> **Este documento registra apenas uma hipótese de motor. Não altera as regras aprovadas.**
