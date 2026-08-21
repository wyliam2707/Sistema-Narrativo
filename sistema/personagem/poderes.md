# Poderes

Status: EM REVISÃO

Poderes representam capacidades especiais, sobrenaturais, tecnológicas ou ativas que precisam ser registradas separadamente dos atributos.

## Sintaxe padrão

```text
Poder [Fonte opcional] [grau] => usos / especializações
```

Exemplos:

```text
Magia [3] => Cura / Invocação / Proteção / Portal / Demonologia [5] / Contenção [1]
Metamorfose [Animais] [4] => Geral
Telecinético [2] => Voar / Portal / Telecinese
```

## Repertório após `=>`

O que vem depois de `=>` define o repertório disponível.

Exemplo:

```text
Magia [3] => Cura / Invocação / Proteção / Portal / Demonologia [5] / Contenção [1]
```

significa:

- Cura = 3;
- Invocação = 3;
- Proteção = 3;
- Portal = 3;
- Demonologia = 5;
- Contenção = 1.

Se `Disparo` não aparece, ele não existe por padrão.

Se `Ampliação` não aparece, ele não existe por padrão.

## Valor-base

O valor do poder é usado pelas utilizações sem valor próprio.

```text
Magia [3] => Cura / Portal / Proteção
```

Cura, Portal e Proteção funcionam em 3.

Uma utilização com valor próprio substitui o valor-base naquele recorte:

```text
Magia [3] => Portal [1] / Invocação [5]
```

- Portal = 1;
- Invocação = 5.

Não existe soma `3 + 1` ou `3 + 5`.

## Geral

`Geral` autoriza usos não listados especificamente, desde que sejam coerentes com o domínio do poder.

```text
Magia [1] => Geral / Portal [5]
```

Nesse caso, usos mágicos genéricos funcionam em grau 1 e Portal em grau 5.

Sem `Geral`, o repertório permanece restrito aos usos listados.

## Fonte no cabeçalho

Uma fonte entre colchetes no cabeçalho limita todo o poder.

```text
Magia [Fogo] [3] => Disparo
```

Esse poder pode produzir um Disparo de fogo, não gelo, raio ou energia arcana genérica.

Outro exemplo:

```text
Metamorfose [Animais] [3] => Geral
```

`Geral` amplia os usos possíveis, mas sempre dentro da fronteira `Animais`.

> **Fonte no cabeçalho = fronteira temática do poder.**

## Especialização dentro da lista

Uma fonte ou tema depois de `=>` funciona como especialização e não restringe o poder inteiro.

```text
Magia [2] => Disparo / Fogo [4]
```

Aqui:

- magia genérica = 2;
- disparo mágico genérico = 2;
- aplicações especificamente de fogo = 4.

Outro exemplo:

```text
Magia [2] => Geral / Invocação / Demonologia [5]
```

- magia genérica = 2;
- invocação comum = 2;
- aplicações especificamente demonológicas = 5.

A especialização aplicável substitui o valor-base naquele tema. Ela não é somada a ele.

## Categorias específicas sem Geral

```text
Metamorfose [3] => Animais / Humanos / Plantas Grandes / Objetos Grandes / Animais Minúsculos
```

O personagem possui exatamente as categorias declaradas, todas no valor-base salvo exceções específicas.

Ele não recebe automaticamente categorias não listadas.

## Disparo

`Disparo` significa apenas:

> **projetar algo à distância.**

A natureza do que é disparado vem do poder-base.

Exemplos:

```text
Telecinese => Disparo
Magia => Disparo
Lançador de Teia => Disparo
```

A palavra `Disparo` não define sozinha elemento, aparência ou natureza do efeito.

## Ampliação

`Ampliação` é um uso ativo para reforçar algo existente.

Exemplos:

- encantar uma arma;
- aumentar temporariamente a própria força;
- reforçar uma armadura;
- intensificar outro efeito.

Se o aumento é natural e permanente, ele deve aparecer no atributo ou na capacidade permanente apropriada, e não em Ampliação apenas para duplicar a mesma informação.

## Capacidades diferentes não se fundem numa soma automática

Cada capacidade continua representando uma parte distinta do que o personagem consegue fazer.

Exemplo:

```text
Ampliação [5]
Telecinese [1]
```

pode representar enorme potência de reforço combinada com controle telecinético limitado.

Um valor alto em uma capacidade não apaga automaticamente a limitação de outra.

A regra de como múltiplas capacidades participam de uma ação pertence a `../resolucao/`.

## Poder e atributo

Uma capacidade natural e permanente deve ser registrada diretamente no atributo quando isso representar adequadamente o personagem.

Uma capacidade ativa, temática ou com repertório próprio deve ser registrada como poder.

A separação detalhada está em `atributos.md`.
