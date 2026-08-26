# Poderes

Status: APROVADO

Esta pasta reúne as regras mecânicas concretas dos **Poderes**.

A definição de quais Poderes pertencem a uma personagem e como aparecem na ficha pertence a `../../personagem/poderes.md`.

> **Poder representa parte do arsenal funcional da personagem. O arquivo individual define a mecânica; o Hub configura o uso.**

Um Poder pode ter origem física, técnica, tecnológica, sobrenatural, psíquica, biológica ou qualquer outra coerente com o Conceito.

---

## 1. Ações comuns não exigem Poder

Poder só é necessário quando a personagem pretende produzir uma capacidade que não esteja disponível como ação comum em sua situação.

```text
soco, corrida, empurrão comum
→ ação comum

teleporte, raio, domínio mental, invocação
→ exige capacidade correspondente
```

Quando um ataque comum causa Dano sem Poder ofensivo, consultar `../combate-e-dano.md`.

---

## 2. Resolução universal

Quando houver incerteza real, Poderes usam o motor universal de `../motor-de-disputa.md`.

A rolagem termina sempre com:

> **4 dados mantidos + Atributo pertinente**

O Atributo é determinado pela **forma real da ação, reação ou resistência**.

> **Nunca escolher automaticamente o maior Atributo.**

Se um arquivo individual definir explicitamente um Atributo para uma função específica daquele Poder, essa regra vale naquele recorte.

Perícia relevante pode conceder `+1d` quando seu campo realmente contribuir, mas não existe Perícia genérica de combate.

---

## 3. Sequência ofensiva

A sequência geral dos Poderes ofensivos é:

> **Defesa → Dano → Resistência → Efeito**

Nem todo Poder utiliza todas as etapas.

### Defesa [Absoluta]

Se a Defesa vencer:

- não há Dano;
- o Efeito é anulado antes da Resistência.

### Defesa [Total]

Se a Defesa vencer:

- não há Dano;
- o Efeito ainda pode seguir para Resistência.

### Defesa [Parcial]

Se a Defesa vencer:

- o alvo sofre metade do Dano, arredondando para baixo;
- o Efeito ainda pode seguir para Resistência.

### Defesa [Nula]

Não existe etapa de Defesa.

### Efeito [Total]

Resistência bem-sucedida anula o Efeito.

### Efeito [Parcial]

Resistência bem-sucedida reduz o Efeito em uma posição da progressão. Se o primeiro estágio for reduzido, nenhum Efeito é aplicado.

### Efeito [Nula]

Não existe etapa de Resistência.

A ordem de RD, Barreira, Trama e Vida pertence a `../combate-e-dano.md`.

---

## 4. Hub e custo

Cada Poder apresenta somente os campos necessários à sua função.

Campos possíveis incluem:

- Alcance;
- Alvos;
- Área;
- Dano;
- Efeito;
- Defesa;
- Duração;
- Conjuração;
- Referência;
- Tipo;
- Modo;
- Distância;
- Escopo;
- Contra;
- Tamanho;
- Material;
- outras progressões específicas.

Salvo regra diferente no próprio arquivo:

```text
primeira posição de uma progressão
→ +0 Mana

cada avanço seguinte
→ +1 Mana
```

O custo final é a soma das escolhas usadas naquela configuração.

> **Custo total ≤ [X]**

`[X]` é o Patamar da personagem e representa o máximo de Mana que pode ser gasto em um único uso. A regra completa está em `../mana.md`.

---

## 5. Configuração e confirmação

A operação geral continua obedecendo `../../operacao/ordem-de-resolucao-do-combate.md`:

> **perguntar somente o que ainda pode mudar a resolução.**

Por isso, frases em arquivos individuais como `Confirmar uso por X Mana?` devem ser interpretadas assim:

