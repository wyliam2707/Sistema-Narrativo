# Pareamento de informações entre fichas

Status: APROVADO

O pareamento é uma etapa de consistência cruzada realizada **depois que todas as fichas iniciais com agência foram aprovadas e antes de definir a situação inicial da história**.

Seu objetivo é descobrir somente as informações compartilhadas necessárias para que personagens relacionados sejam interpretados sem contradições.

> **Pareamento não é biografia completa. É apenas o mínimo necessário para as fichas conversarem entre si.**

## Princípio central

Quando a comparação entre fichas revelar uma lacuna realmente relevante, o narrador:

```text
compara as fichas relacionadas
→ identifica a próxima informação essencial que falta
→ faz UMA pergunta ao JOGADOR HUMANO
→ guarda a resposta sem alterar ainda as fichas
→ repete somente enquanto ainda houver lacuna importante
→ consolida as respostas
→ ajusta em conjunto todas as fichas afetadas
```

As perguntas são feitas uma por vez, mas as fichas não precisam ser alteradas a cada resposta.

## Regra de minimalidade

Perguntar apenas o que puder causar diferença real em:

- interpretação;
- conhecimento entre personagens;
- relação atual;
- história compartilhada importante;
- acesso ou confiança recorrente;
- continuidade da campanha.

Não transformar o pareamento em questionário exaustivo.

Não perguntar por:

- curiosidades;
- hábitos sem efeito narrativo;
- detalhes íntimos irrelevantes;
- cronologia minuciosa quando uma referência aproximada basta;
- informações de terceiros que não alterem nenhuma ficha atual;
- detalhes que podem surgir naturalmente durante o jogo sem criar contradição.

> **Se a informação pode tranquilamente ser descoberta em cena depois, normalmente ela não precisa ser definida no pareamento.**

## O que normalmente basta em um par

Para um par relevante, verificar somente quando necessário:

- se se conhecem;
- há quanto tempo, aproximadamente;
- como surgiu o vínculo, se isso importar;
- natureza atual da relação;
- fatos importantes que um sabe sobre o outro;
- segredos ou desconhecimentos que mudariam a interpretação;
- algum evento compartilhado essencial.

Nem todos esses itens precisam ser perguntados.

## Conhecimento é direcional

`A sabe X sobre B` não implica que `B sabe que A sabe X`.

Também não implica conhecimento total.

Registrar apenas o nível de conhecimento necessário para evitar erros de interpretação.

## Relações são direcionais

A relação de A com B pode diferir da relação de B com A.

O objetivo do pareamento é coerência cruzada, não simetria forçada.

## Relações de grupo

Quando existir um grupo recorrente, verificar apenas fatos coletivos essenciais que não estejam claros nas relações individuais.

Exemplo:

```text
Corvin + Wanda + Ravena
```

Pode ser suficiente saber que vivem juntos, há quanto tempo aproximadamente e qual é a natureza geral do vínculo. Rotinas menores podem surgir em jogo.

## Coleta sequencial, persistência em lote

Durante o pareamento:

```text
pergunta essencial
→ resposta
→ próxima pergunta essencial
→ resposta
→ ...
```

As respostas podem permanecer no contexto de trabalho.

Quando houver informação suficiente:

```text
consolidar respostas
→ atualizar somente os campos afetados
→ persistir todas as fichas necessárias em conjunto
→ encerrar o pareamento
```

Se uma resposta posterior corrigir uma anterior, vale a informação mais recente explicitamente dada pelo JOGADOR HUMANO.

## Ajuste das fichas

O pareamento pode atualizar fichas já `APROVADO` sem reiniciar os cinco blocos.

As fichas permanecem `APROVADO`.

Atualizar somente campos realmente afetados, principalmente:

- `Relações`;
- `Conhecimento atual relevante`;
- `História consolidada relevante`;
- `Recursos`, quando um vínculo concede acesso recorrente real;
- `Traços`, quando houver uma verdade estável que realmente importe.

Não duplicar a mesma informação em vários campos sem necessidade.

## Persistência

O pareamento não cria arquivo paralelo de campanha para repetir relações ou conhecimento.

As informações são persistidas diretamente nas fichas afetadas:

```text
personagens/<nome>.md
```

O checkpoint da campanha registra apenas onde retomar.

## Critério de encerramento

O pareamento termina quando já existe informação suficiente para começar a campanha sem contradições importantes entre as fichas.

Ele **não** precisa responder tudo sobre a vida dos personagens.

> **Pergunte o essencial, pare quando estiver suficiente e deixe o restante para a história.**
