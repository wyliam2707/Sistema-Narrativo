# Poderes

Status: APROVADO

Poderes representam **arsenais de capacidades relacionadas** por uma mesma fonte, natureza, tecnologia, tradição, equipamento ou conceito.

Um Poder não precisa ser sobrenatural.

Ele pode representar magia, mutação, tecnologia, armadura, veículos, equipamentos especiais, capacidades psíquicas ou qualquer outro conjunto coerente de possibilidades que precise ser registrado separadamente dos atributos e perícias.

> **O Poder define um arsenal. O repertório define o que esse arsenal consegue fazer.**

---

## 1. Sintaxe padrão

```text
Poder [Fonte opcional] [grau] => usos / especializações
```

Exemplos:

```text
Magia Branca [1] => Geral / Dano [2] / Cura [4]
Metamorfose [Animais] [3] => Geral
Armadura [1] => Geral / Balística [2]
Veículos [1] => Moto / Carro / Avião
```

Todo Poder possui obrigatoriamente um patamar-base.

Poder `[0]` não existe.

Se o personagem não possui determinada capacidade ou arsenal, ele simplesmente não aparece na ficha.

---

## 2. Patamar do Poder

Poderes usam a mesma lógica qualitativa e não linear de PATAMAR definida em `escala.md`.

O grau indica em que escala aquele arsenal ou capacidade funciona.

```text
[1] [2] [3] [4] [5]
```

Graus altos devem ser usados com parcimônia.

`[3]` já representa uma capacidade realmente poderosa.

`[4]` representa um patamar extremo, reservado para poucos casos.

`[5]` representa o ápice daquela capacidade e deve ser quase único dentro da categoria.

> **Se o personagem não é o equivalente ao “Superman” daquela capacidade, provavelmente não precisa de [5].**

Essa restrição é de calibração conceitual, não de balanceamento.

Um personagem pode possuir apenas Poderes `[1]` e isso ser a representação correta dele.

Nenhum Poder deve ser elevado apenas para aproximar sua ficha da de outro personagem, tornar um confronto justo ou equilibrar um grupo.

---

## 3. Repertório após `=>`

O que vem depois de `=>` define o repertório disponível dentro daquele Poder.

Exemplo:

```text
Magia Branca [1] => Geral / Dano [2] / Cura [4]
```

significa:

- usos gerais coerentes de Magia Branca = `[1]`;
- Dano = `[2]`;
- Cura = `[4]`.

O nome dos usos é aberto e descritivo.

Podem existir, por exemplo:

```text
Dano
Cura
Movimento
Proteção
Ocultação
Contenção
Congelamento
Invocação
Portal
Análise
Maldição
```

Não existe uma lista universal obrigatória.

O uso deve descrever **o efeito ou função relevante**, não obrigatoriamente a forma visual pela qual ele acontece.

Por isso, `Dano` pode assumir a forma de raio, projétil, explosão, toque, onda ou outra manifestação coerente com o Poder.

> **A forma narrativa não cria automaticamente uma nova capacidade mecânica.**

---

## 4. Valor-base e específico

O patamar-base do Poder é usado pelos usos que não possuem valor próprio.

```text
Magia [2] => Cura / Portal / Proteção
```

Cura, Portal e Proteção funcionam em `[2]`.

Um uso com patamar próprio substitui o valor-base naquele recorte.

```text
Magia [3] => Geral / Cura [1] / Portal [4]
```

significa:

- usos gerais de Magia = `[3]`;
- Cura = `[1]`;
- Portal = `[4]`.

O específico prevalece sobre o geral mesmo quando possui patamar menor.

> **O geral estabelece o padrão. O específico define a exceção.**

Não existe soma entre o valor-base e o valor específico.

```text
Magia [3] + Portal [4] ≠ [7]
```

Portal simplesmente funciona em `[4]`.

---

## 5. Geral

`Geral` autoriza usos não listados especificamente, desde que sejam coerentes com o domínio do Poder.

```text
Magia [2] => Geral / Portal [4]
```

Usos mágicos coerentes e não listados funcionam em `[2]`.

Portal funciona em `[4]`.

Sem `Geral`, o repertório permanece restrito aos usos declarados.