```text
configuração ou custo ainda depende de escolha do JOGADOR HUMANO
→ apresentar a configuração e perguntar apenas pela escolha faltante

configuração, alvo e custo já foram declarados de forma inequívoca
→ não criar confirmação burocrática adicional
```

Esta regra operacional prevalece sobre formulações genéricas repetidas nos arquivos individuais. Uma regra especial do próprio Poder continua prevalecendo quando realmente fizer parte de sua mecânica.

---

## 6. Alvos e Área

Quando um Poder oferece **Alvos** e **Área** como alternativas:

- **Alvos:** escolhe entidades individualmente;
- **Área:** afeta todos dentro da região definida;
- somente a opção usada entra no custo.

O próprio arquivo pode definir outra função para Área quando necessário.

### Múltiplos alvos

Usar o menor número possível de rolagens.

Quando um único uso atinge várias entidades:

- se houver Acerto, fazer **uma rolagem de Acerto**;
- cada alvo resolve sua própria Defesa contra o mesmo resultado;
- se houver rolagem de Dano, rolar o Dano **uma vez** e aplicar o mesmo resultado aos atingidos;
- cada alvo aplica individualmente Defesa, RD, Barreira e outras proteções;
- Resistências de Efeito continuam individuais quando os resultados puderem divergir.

---

## 7. Distâncias

As distâncias são categorias narrativas:

```text
Si Mesmo
Toque
Próximo  ≈ 3 m
Curto    ≈ 20 m
Médio    ≈ 45 m
Longo    ≈ 90 m
```

Os metros são referências, não uma régua geométrica rígida.

Acima de Longo, a própria capacidade precisa justificar a distância, como Teleporte ou outra regra específica.

---

## 8. Tempo, Conjuração e turnos

A terminologia temporal mecânica pode usar:

> **Instante → Turno → Cena → Hora → Dia**

No combate:

> **Turno = intervalo simultâneo de até 10 segundos compartilhado por todas as peças.**

Quando um Hub possuir **Conjuração**, salvo regra específica diferente:

```text
Conjuração: Cena
→ exige preparação ao longo da Cena antes de produzir o efeito

Conjuração: Turno
→ exige preparação durante um intervalo simultâneo completo de até 10 segundos
→ conclui no fechamento daquele Turno se a preparação continuar válida e não tiver sido interrompida

Conjuração: Instante
→ produz o efeito no instante causal em que for resolvido dentro do Turno ou da cena
```

Conjuração mede tempo de preparação. Ela não cria uma fila própria.

Poderes não criam por si mesmos:

- iniciativa fixa;
- fila de atuação;
- uma ação universal por turno;
- ação bônus ou economia abstrata equivalente.

Interferência, interrupção e precedência pertencem a `../../operacao/turnos-de-combate.md`.

---

## 9. Status

Poderes que produzem efeitos nocivos utilizam as definições de `../status/`.

Famílias diferentes podem coexistir. Sobreposição dentro da mesma família segue a regra de Status, não cria empilhamento livre de penalidades.

---

## 10. Índice

- `adaptacao.md`
- `aflicao.md`
- `aprimoramento.md`
- `comunicacao.md`
- `contencao.md`
- `criacao.md`
- `cura.md`
- `debilitacao.md`
- `deteccao.md`
- `disparo.md`
- `dissipacao.md`
- `escudo.md`
- `exaustao.md`
- `golpe.md`
- `ilusao.md`
- `influencia.md`
- `invocacao.md`
- `metamorfose.md`
- `movimento.md`
- `perturbacao.md`
- `posicao.md`
- `protecao.md`
- `raio.md`
- `ruina.md`
- `sentidos.md`
- `telecinese.md`
- `teleporte.md`
- `terror.md`

## Regra final

> **A ficção determina se o Poder pode ser usado e qual Atributo participa. O Hub define sua configuração e custo. A resolução usa apenas as etapas necessárias e nunca cria iniciativa ou economia de ações paralela à operação do sistema.**
