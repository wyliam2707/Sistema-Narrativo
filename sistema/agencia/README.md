# Agência

Status: APROVADO

Esta pasta define como personagens e forças do mundo continuam capazes de agir sem transformar a campanha em uma simulação permanente de tudo que existe.

A imagem mental operacional pertence a `../personas/README.md`:

> **Os jogadores defendem e movimentam suas próprias peças. O OPOSITOR observa a mesa, guarda ganchos e movimenta a parte adversarial da ficção. O NARRADOR julga, narra a sentença e registra.**

## Princípio central

Todo personagem que está efetivamente em uma cena possui agência compatível com:

- quem ele é;
- o que sabe;
- o que quer;
- sua situação;
- suas capacidades e limitações.

Isso vale independentemente de sua `IMPORTÂNCIA`.

Um Figurante presente em cena não vira ferramenta automática do roteiro. Ele pode recusar, fugir, mentir, ajudar, ter medo, mudar de ideia ou agir de outra forma coerente.

> **IMPORTÂNCIA não concede agência. CONTROLE não define personalidade. Todo personagem em cena age como uma peça própria.**

## Fora de cena não significa simular tudo

Quando um personagem sai da cena, não é necessário continuar simulando sua vida apenas porque ele existe.

Pergunta operacional:

> **Existe alguma continuidade causal que ainda pode voltar a mover a história?**

Se não houver:

```text
sem pendência
+ sem plano relevante
+ sem retorno estabelecido
+ sem consequência viva
→ pode sair do acompanhamento.
```

Se houver:

```text
retorno
prazo
promessa
objetivo
plano
consequência
relação ativa
ou outra ponta útil
→ preservar somente o necessário.
```

Não acompanhar cada hora ou dia intermediário.

## Ganchos do OPOSITOR

Qualquer ponta útil que possa voltar a movimentar a história pode ser guardada pelo OPOSITOR.

Exemplos:

```text
- Ravena sente ciúme de Fulana quando ela está perto de Corvin.
- Corvin contou que não fala com o irmão há dez anos.
- O credor pode voltar entre 18 e 30 dias.
- Trigon pretende sequestrar Ravena antes do fim da semana.
```

Quando houver ganchos ativos, a campanha pode usar:

```text
campanhas/<nome>/mestre/ganchos-do-opositor.md
```

O arquivo é uma lista simples de oportunidades atuais. Não é histórico nem roteiro.

```text
gancho ainda serve
→ permanece.

gancho mudou
→ atualizar.

gancho deixou de servir ou deixou de ser verdadeiro
→ apagar.
```

Regras completas:

- `ganchos-do-opositor.md`

## Planos maiores

Personagens importantes e antagonistas podem possuir objetivos ou planos que continuam vivos fora de cena.

Exemplo:

```text
Trigon quer usar Ravena para abrir caminho à Terra.
```

Isso pode permanecer como gancho disponível ao OPOSITOR.

O OPOSITOR pode tentar fazer o plano avançar, escolher oportunidades, mudar de abordagem depois de uma falha e usar NPCs ou recursos legitimamente disponíveis.

O plano não garante o resultado.

> **O plano pertence à peça. O gancho preserva a oportunidade. O OPOSITOR movimenta. O NARRADOR julga.**

## NPCs e delegação

O OPOSITOR não controla automaticamente todos os NPCs e forças do mundo.

Quando uma oposição concreta exigir agência adversária, o NARRADOR julga quais peças realmente existem e podem participar.

Se forem válidas, pode delegá-las temporariamente ao OPOSITOR.

```text
NARRADOR
→ julga se a peça existe, sabe, pode e consegue agir.

OPOSITOR
→ recebe a peça e joga suas decisões durante aquela oposição.

NARRADOR
→ julga as declarações dos dois lados.
```

Ao terminar a oposição, a delegação termina. A peça continua sendo NPC.

## Conhecimento separado

Conhecimento operacional de uma persona não vira automaticamente conhecimento da peça que ela movimenta.

```text
PERSONA SABE
≠
PERSONAGEM SABE
```

O OPOSITOR pode enxergar uma ponta solta porque observa a mesa inteira. Um NPC só pode agir com base nela se possuir meio legítimo de conhecê-la.

## Importância e continuidade

`IMPORTÂNCIA` indica peso estrutural, não obrigação de simular continuamente o personagem.

Um personagem Central pode passar semanas fora da câmera sem exigir decisões diárias.

Um Figurante pode deixar um fio futuro importante e precisar voltar depois.

Exemplo:

```text
Figurante
→ prometeu entregar um documento amanhã
→ preservar o fio até amanhã.
```

O que determina acompanhamento fora da cena é a existência de **continuidade causal útil**, não apenas a classificação estrutural.

## Arquivos desta área

- `ganchos-do-opositor.md` — lista simples de oportunidades, pontas, planos e informações que o OPOSITOR pode voltar a usar.
- `continuidade-de-npcs.md` — quando NPCs precisam continuar sendo acompanhados e quando podem ser esquecidos.
- `continuidade-de-jogadores-ia.md` — continuidade de personagens controlados por IA fora da câmera.

## Relação com outras áreas

```text
personas/
→ quem possui qual autoridade na mesa.

personagem/
→ quem a peça é e do que é capaz.

agencia/
→ como vontade, objetivos, fios e decisões continuam ao longo da ficção.

operacao/
→ em que ordem as declarações entram numa janela de cena.

persistencia/
→ onde o resultado e os fios vivos são registrados.
```

## Regra final

> **Em cena, todo personagem é uma peça com agência própria. Fora da cena, acompanhe apenas o que ainda pode voltar a importar. Pontas úteis viram ganchos do OPOSITOR; pontas mortas são esquecidas.**
