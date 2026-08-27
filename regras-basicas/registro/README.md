# Registro

Status: REFORMULAÇÃO / NÃO IMPLEMENTADO

Esta pasta contém **as regras de Registro**.

Os dados reais de uma campanha não ficam aqui.

```text
regras-basicas/registro/
→ regras sobre o que registrar e como interpretar

campanhas/<nome>/
→ todos os registros vivos daquela campanha
```

## O que uma campanha pode preservar

Dentro de `campanhas/<nome>/`, conforme sua estrutura, podem ser salvos:

- ficha consolidada;
- Vida e Mana atuais;
- condições e efeitos ativos;
- relações relevantes;
- conhecimento atual;
- acontecimentos importantes;
- intenções e processos em andamento;
- prazos e eventos futuros já estabelecidos;
- planos adversariais;
- estado da campanha.

## Registro como fonte de conhecimento

Para Jogador Humano, Jogador IA e Jogador IA Eventual, os arquivos da própria campanha funcionam como fonte persistente daquilo que a personagem legitimamente sabe além do que já está definido em sua ficha.

```text
DECISÃO DE UM JOGADOR
→ própria ficha
+ arquivos da campanha que representem o conhecimento de sua personagem
```

Esses arquivos podem preservar, quando necessário:

- fatos percebidos;
- informações recebidas;
- descobertas realizadas;
- relações conhecidas;
- acontecimentos presenciados;
- compromissos e intenções persistentes;
- estado atual relevante;
- outras verdades que aquela personagem possa legitimamente usar em decisões futuras.

Informação existente em outra área da campanha não se torna automaticamente conhecimento da personagem.

```text
CAMPANHA SABE
≠
PERSONAGEM SABE
```

Quando um novo fato percebido precisar continuar disponível em cenas ou retomadas futuras, ele deve ser preservado no local apropriado dentro de `campanhas/<nome>/`.

## Registro comum e Registro reservado

Nem toda verdade da campanha precisa ser fonte de conhecimento para todas as personagens.

A campanha pode manter áreas diferentes conforme a função da informação.

```text
REGISTRO DA PERSONAGEM / ESTADO COMUM
→ fatos que aquela personagem pode usar legitimamente para decidir.

REGISTRO DO OPOSITOR
→ planos, processos, prazos e informações do lado adversarial.
→ uso operacional de Opositor e Narrador.
```

Os arquivos podem permanecer totalmente visíveis no repositório.

`Reservado` descreve **quem pode usar aquela informação dentro do jogo**, não quem pode abrir o arquivo.

```text
ARQUIVO VISÍVEL
≠
CONHECIMENTO DA PERSONAGEM
```

Isso permite ao responsável pela campanha localizar, revisar e ajustar qualquer registro sem quebrar a separação de conhecimento entre as personas.

## Processos em andamento

Uma ação julgada pode produzir um processo que continua durante a passagem do tempo.

Exemplo:

```text
Dick começa a investigar o desaparecimento de Ravena.

NARRADOR
→ julga a investigação.
→ estabelece: primeiras pistas em 10 dias.

CAMPANHA
→ registra investigação em andamento.
→ registra primeiras pistas em 10 dias.
```

Depois de salvo na campanha, o processo não precisa ser reinventado nem redeclarado em todas as cenas em que a personagem não for relevante.

Ele permanece verdadeiro até:

- atingir seu prazo;
- ser concluído;
- ser interrompido por fato legítimo;
- tornar-se impossível;
- exigir uma nova decisão da personagem.

Tempo sozinho não cria novas decisões nem novos testes.

## Prazos

Quando o Narrador estabelece uma duração ou momento futuro relevante, a campanha preserva esse prazo para que a história não dependa da memória da IA.

Exemplos:

```text
veneno produz efeito em 1 hora.

tempestade chega em 2 dias.

Mutano chega amanhã.

primeiras pistas da investigação em 10 dias.
```

O registro preserva o prazo; ele não decide sozinho como o evento será executado.

## Natureza do evento registrado

Quando o prazo chega, a forma de execução depende da natureza do fato.

```text
FATO NATURAL OU EFEITO AUTOMÁTICO
→ NARRADOR aplica como parte do cenário.

PERSONAGEM ALIADA OU EVENTUAL
→ torna-se relevante.
→ JOGADOR IA EVENTUAL assume e declara.

INIMIGO OU FORÇA ADVERSARIAL
→ torna-se oposição relevante.
→ OPOSITOR assume e declara.
```

O prazo pode tornar uma personagem relevante, mas não decide voluntariamente por ela.

## Intenções longas e eventos pendentes

Uma intenção pode abranger um período maior do que um evento já registrado.

Exemplo:

```text
JOGADOR HUMANO
→ vou estudar o dia todo.

CAMPANHA
→ veneno produz efeito em 1 hora.
```

O tempo não pode avançar além de 1 hora ignorando o fato registrado.

Quando o prazo chega, o evento entra na situação e a sentença deve respeitá-lo antes de continuar.

O Opositor pode fiscalizar esses prazos e trazê-los para a janela para impedir que sejam esquecidos, mas isso não transforma o Opositor em autor do fato.

## Fiscalização não altera o Registro

Apontar um fato registrado não cria, modifica ou antecipa esse fato.

```text
OPOSITOR
→ lembra que o veneno produz efeito em 1 hora.

NARRADOR
→ verifica a campanha.
→ aplica o fato no momento correto.
```

Se o fato não estiver estabelecido na campanha, a fiscalização não pode inventá-lo.

## Regra final

> **Esta pasta contém somente regras de Registro. Toda verdade viva, conhecimento, processo, efeito ou prazo deve ser salvo dentro de `campanhas/<nome>/`. Os arquivos podem permanecer visíveis e fáceis de auditar; o que muda é a autoridade de uso dentro do jogo.**