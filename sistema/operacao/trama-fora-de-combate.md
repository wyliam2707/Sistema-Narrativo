# Trama Fora de Combate

Status: APROVADO

Este arquivo define **como o JOGADOR HUMANO declara Trama durante janelas de cena fora de combate**.

Os custos e efeitos de Trama pertencem a `../personagem/trama.md`. Este arquivo define somente o momento da declaração e a forma operacional de resolução.

> **Fora de combate, Trama usada para reforçar uma ação é declarada pelo JOGADOR HUMANO junto da própria intenção.**

## Regra central

Quando o JOGADOR HUMANO quiser usar Trama para melhorar uma rolagem ou reduzir uma penalidade de dados fora de combate, deve declarar o gasto junto da ação que está propondo.

```text
JOGADOR HUMANO
→ declara intenção
→ declara gasto de Trama, se quiser

NARRADOR
→ recebe a intenção já configurada
→ julga
→ resolve somente a mecânica necessária
→ narra o resultado
```

Exemplo:

```text
JOGADOR HUMANO
→ vou saltar o muro e entrar pelo jardim. Gasto 5 de Trama.
```

O gasto faz parte daquela intenção e é aplicado antes da resolução correspondente.

## Sem janela automática

Fora de combate, o NARRADOR não interrompe a cena apenas para perguntar se o jogador deseja usar Trama para melhorar uma ação.

```text
Trama declarada junto da intenção
→ aplicar normalmente

Trama não declarada
→ resolver normalmente sem bônus de Trama
```

Depois que o resultado daquela resolução já estiver estabelecido, não oferecer retroativamente Trama para alterar a rolagem.

> **No combate, a operação pergunta. Fora de combate, o jogador anuncia.**

A rotina obrigatória de oferta pertence exclusivamente a `rotina-de-trama-em-combate.md`.

## Etapa mecânica separada da prosa

Quando houver incerteza objetiva, o NARRADOR pode separar a resposta em duas partes consecutivas:

```text
ETAPA DE RESOLUÇÃO
→ mostrar somente a mecânica mínima necessária
→ estabelecer o resultado

APRESENTAÇÃO DA CENA
→ transformar esse resultado em ficção
```

Essa separação não cria Turno, Rodada ou Iniciativa fora de combate. É apenas uma divisão de apresentação.

Formato mecânico preferido:

```text
Teste: 5d6 mantém 4 + CON [2] | CD 16
Resultado: sucesso | Trama 25/30
```

Mostrar somente o necessário para o jogador compreender a resolução. Não expor cálculos intermediários, justificativas longas ou mecânica que não altere sua compreensão da cena.

## Resolução pode ocupar uma resposta própria

Quando for útil para clareza, a etapa mecânica pode ser apresentada em uma resposta própria antes da narração conclusiva.

```text
resposta de resolução
→ mecânica mínima
→ resultado estabelecido

resposta narrativa seguinte
→ cena já baseada no resultado estabelecido
```

Isso não devolve automaticamente uma nova decisão ao jogador entre as duas partes. Se a resolução não criou nova escolha relevante, a narração continua pertencendo à mesma janela causal.

Se a própria resolução criar uma nova decisão relevante, aplicar `janelas-e-interrupcoes.md` e parar antes de narrar além desse ponto.

## Outros usos de Trama

Usos de Trama que dependem de uma condição conhecida apenas durante a resolução continuam obedecendo ao momento causal definido em `../personagem/trama.md`.

Esta regra de declaração conjunta é especialmente aplicável a:

```text
melhorar uma rolagem
reduzir penalidade de dados
```

Ela não autoriza uso retroativo depois que o resultado já foi estabelecido.

## Regra final

> **Fora de combate, o JOGADOR HUMANO declara junto da intenção qualquer Trama usada para reforçar aquela ação. O NARRADOR resolve somente a mecânica necessária, pode apresentá-la em etapa separada e depois narra a cena. Não existe oferta automática de Trama nem uso retroativo após o resultado.**
