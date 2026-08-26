# Pareamento de Informações

Status: APROVADO

O pareamento é uma etapa de **criação da campanha** realizada depois que todas as fichas iniciais com agência foram aprovadas e antes de definir a situação inicial da história.

> **Pareamento verifica se fichas relacionadas conseguem coexistir sem contradições importantes.**

Ele não define a mecânica das relações — isso pertence a `../personagem/relacoes.md` — e não cria uma nova fonte de persistência.

## Princípio central

Quando duas ou mais fichas relacionadas deixam uma lacuna realmente relevante:

```text
comparar as fichas
→ identificar a próxima lacuna essencial
→ fazer UMA pergunta ao JOGADOR HUMANO
→ guardar a resposta
→ repetir somente se ainda houver lacuna importante
→ consolidar o conjunto
→ atualizar as fichas afetadas
```

Perguntas são sequenciais; a persistência pode ser feita em lote ao final do conjunto.

## O que verificar

Somente quando necessário:

- se as pessoas se conhecem;
- há quanto tempo, aproximadamente;
- como surgiu o vínculo, se isso importar;
- natureza atual da relação;
- fatos importantes que uma sabe sobre a outra;
- segredos ou desconhecimentos relevantes;
- acesso, confiança ou obrigação recorrente;
- evento compartilhado essencial.

Não transformar pareamento em biografia completa.

> **Se a informação pode surgir normalmente em cena sem gerar contradição, ela provavelmente não precisa ser definida aqui.**

## Conhecimento é direcional

```text
A sabe algo sobre B
≠
B sabe que A sabe
```

Registrar somente o conhecimento necessário para evitar erro futuro de interpretação.

## Relações são direcionais

A relação de A com B pode ser diferente da relação de B com A.

Pareamento busca coerência, não simetria.

## Grupos

Quando houver grupo recorrente, definir apenas os fatos coletivos realmente necessários que não estejam claros nas relações individuais.

Rotinas menores podem surgir durante o jogo.

## Atualização das fichas

O pareamento pode atualizar fichas já `APROVADO` sem reiniciar a revisão em cinco blocos.

Atualizar somente campos afetados, principalmente:

- `REL`;
- conhecimento atual relevante;
- história consolidada relevante;
- RECURSOS quando o vínculo realmente concede acesso recorrente;
- Traços apenas quando surgir uma verdade estável que pertença à personagem.

O critério do que merece permanecer na ficha pertence a `../persistencia/relevancia-da-ficha.md`.

## Persistência

Não criar arquivo paralelo de relacionamento apenas para repetir a mesma informação.

As verdades aprovadas são consolidadas nas fontes adequadas conforme `../persistencia/`.

Se uma resposta posterior corrigir uma anterior durante a criação, vale a informação explícita mais recente.

## Encerramento

O pareamento termina quando já existe informação suficiente para iniciar a campanha sem contradições importantes entre as fichas.

Depois disso, `README.md` avança o checkpoint para **Início da história**.

## Regra final

> **Pareamento é uma verificação mínima de consistência entre fichas antes da primeira cena. Pergunte o essencial, consolide o aprovado e deixe o restante para a história.**
