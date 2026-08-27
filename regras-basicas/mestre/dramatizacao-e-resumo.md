# Dramatização e Resumo

Status: REFORMULAÇÃO / NÃO IMPLEMENTADO

Este arquivo define **quando o Narrador deve permanecer dentro da cena e quando pode condensar a passagem do tempo**.

> **Dramatizar o que precisa ser vivido. Resumir o que precisa apenas ter acontecido.**

## Dramatizar

Usar cena detalhada quando importarem:

- palavras exatas;
- reação observável;
- decisão;
- conflito;
- descoberta;
- revelação;
- mudança de relação;
- humor;
- ação decisiva;
- posição ou causalidade precisa.

Dramatizar significa mostrar o momento próximo da perspectiva em vez de saltar diretamente para o resultado final.

## Resumir

Usar resumo quando o principal é preservar que um intervalo aconteceu.

Exemplos:

- deslocamento sem acontecimento relevante;
- rotina repetitiva;
- treino sem novidade;
- pesquisa longa já julgada;
- trabalho repetido;
- recuperação;
- espera;
- dias semelhantes;
- processo já registrado em andamento.

Resumo não apaga consequência, prazo ou informação importante.

## Intenção longa

Uma intenção pode cobrir horas ou dias conforme `../nucleo/1.0-tribunal.md`.

Se a intenção já autoriza continuar e nenhuma nova decisão surgir, o Narrador pode condensar o período.

Exemplo:

```text
JOGADOR
→ vou passar a tarde estudando.

NARRADOR
→ julga a intenção.
→ nada relevante interfere.
→ resume a tarde até o ponto permitido.
```

O resumo não significa que todo período declarado precisa necessariamente ser consumido.

Se o objetivo terminar antes, a sentença pode parar antes.

## Processos registrados

Um processo já estabelecido pode avançar fora de cena sem precisar ser reencenado a cada janela distante.

Exemplo:

```text
REGISTRO
→ Dick investiga o desaparecimento.
→ primeiras pistas em 10 dias.
```

Enquanto nada exige nova decisão, a campanha pode avançar sem dramatizar cada dia da investigação.

Quando o prazo ou uma nova situação tornar Dick relevante novamente:

```text
→ parar o avanço aplicável
→ Jogador IA Eventual assume Dick
→ nova declaração
```

## Prazos interrompem resumo

O Narrador não resume por cima de um prazo registrado relevante.

Exemplo:

```text
JOGADOR
→ vou estudar o dia todo.

REGISTRO
→ veneno produz efeito em 1 hora.
```

A narração pode condensar no máximo até esse ponto.

```text
1 hora passa
→ veneno entra em efeito
→ consequência é aplicada
→ situação é reavaliada
```

O mesmo vale para:

- tempestade registrada;
- compromisso;
- chegada de aliado;
- entrada de inimigo;
- estágio de plano adversarial;
- condição que muda no tempo;
- outro fato já estabelecido.

## Aliado ou personagem eventual

Quando um resumo alcança o momento em que uma personagem eventual precisa escolher algo:

```text
RESUMO PARA
→ personagem torna-se relevante
→ JOGADOR IA EVENTUAL assume
→ Tribunal recebe nova declaração
```

O Narrador não escolhe a nova ação apenas para continuar o resumo.

## Inimigo ou força adversarial

Quando o resumo alcança uma entrada ou decisão adversarial:

```text
RESUMO PARA
→ força torna-se relevante
→ OPOSITOR assume ou declara movimento
→ Tribunal julga a nova situação
```

Um plano registrado não autoriza o Narrador a decidir como o vilão age quando chega o momento da escolha.

## Quando sair do resumo

Interromper a condensação quando surgir:

- nova decisão voluntária;
- informação capaz de mudar escolha;
- obstáculo não coberto pela intenção;
- oportunidade relevante;
- conflito;
- descoberta importante;
- personagem que precise ser assumida;
- movimento do Opositor;
- prazo ou efeito aplicável;
- mudança causal que torne o próximo passo incerto.

```text
RESUMO
→ algo muda
→ PARAR
→ apresentar a nova situação
→ abrir nova janela quando necessária
```

## Quando continuar resumindo

Uma fala casual, gesto rotineiro ou pequeno detalhe não exige automaticamente nova janela.

O resumo pode continuar quando:

- não surge escolha nova;
- a intenção continua cobrindo o próximo passo;
- nenhuma oposição entra;
- nenhum prazo interfere;
- nada muda as opções reais.

> **Não interromper por hábito. Interromper quando a ficção volta a precisar de agência ou julgamento.**

## Condensar sem virar relatório

Resumo ainda é narração.

Evitar:

```text
08h estudou
10h estudou
12h almoçou
14h estudou
```

Preferir uma passagem que preserve sensação de tempo e consequência:

```text
A manhã passa entre anotações e páginas marcadas. Depois do almoço, o trabalho continua sem novidade suficiente para alterar o plano.
```

Quando uma fala ou pequeno momento possuir valor de personagem, ele pode ser preservado dentro de uma passagem condensada.

## Cena tranquila não é resumo automático

Cotidiano pode ser dramatizado quando o valor está em:

- convivência;
- relação;
- humor;
- personalidade;
- conversa;
- mudança emocional legitimamente estabelecida.

Da mesma forma, ação longa pode ser resumida quando seu processo já está determinado e não exige novas escolhas.

## Mudança de tempo, lugar ou foco

Quando houver mudança clara, pode-se usar:

```text
* * *
```

A quebra ajuda orientação, mas não é obrigatória.

## Relação com o Registro

Resumo não substitui Registro.

Depois da sentença, fatos que precisem continuar verdadeiros devem ser preservados em `../registro/` e, quando forem específicos de uma campanha, dentro de `campanhas/<nome>/`.

## Regra final

> **Dramatize decisão, descoberta, conflito, relação e ação que precisa ser acompanhada. Resuma rotina, espera, repetição e processo já determinado. Nunca resuma através de um prazo, evento ou nova decisão que precise voltar ao Tribunal.**
