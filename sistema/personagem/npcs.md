# NPCs, Importância e Modelos Rápidos

Status: EM REVISÃO

A importância narrativa determina **quanto detalhe precisa ser acompanhado**, não quanto poder, resistência ou proteção de roteiro um personagem possui.

## Categorias de importância

### Central

Personagem nuclear da história.

Acompanhar com alta continuidade:

- personalidade;
- relações;
- capacidades;
- equipamentos recorrentes;
- mudanças estáveis;
- consequências relevantes.

STATUS temporário continua fora da ficha permanente.

### Relevante

Personagem recorrente ou importante para cenas e arcos.

Usar ficha curta ou completa conforme a necessidade real de continuidade.

### Figurante

Personagem de cena ou baixa importância.

Usar apenas a informação necessária para resolver e narrar sua participação.

> **Importância não altera poder, chance de sucesso, resistência nem realidade do mundo.**

Um Figurante pode ser muito mais poderoso que um personagem Central. A categoria apenas determina o nível de detalhe acompanhado.

## Modelo rápido — modelo e exceção

Para NPCs simples, especialmente Figurantes, usar:

```text
Função/Nome — Modelo [grau] | exceções
```

O nome do modelo representa natureza, espécie ou arquétipo.

O grau representa a escala-base dos atributos.

Exemplos válidos:

```text
Humano [0]
Humano [1]
Zumbi [0]
Vampiro [1]
Demônio [0]
Demônio [3]
```

O nome do modelo não determina automaticamente o grau.

## O que o modelo preenche

O valor do modelo preenche todos os atributos automaticamente.

Exemplo:

```text
Guarda — Humano [1]
```

significa:

```text
FOR [1]
AGI [1]
RES [1]
MEN [1]
VON [1]
```

Somente valores diferentes precisam ser escritos.

Exemplo:

```text
Invocação — Demônio [3] | FOR [4] | VON [1]
```

significa base 3 em todos os atributos, com FOR 4 e VON 1 como exceções.

## Características implícitas do modelo

Além dos atributos, um modelo pode carregar características básicas **já estabelecidas para aquela natureza no cenário, cânone ou aventura**.

Isso pode incluir:

- comportamentos típicos;
- necessidades;
- hábitos;
- capacidades comuns;
- limitações;
- fraquezas.

O modelo não cria propriedades universais para uma espécie.

Exemplo:

```text
Vampiro [1]
```

usa as propriedades vampíricas já definidas naquele cenário específico.

Se naquele mundo vampiros não queimam ao sol, o modelo não inventa essa fraqueza.

## Exceções

Somente o que foge do modelo precisa ser declarado.

```text
Vampiro [1] | FOR [2] | resistente à luz solar
```

significa que o personagem segue o modelo vampírico daquele mundo, exceto pelas alterações expressas.

Perícias e recursos importantes podem ser adicionados:

```text
Guarda — Humano [0] | Soldado [+2] | rifle / colete
```

## Figurantes não exigem arquivo persistente

Um Figurante ou inimigo comum normalmente pode existir apenas durante a cena.

Não é necessário criar um arquivo individual em `personagens/` ou `mestre/viloes/` apenas porque ele participou de uma resolução.

Se sobreviver, reaparecer, ganhar importância ou passar a exigir continuidade própria, ele pode receber uma ficha Relevante ou reservada posteriormente.

> **Poder por si só não exige ficha persistente. Continuidade e necessidade de detalhe é que exigem.**

## Antagonistas importantes

Um antagonista importante, recorrente ou poderoso pode receber ficha completa quando suas capacidades, objetivos, limites ou segredos precisarem existir de forma estável.

Se a ficha precisar permanecer oculta, armazená-la na área reservada da aventura.

Uma ficha oculta já estabelecida não pode ganhar poderes, imunidades ou recursos retroativos apenas para neutralizar uma solução válida do protagonista.

Mudanças posteriores precisam nascer de acontecimentos reais da ficção.

## Calibração

NPCs, antagonistas, aliados e protagonistas obedecem à mesma regra de `calibracao.md`:

> **cada personagem é construído pelo que ele é, nunca para equilibrar outra ficha.**
