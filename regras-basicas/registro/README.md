# Registro

Status: REFORMULAÇÃO / NÃO IMPLEMENTADO

Reúne as regras sobre o que precisa continuar verdadeiro entre ações, cenas, capítulos e retomadas.

Inclui, quando forem definidas:

- ficha consolidada;
- Vida e Mana atuais;
- condições e efeitos ativos;
- relações relevantes;
- conhecimento atual;
- acontecimentos importantes;
- intenções e processos em andamento;
- prazos e eventos futuros já estabelecidos;
- estado da campanha.

## Registro como fonte de conhecimento

Para Jogador Humano, Jogador IA e Jogador IA Eventual, o Registro funciona como a fonte persistente daquilo que a personagem legitimamente sabe além do que já está definido em sua própria ficha.

```text
DECISÃO DE UM JOGADOR
→ própria ficha
+ Registro que represente o conhecimento de sua personagem
```

O Registro pode preservar, quando necessário:

- fatos percebidos;
- informações recebidas;
- descobertas realizadas;
- relações conhecidas;
- acontecimentos presenciados;
- compromissos e intenções persistentes;
- estado atual relevante;
- outras verdades que aquela personagem possa legitimamente usar em decisões futuras.

Informação existente em outra fonte do sistema não se torna automaticamente conhecimento da personagem.

```text
SISTEMA SABE
≠
PERSONAGEM SABE
```

Quando um novo fato percebido precisar continuar disponível em cenas ou retomadas futuras, ele deve ser preservado no Registro apropriado.

## Registro comum e Registro reservado

Nem toda verdade da campanha precisa ser fonte de conhecimento para todas as personagens.

O sistema pode manter áreas diferentes de Registro conforme a função da informação.

```text
REGISTRO COMUM / DA PERSONAGEM
→ fatos que aquela personagem pode usar legitimamente para decidir.

REGISTRO RESERVADO DO OPOSITOR
→ planos, processos, prazos e informações do lado adversarial.
→ uso operacional de Opositor e Narrador.
```

O Registro reservado pode permanecer totalmente visível no repositório.

`Reservado` descreve **quem pode usar aquela informação dentro do jogo**, não quem pode abrir o arquivo.

```text
ARQUIVO VISÍVEL
≠
CONHECIMENTO DA PERSONAGEM
```

Isso permite ao responsável pela campanha localizar, revisar e ajustar qualquer arquivo sem quebrar a separação de conhecimento entre as personas.

## Processos em andamento

Uma ação julgada pode produzir um processo que continua durante a passagem do tempo.

Exemplo:

```text
Dick começa a investigar o desaparecimento de Ravena.

NARRADOR
→ julga a investigação.
→ estabelece: primeiras pistas em 10 dias.

REGISTRO
→ investigação de Dick em andamento.
→ primeiras pistas em 10 dias.
```

Depois de registrado, o processo não precisa ser reinventado nem redeclarado em todas as cenas em que a personagem não for relevante.

Ele permanece verdadeiro até:

- atingir seu prazo;
- ser concluído;
- ser interrompido por fato legítimo;
- tornar-se impossível;
- exigir uma nova decisão da personagem.

Tempo sozinho não cria novas decisões nem novos testes.

## Prazos

Quando o Narrador estabelece uma duração ou momento futuro relevante, o Registro preserva esse prazo para que a história não dependa da memória da IA.

Exemplos:

```text
veneno produz efeito em 1 hora.

tempestade chega em 2 dias.

Mutano chega amanhã.

primeiras pistas da investigação em 10 dias.
```

O Registro preserva o prazo; ele não decide sozinho como o evento será executado.

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

Exemplos:

```text
tempestade chega
→ Narrador aplica.

veneno produz efeito
→ Narrador aplica conforme a regra estabelecida.

Mutano chega
→ Eventual assume Mutano.

inimigo entra em campo
→ Opositor assume a força adversarial.
```

O prazo pode tornar uma personagem relevante, mas não decide voluntariamente por ela.

## Intenções longas e eventos pendentes

Uma intenção pode abranger um período maior do que um evento já registrado.

Exemplo:

```text
JOGADOR HUMANO
→ vou estudar o dia todo.

REGISTRO
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
→ verifica o Registro.
→ aplica o fato no momento correto.
```

Se o fato não estiver estabelecido, a fiscalização não pode inventá-lo.

## Regra final

> **Registro preserva verdades, conhecimentos, processos, efeitos e prazos já estabelecidos. Os arquivos podem permanecer visíveis e fáceis de auditar; o que muda entre registros é a autoridade de uso dentro do jogo. Fatos naturais e efeitos automáticos pertencem ao Narrador; personagens eventuais retornam ao Jogador IA Eventual; forças adversariais retornam ao Opositor.**