```text
Veículos [1] => Moto / Carro / Avião
```

Nesse caso, o Poder garante apenas as categorias declaradas.

---

## 6. Fonte no cabeçalho

Uma fonte entre colchetes no cabeçalho funciona como fronteira temática de um único Poder.

```text
Metamorfose [Animais] [3] => Geral
```

`Geral` autoriza usos amplos de Metamorfose, mas sempre dentro da fronteira `Animais`.

> **Fonte no cabeçalho = limite temático daquele arsenal.**

A fonte no cabeçalho deve ser usada quando realmente delimita uma única capacidade.

Quando uma fonte possui identidade, repertório ou patamar próprios, ela deve ser registrada como Poder separado.

Exemplo:

```text
Magia [3] => Geral / Dano / Proteção
Magia Negra [5] => Geral / Dano / Maldição / Invocação
Magia Branca [1] => Geral / Dano [2] / Cura [4]
```

Esses são três arsenais distintos.

Um não herda automaticamente o repertório ou o patamar dos outros.

---

## 7. Poderes diferentes não se somam

Dois Poderes diferentes podem produzir efeitos semelhantes sem se fundirem numa soma automática.

```text
Magia [2] => Dano
Magia Negra [4] => Dano
```

Se o personagem usa Magia, o Dano opera em `[2]`.

Se usa Magia Negra, o Dano opera em `[4]`.

A resolução considera qual arsenal foi realmente empregado na ficção.

O sistema não escolhe automaticamente o maior valor sem considerar a ação declarada.

---

## 8. Efeito não é forma de entrega

Não existe um uso universal chamado `Disparo` necessário para permitir ataques à distância.

A forma de entrega e o efeito são informações diferentes.

Exemplo:

```text
Gelo [2] => Dano / Congelamento
```

O personagem pode manifestar Dano ou Congelamento de maneiras coerentes com seu Poder — raio, toque, projétil, onda ou outra forma apropriada — sem que `Disparo` precise existir como categoria separada.

Da mesma forma:

```text
Telecinese [3] => Dano / Movimento / Contenção / Proteção
```

cada termo descreve uma função do arsenal, não uma aparência obrigatória.

---

## 9. Poder, atributo e perícia

Cada parte da ficha responde a uma pergunta diferente.

```text
ATRIBUTO → qual capacidade inerente o personagem possui?
PERÍCIA  → qual domínio adquirido ele possui?
PODER    → qual arsenal especial ele possui e em que patamar funciona?
```

Exemplo:

```text
Armadura [1] => Geral / Balística [2]
Veículos [1] => Moto / Carro / Avião
Piloto [+3]
```

`Veículos [1]` informa quais recursos extraordinários estão disponíveis e em qual patamar.

`Piloto [+3]` informa quão bem o personagem sabe conduzi-los.

Uma coisa não substitui automaticamente a outra.

Uma capacidade natural e permanente pode ser registrada diretamente no atributo quando o atributo representar adequadamente aquela capacidade.

Quando existe um arsenal temático, uma capacidade especial ou um repertório próprio, ele deve ser registrado como Poder.

---

## 10. Exemplo de arsenal tecnológico

Um personagem como Batman pode ser representado sem transformar seus equipamentos em dezenas de entradas independentes:

```text
Arsenal [1] => Dano / Cura / Ocultação / Movimento / Contenção
Armadura [1] => Geral / Balística [2]
Veículos [1] => Moto / Carro / Avião
```

O Poder registra o conjunto de recursos disponíveis.

A Perícia registra o domínio do personagem ao utilizá-los.

Isso permite fichas compactas sem perder diferenças relevantes entre recursos gerais e especializações.

---

## 11. Sem balanceamento por comparação

Poderes são calibrados pelo personagem que os possui.

Não usar protagonista, aliado, rival, antagonista ou outro membro do grupo como régua para aumentar ou reduzir patamares.

Não elevar um Poder porque outro personagem parece mais forte.

Não reduzir um Poder porque ele parece injusto para um confronto.

Não criar contramedidas retroativas apenas para restaurar dificuldade.

> **A ficha descreve o personagem. Ela não tenta torná-lo justo em relação aos demais.**

A regra completa de calibração independente pertence a `calibracao.md`.
