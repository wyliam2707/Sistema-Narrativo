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

Quando houver incerteza real, Poderes usam o motor universal de `../motor-de-disputa.md` e, durante combate, as Defesas fixas de `../combate-e-dano.md`.

A rolagem ativa termina sempre com:

> **4 dados mantidos + Atributo pertinente**

O Atributo é determinado pela **forma real da ação**.

> **Nunca escolher automaticamente o maior Atributo.**

Se um arquivo individual definir explicitamente um Atributo para uma função específica daquele Poder, essa regra vale naquele recorte.

Perícia relevante pode conceder `+1d` quando seu campo realmente contribuir, mas não existe Perícia genérica de combate.

Durante combate, a peça que recebe a ação não faz uma rolagem defensiva comum. Usar:

```text
DF = 14 + Controle
RF = 14 + Resistência
DM = 14 + Intelecto
RM = 14 + Vontade
```

Em regra:

```text
ataque físico → DF
resistência física → RF
ataque mental → DM
resistência mental → RM
```

A natureza real do Poder pode determinar outro enquadramento, e uma regra específica pode substituir ou ignorar esses valores.

---

## 3. Sequência ofensiva

A sequência geral dos Poderes ofensivos é:

> **Defesa → Dano → Resistência → Efeito**

Nem todo Poder utiliza todas as etapas.

Na etapa de Defesa, a rolagem ativa é comparada à Defesa fixa apropriada. Resultado igual ou maior vence a etapa.

### Defesa [Absoluta]

Se o resultado ativo ficar abaixo da Defesa:

- não há Dano;
- o Efeito é anulado antes da Resistência.

### Defesa [Total]

Se o resultado ativo ficar abaixo da Defesa:

- não há Dano;
- o Efeito ainda pode seguir para Resistência.

### Defesa [Parcial]

Se o resultado ativo ficar abaixo da Defesa:

- o alvo sofre metade do Dano, arredondando para baixo;
- o Efeito ainda pode seguir para Resistência.

### Defesa [Nula]

Não existe etapa de Defesa.

Na etapa de Resistência, usar RF ou RM conforme a natureza do Efeito, salvo regra específica.

### Efeito [Total]

Resistência suficiente anula o Efeito.

### Efeito [Parcial]

Resistência suficiente reduz o Efeito em uma posição da progressão. Se o primeiro estágio for reduzido, nenhum Efeito é aplicado.

### Efeito [Nula]

Não existe etapa de Resistência.

A ordem de RD, Escudo, Trama e Vida pertence a `../combate-e-dano.md`.

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

### Apresentação do Hub ao jogador

O arquivo do Poder pode conter explicações, exemplos e regras detalhadas, mas a versão mostrada ao JOGADOR HUMANO deve ser **compacta e limpa**.

Na apresentação ao jogador:

- não inserir linhas em branco dentro do Hub;
- mostrar uma linha por campo relevante;
- não repetir explicações que já pertencem ao arquivo do Poder;
- não mostrar cálculos internos, justificativas ou texto de apoio salvo quando forem necessários para uma decisão real;
- manter somente as opções que o jogador pode consultar ou configurar naquele uso.

Formato preferido:

```text
Golpe [X]
Alcance: Toque → Próximo (~3 m)
Alvos: 1 → 2 → 4
Área: Alvo → Próximo (~3 m)
Dano: 1d8 → 2d8 → 3d8 → 4d8 [+Potência]
Efeito: Nenhum
Defesa: Total → Parcial
Efeito [Nula]
```

> **Arquivo detalha. Hub apresentado resume.**

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
- comparar o mesmo resultado às Defesas fixas individuais;
- se houver rolagem de Dano, rolar o Dano **uma vez** e aplicar o mesmo resultado aos atingidos;
- cada alvo aplica individualmente Defesa, RD, Escudo e outras proteções;
- Resistências de Efeito usam os valores fixos individuais quando os resultados puderem divergir.

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

## 8. Tempo, Conjuração e Turno

A terminologia temporal mecânica pode usar:

> **Instante → Turno → Cena → Hora → Dia**

No combate:

> **Turno = intervalo pessoal da peça, da sua vez atual até o início de sua próxima vez.**

Quando um Hub possuir **Conjuração**, salvo regra específica diferente:

```text
Conjuração: Cena
→ exige preparação ao longo da Cena antes de produzir o efeito

Conjuração: Turno
→ exige preparação durante o Turno pessoal completo da peça
→ conclui quando sua próxima vez começa, se a preparação continuar válida e não tiver sido interrompida

Conjuração: Instante
→ produz o efeito no instante causal em que for resolvido dentro da vez ou da cena
```

Conjuração mede tempo de preparação. Ela não cria uma fila própria.

Poderes não criam por si mesmos:

- iniciativa própria;
- fila de atuação paralela;
- ação bônus ou economia abstrata equivalente.

Iniciativa, Rodada, Turno pessoal, vez, interferência e precedência pertencem a `../../operacao/turnos-de-combate.md`.

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

> **A ficção determina se o Poder pode ser usado e qual Atributo participa. O Hub define sua configuração e custo. Durante combate, quem age faz a rolagem necessária e compara o resultado a DF, RF, DM ou RM conforme a natureza da etapa. A resolução usa apenas as etapas necessárias e nunca cria Iniciativa ou economia de ações paralela à operação do sistema.**