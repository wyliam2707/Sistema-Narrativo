# Traços

Status: APROVADO

Traços registram **verdades passivas e estáveis** da personagem: propriedades, capacidades naturais, limitações, necessidades ou condições consolidadas.

> **Traço descreve algo que a personagem é, possui ou faz naturalmente. Poder descreve uma função ativa do arsenal.**

Os catálogos canônicos estão em `tracos/`.

## Traço é verdade da ficha

Um Traço:

- existe passivamente;
- garante apenas o que sua descrição afirma;
- não substitui Atributos ou Perícias;
- não concede bônus genérico de rolagem;
- pode tornar um resultado evidente quando sua própria redação já resolve a questão;
- pode limitar possibilidades quando sua condição se aplica.

Exemplos:

```text
Fisiologia Sobrenatural.
Não envelhece.
Corpo artificial.
Não pode mentir.
Vulnerável à luz solar.
```

## Grupos

```text
Comuns        → tracos/comuns.md
Sobrenaturais → tracos/sobrenaturais.md
Vícios        → tracos/vicios.md
Corrupções    → tracos/corrupcao.md
```

### Comuns

Vantagens ou características passivas compatíveis com pessoas comuns do cenário.

### Sobrenaturais

Propriedades passivas extraordinárias, como fisiologia incomum, imunidades, sentidos especiais ou recuperação.

### Vícios

Limitações negativas mundanas, hábitos, medos, conflitos, compromissos e problemas recorrentes.

### Corrupções

Fraquezas, necessidades, vulnerabilidades e restrições sobrenaturais.

## Custo dos Traços positivos

Todo Traço positivo custa:

> **1 espaço de Traço positivo**

Não existe preço de aquisição `[1]`, `[2]` ou `[3]` para Traços positivos.

Na criação:

```text
1 Traço positivo
→ ocupa 1 espaço de Traço

1 Poder
→ ocupa 1 espaço de Poder
```

Essa equivalência é de **custo de construção**, não de função. Traços e Poderes continuam fazendo coisas diferentes.

Um Traço pode possuir níveis, categorias ou estágios internos quando sua própria regra realmente precisar deles. Nesse caso, o número faz parte do **efeito do Traço**, não aumenta seu custo de aquisição.

> **Nível interno não é preço. Todo Traço positivo continua custando 1.**

## Relevância mínima

Como cada Traço positivo ocupa um espaço inteiro de construção, ele deve estabelecer uma vantagem passiva relevante.

Detalhes menores que apenas descrevem a personagem, sem alterar de forma significativa o que ela pode fazer, acessar, possuir ou estabelecer na ficção, pertencem normalmente ao Conceito ou à descrição.

Exemplos de detalhes que não precisam virar Traço pago por si só:

```text
ser ambidestro
ter bom senso de direção
ter aparência pouco chamativa
preferir determinada mão, roupa ou hábito
```

Criar um Traço pago quando a característica realmente estabelecer uma vantagem persistente própria.

## Valores negativos

```text
Vício      → [-1]
Corrupção  → [-1] ou [-2]
```

A economia de criação pertence a `patamar.md` e ao processo de `../criacao/`.

Cada ponto negativo pode comprar **uma** destas opções:

- `+1` Traço positivo;
- `+1` Poder.

O mesmo ponto não compra as duas coisas.

## Número não entra automaticamente na rolagem

Qualquer número que faça parte de um Traço:

```text
≠ bônus genérico
≠ +Xd automático
```

Só existe modificação mecânica quando a própria descrição do Traço disser explicitamente `+Xd`, `-Xd`, RD, Imunidade, recuperação ou outra consequência específica.

## Resultado evidente

Se o Traço já responde à questão, não se cria teste.

```text
Traço: Fisiologia Sobrenatural
Situação: ambiente sem ar
→ ausência de oxigênio por si só não causa sufocamento
```

Quando o Traço apenas torna uma ação possível e ainda existe incerteza real na execução, `../resolucao/` continua aplicável.

## Permanência e condição

Um Traço pode ser permanente e produzir consequência apenas quando determinada condição existe.

```text
Vulnerável à luz solar.
Enfraquece em água corrente.
Não pode entrar em cemitérios.
```

Ferimentos, Status e efeitos passageiros pertencem ao estado atual, não à lista de Traços permanentes.

## Aplicação literal

Um Traço produz apenas as consequências sustentadas por sua redação.

Não ampliar uma limitação por inferência apenas para impedir uma solução válida.

```text
não pode atravessar água corrente
→ um Teleporte pode contornar se realmente não houver travessia

não pode entrar em cemitérios
→ mudar o método de entrada não contorna a proibição
```

## Conhecimento

Uma verdade estar registrada na ficha não significa que todas as personagens saibam dela.

A separação entre informação disponível à persona e conhecimento da personagem pertence a `../personas/escopo-de-consulta.md`.

Este arquivo não autoriza conhecimento retroativo de vulnerabilidades ou limitações.

## Evitar duplicação

Não criar Traço para repetir algo já suficientemente representado:

```text
Potência alta → força natural
Medicina      → treinamento médico
Teleporte     → Poder ativo
```

Criar Traço quando existir uma verdade passiva própria que ainda precise ser registrada.

## Traços e Trama

A interação mecânica com Pontos de Trama pertence a `trama.md`.

Quando uma complicação de Traço for voluntariamente aceita pela peça elegível, a regra de Trama determina eventual ganho. A autoridade da decisão continua em `../personas/`.

## Regra final

> **Todo Traço positivo custa 1 espaço. Sua redação define sua consequência; qualquer nível interno pertence ao efeito, nunca ao preço. Traço continua sendo uma verdade passiva consolidada da personagem.**
