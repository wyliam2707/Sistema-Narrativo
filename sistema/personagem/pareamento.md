# Pareamento de informações entre fichas

Status: APROVADO

O pareamento é uma etapa de consistência cruzada realizada **depois que todas as fichas iniciais com agência foram aprovadas e antes de definir a situação inicial da história**.

Seu objetivo é descobrir informações compartilhadas, assimetrias de conhecimento e relações históricas que só ficam claras quando duas ou mais fichas são comparadas.

> **Uma ficha pode estar correta sozinha e ainda estar incompleta em relação às outras. O pareamento verifica o que existe entre elas.**

## Princípio central

O pareamento não é uma revisão silenciosa feita pelo narrador.

Quando a comparação entre fichas revelar lacunas relevantes, o narrador:

```text
compara todas as fichas relacionadas
→ identifica internamente as perguntas que realmente importam
→ faz UMA pergunta ao JOGADOR HUMANO
→ guarda a resposta sem alterar ainda as fichas
→ faz a próxima pergunta necessária
→ repete até esclarecer as lacunas relevantes
→ consolida todas as respostas
→ ajusta em conjunto todas as fichas afetadas
→ verifica se ainda restou alguma lacuna cruzada relevante
```

Não presumir respostas apenas porque uma relação parece óbvia.

> **No pareamento, as perguntas são feitas uma por vez, mas as fichas não precisam ser alteradas a cada resposta. Primeiro esclarecemos; depois persistimos o conjunto.**

## Unidade de revisão

O pareamento trabalha principalmente em pares:

```text
A ↔ B
```

Para cada par relevante, verificar, quando fizer diferença:

- se eles se conhecem;
- há quanto tempo se conhecem;
- como ou em que contexto se conheceram;
- qual é a natureza atual da relação;
- o que A sabe sobre B;
- o que B sabe sobre A;
- quais fatos importantes viveram juntos;
- quais informações são assimétricas, secretas ou desconhecidas;
- que acesso, contato, confiança, obrigação ou rotina existe entre eles;
- o que um sabe sobre terceiros por causa dessa relação.

Nem todo item precisa virar pergunta. Perguntar apenas o que tiver efeito real sobre interpretação, decisão, continuidade ou coerência.

## A comparação gera perguntas, não respostas automáticas

Exemplo:

```text
Corvin tem 62 anos.
Nick Fury possui idade próxima.
A ficha de Nick diz que Corvin é consultor eventual da S.H.I.E.L.D.
```

Isso revela perguntas relevantes como:

```text
Há quanto tempo Nick e Corvin se conhecem?
Fury sabe que Corvin é mutante?
Fury sabe que ele é mago?
Fury conhece a regeneração e o envelhecimento retardado?
Fury sabe sobre Wanda e Ravena?
Ele sabe que os três vivem juntos?
```

O narrador não inventa essas respostas sozinho. Ele usa a comparação para decidir quais perguntas precisam ser feitas e apresenta **uma de cada vez** ao jogador.

## Coleta sequencial, persistência em lote

Durante o pareamento, a conversa continua simples:

```text
pergunta 1
→ resposta
→ pergunta 2
→ resposta
→ pergunta 3
→ resposta
→ ...
```

As respostas permanecem em contexto de trabalho enquanto o pareamento daquele conjunto ainda estiver aberto.

Não é necessário atualizar as fichas após cada resposta individual.

Quando todas as perguntas relevantes daquele par, grupo ou rodada estiverem respondidas:

```text
interpretar todas as respostas
→ resolver eventuais contradições
→ consolidar as consequências
→ atualizar todas as fichas afetadas em conjunto
→ persistir
→ fazer nova rodada somente se ainda houver lacunas relevantes
```

Esse formato preserva a regra de uma pergunta por vez sem produzir várias pequenas gravações durante o mesmo pareamento.

Se uma resposta posterior alterar ou corrigir uma resposta anterior, vale a informação mais recente explicitamente consolidada pelo JOGADOR HUMANO antes da persistência.

