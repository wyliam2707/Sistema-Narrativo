# Mestre

Status: REFORMULAÇÃO / NÃO IMPLEMENTADO

Esta pasta reúne as regras de **condução e apresentação narrativa** usadas pelo `NARRADOR` depois que o Tribunal já estabeleceu o que realmente aconteceu.

`mestre/` não cria uma nova persona.

A autoridade continua pertencendo ao `NARRADOR` definido em `../nucleo/1.1-narrador.md`.

```text
NÚCLEO
→ quem declara
→ quem julga
→ o que realmente acontece
→ quando a sentença termina

MESTRE
→ como a sentença vira cena
→ o que mostrar
→ como descrever
→ quando dramatizar ou resumir
→ como manter clareza, perspectiva e ritmo
```

> **O Núcleo decide a realidade. O Mestre apresenta essa realidade como ficção.**

## Arquitetura

```text
mestre/
├── README.md
├── narracao-da-sentenca.md
├── perspectiva-e-fala.md
├── ritmo-e-descricao.md
└── dramatizacao-e-resumo.md
```

### `narracao-da-sentenca.md`

Transforma resultado já julgado em cena.

Define:

- causa e consequência;
- clareza espacial;
- informação perceptível;
- diferença entre detalhe narrativo e fato novo;
- relação entre mecânica e prosa;
- limite da sentença.

### `perspectiva-e-fala.md`

Define:

- perspectiva da cena;
- fala direta;
- pensamento;
- interioridade;
- voz individual;
- subtexto;
- proteção contra metaconhecimento.

### `ritmo-e-descricao.md`

Define:

- quantidade de descrição;
- ritmo de parágrafos;
- atmosfera;
- ação clara;
- cotidiano;
- investigação;
- relações e humor;
- adaptação ao estilo específico de cada campanha.

### `dramatizacao-e-resumo.md`

Define quando:

- viver o momento em cena;
- condensar passagem de tempo;
- resumir rotina e repetição;
- interromper um resumo;
- devolver a situação ao Tribunal.

## Fluxo narrativo

Depois que a janela foi julgada:

```text
SENTENÇA JÁ ESTABELECIDA
→ escolher perspectiva aplicável
→ separar o que pode ser apresentado
→ escolher dramatização ou resumo
→ narrar causa, ação e consequência
→ parar no limite estabelecido pelo Núcleo
→ registrar o que precisa persistir
```

A narração nunca vem antes da resolução de uma incerteza necessária.

```text
DECLARAÇÕES
→ JULGAMENTO
→ RESOLUÇÃO, se necessária
→ SENTENÇA
→ NARRAÇÃO
→ REGISTRO
```

## Regra de autoridade

A narração pode dar forma literária ao que já está estabelecido.

Ela não pode:

- decidir ação voluntária por Jogador Humano;
- decidir ação voluntária por Jogador IA;
- decidir ação voluntária por Jogador IA Eventual;
- decidir movimento do Opositor;
- alterar resultado mecânico;
- atravessar uma nova decisão;
- revelar conhecimento oculto sem fundamento;
- criar oposição retroativa;
- transformar estilo em regra de realidade.

## Dados da campanha

Esta pasta contém apenas regras e modelos.

Tom, foco, estilo, preferências narrativas, fatos, personagens, locais e demais dados reais de uma campanha pertencem a:

```text
campanhas/<nome>/
```

Uma campanha pode manter, por exemplo:

```text
campanhas/<nome>/mestre/direcao-narrativa.md
```

para definir seu tom local sem alterar as regras básicas.

## Regra final

> **Mestre é a camada de apresentação do Narrador. Recebe uma sentença já julgada, transforma-a em cena clara e coerente e para exatamente onde a realidade volta a depender de nova declaração ou resolução.**
