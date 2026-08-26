# Calibração Independente

Status: APROVADO

Este arquivo define **como converter um conceito de personagem para a linguagem mecânica do sistema**.

Ele pertence a `criacao/` porque descreve um procedimento de construção e revisão. As definições de Patamar, Atributos, Perícias, Poderes e Traços permanecem em `../personagem/`.

## Princípio obrigatório

> **Cada personagem é calibrado pelo que ele próprio é, nunca pela ficha de outro personagem, salvo quando o JOGADOR HUMANO escolher explicitamente usar outra ficha como referência de equilíbrio.**

Como padrão:

- não usar protagonista, aliado ou rival como régua automática;
- não aumentar ou reduzir Atributos para equilibrar grupo;
- não escolher ou retirar Perícias para produzir contraste artificial;
- não inflar ou reduzir Patamar, Poderes, Traços ou recursos para aproximar fichas;
- aceitar assimetria quando ela representar corretamente os conceitos.

## Equilíbrio deliberado

Equilíbrio é permitido quando for uma escolha explícita do JOGADOR HUMANO.

Exemplos:

```text
equilibrar uma personagem com outra
usar outra ficha como referência mecânica
aproximar duas peças em capacidade geral
criar simetria deliberada
```

Nesse caso, a comparação pode orientar Patamar, Atributos, Perícias, Traços, Poderes e recursos na medida necessária para cumprir essa direção.

Isso não exige fichas idênticas nem resultados iguais em todas as disputas.

> **O sistema não balanceia por conta própria. O jogador pode pedir balanceamento deliberado.**

## Ordem de calibração

Sem pedido explícito de equilíbrio:

```text
1. definir Conceito e versão da personagem
2. listar capacidades e limites em linguagem natural
3. identificar treinamento, conhecimento, recursos e arsenal
4. definir Patamar coerente
5. distribuir Atributos
6. escolher Perícias realmente pertencentes à personagem
7. registrar Poderes e Traços coerentes
8. calcular Vida/Mana derivadas
9. comparar com outras fichas apenas para continuidade factual, se necessário
```

Fontes:

```text
Patamar    → ../personagem/patamar.md
Atributos  → ../personagem/atributos.md
Perícias   → ../personagem/pericias.md
Poderes    → ../personagem/poderes.md
Traços     → ../personagem/tracos.md
Vida       → ../resolucao/vida.md
Mana       → ../resolucao/mana.md
```

## Atributos

Atributos usam a escala permanente normal `[-2] a [7]`.

Escolher valores pelo que a personagem realmente consegue produzir, controlar, suportar, compreender, influenciar ou sustentar.

Não distribuir valor alto por protagonismo ou Importância.

## Perícias

Perícias não possuem graduação.

A pergunta é:

> **Em quais campos esta personagem realmente possui treinamento, prática ou experiência relevante?**

Não adicionar Perícia apenas para completar tema nem retirar para enfraquecer artificialmente a ficha.

## Patamar

Patamar `[1–7]` representa desenvolvimento mecânico geral.

Ele não mede:

- fama;
- importância narrativa;
- dificuldade do mundo;
- garantia de vitória.

> **Patamar descreve desenvolvimento. Dificuldade descreve a situação.**

## Poderes

Poder não possui grau genérico `[1–5]`.

A calibração pergunta:

- essa capacidade realmente pertence ao arsenal?
- qual função especial ela produz?
- qual Hub representa essa função?
- quais limites narrativos pertencem a esta versão?

A mecânica concreta pertence a `../resolucao/poderes/`.

## Traços e recursos

Traços registram verdades passivas estáveis. Recursos registram meios externos consolidados.

Não criar Traço ou Recurso apenas para compensar outra personagem.

## Calibração conservadora

“Conservadora” significa **não inventar capacidade maior do que o conceito sustenta**.

```text
há base clara
→ registrar a capacidade coerente

há dúvida real
→ usar a interpretação mais simples ainda fiel ao conceito

não há base
→ não inventar para preencher ficha ou confronto
```

Isso não significa escolher sempre o menor valor possível.

## Vitória não é régua de ficha

Não calibrar pela pergunta:

> **Quem precisa vencer quem?**

Confrontos dependem de especialização, conhecimento, preparação, recursos, vulnerabilidades, ambiente e abordagem concreta.

Ser capaz de vencer alguém em certas condições não justifica inflar todos os Atributos ou o arsenal.

## Personagens canônicos ou licenciados

Quando houver base externa:

1. identificar a versão escolhida;
2. registrar capacidades, limites, natureza, recursos, treinamento e conhecimento relevantes;
3. converter isso para a linguagem do sistema;
4. persistir a versão local aprovada, não uma lista de comparações com a obra-base.

O critério do que merece permanecer na ficha pertence a `../persistencia/relevancia-da-ficha.md`.

## Ordem de revisão

A calibração pode ser usada dentro dos blocos de `personagem.md` sempre que for preciso transformar conceito em valores ou capacidades.

Ela não substitui o procedimento de aprovação da criação.

## Regra final

> **Calibrar é converter fielmente uma personagem para as estruturas atuais do sistema. É construção, não balanceamento automático e não garantia de resultado.**