## Ajuste das fichas

O pareamento pode acrescentar ou corrigir conteúdo em fichas já `APROVADO` sem reiniciar toda a revisão em cinco blocos.

As fichas permanecem `APROVADO`.

Atualizar somente os campos realmente afetados, por exemplo:

- `Relações`;
- `Conhecimento atual relevante`;
- `História consolidada relevante`;
- `Recursos`, quando um vínculo concede acesso recorrente real;
- `Traços`, quando a relação cria uma verdade estável sobre o personagem.

Uma resposta pode exigir atualização em mais de uma ficha.

Exemplo:

```text
Fury conhece Corvin há 20 anos e sabe que sua aparência não envelhece normalmente.
```

Isso pode gerar:

```text
Nick Fury
→ História: conhece Corvin há 20 anos
→ Conhecimento: sabe sobre seu envelhecimento anormal

Corvin
→ História: relação profissional com Fury existe há 20 anos
```

As duas fichas não precisam usar texto idêntico; cada uma registra o que é relevante à sua própria perspectiva.

## Conhecimento é direcional

`A sabe X sobre B` não implica que `B sabe que A sabe X`.

Também não implica conhecimento total.

Registrar o nível de conhecimento necessário para evitar erros de interpretação.

Exemplo:

```text
Fury sabe que Corvin possui regeneração.
```

não significa automaticamente:

```text
Fury conhece os limites exatos da regeneração.
```

Segredos, suspeitas, informação parcial e informação errada podem ser preservados quando forem narrativamente relevantes.

## Relações são direcionais

O pareamento deve respeitar `relacoes.md`.

A relação de A com B pode diferir da relação de B com A em intensidade, confiança, afeto, obrigação ou conhecimento.

O objetivo do pareamento é coerência cruzada, não simetria forçada.

## Relações de grupo

Depois dos pares, verificar grupos recorrentes quando a relação coletiva tiver fatos próprios que não se reduzem aos pares.

Exemplo:

```text
Corvin + Wanda + Ravena
```

Perguntas possíveis:

- há quanto tempo vivem juntos;
- que rotina compartilham;
- o que terceiros sabem sobre a relação;
- quais espaços, recursos ou compromissos são realmente comuns aos três.

Só perguntar o que ainda não estiver consolidado.

## Ordem sugerida

Após todas as fichas iniciais aprovadas:

```text
listar os pares narrativamente relevantes
→ comparar todos eles
→ revisar grupos recorrentes, se houver
→ identificar as lacunas relevantes
→ fazer uma pergunta por vez
→ guardar as respostas enquanto o pareamento continua
→ quando o conjunto estiver esclarecido, ajustar em lote todas as fichas afetadas
→ confirmar que não restam lacunas cruzadas relevantes
→ somente então definir a situação inicial
```

Não é obrigatório parear personagens que praticamente não possuem vínculo ou cujo encontro ainda não ocorreu.

## Persistência

O pareamento **não cria um arquivo de campanha paralelo** para repetir relações ou conhecimento.

As respostas são persistidas diretamente nas fontes canônicas afetadas:

```text
personagens/<nome>.md
```

Se a resposta estabelecer uma verdade geral do cenário, ela pode pertencer a `mundo/` conforme as regras normais de persistência.

O checkpoint da campanha registra apenas onde retomar o pareamento.

Durante uma rodada ainda não concluída, as respostas podem permanecer apenas no contexto de trabalho; a persistência ocorre quando o conjunto necessário estiver suficientemente esclarecido.

## Regra final

> **Depois que as fichas individuais estiverem aprovadas, compare personagens que possuem vínculos relevantes. Identifique as lacunas, faça uma pergunta por vez ao JOGADOR HUMANO e acumule as respostas sem editar a ficha a cada turno. Quando o conjunto estiver esclarecido, ajuste em lote todas as fichas afetadas. Só depois do pareamento concluído a situação inicial da história é definida.**