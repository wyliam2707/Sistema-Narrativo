# Criação de Temporada

Status: REFORMULAÇÃO / NÃO IMPLEMENTADO

Este arquivo define o **Passo 02** da criação: transformar a identidade da campanha em um arco atual que começa, se desenvolve e termina.

O Passo 01 está em `CRIACAO-DE-CAMPANHA.md`. O Passo 03 está em `jogador/1.3-criacao-da-ficha.md`.

> **A campanha diz sobre o que a história é. A temporada diz como esse foco será explorado agora.**

## Entrada

Antes de criar uma temporada, carregar:

```text
mestre/narrativa.md
```

Se não for a primeira temporada, carregar também apenas o necessário do encerramento anterior:

```text
epílogo da temporada anterior
+ fichas atualizadas
+ estado consolidado
+ problemas realmente abertos, quando relevantes
```

A nova temporada parte do que realmente aconteceu. Não reinicia relações, conhecimento, mudanças ou consequências já consolidadas.

## Perguntas da temporada

Responder apenas o necessário para criar um arco jogável:

```text
Onde esta temporada começa?
Por que estas personagens estão envolvidas agora?
Que situação sustenta o arco?
Qual problema, condição ou oportunidade move a temporada?
Existe prazo ou processo importante?
Que miniquests ou variações podem aparecer?
Como esta temporada explora o foco da campanha?
O que encerra esta temporada?
```

Não é necessário prever cenas, soluções ou resultados.

## Roteiro ativo

A temporada atual é registrada em:

```text
campanhas/<nome>/mestre/roteiro.md
```

Esse arquivo representa **somente a temporada ativa**.

Estrutura mínima:

```text
# Roteiro da Temporada [N]

Status: ATIVA

## Situação inicial
→ onde o arco começa e que condição coloca as personagens em movimento.

## Foco aplicado
→ como esta temporada explora a narrativa permanente da campanha.

## Trama de fundo
→ problema, situação ou oportunidade que sustenta o arco.

## Prazo / processo
→ quando existir algo que avance com o tempo.

## Miniquests / variações
→ conflitos menores que podem variar o ritmo sem substituir o foco.

## Direção da temporada
→ limites e orientações necessárias para preservar o arco atual.

## Condição de encerramento
→ o que precisa estar resolvido ou alcançado para esta temporada terminar.
```

Preencher somente os blocos que forem úteis.

## O roteiro não predetermina a história

```text
ROTEIRO
→ cria situação e direção.

PERSONAGENS
→ decidem como agir dentro dela.

NARRADOR
→ julga o encontro das decisões.
```

O roteiro não escolhe:

- quem vence;
- quem se apaixona;
- quem aceita uma proposta;
- como um mistério será resolvido;
- que decisão uma personagem tomará;
- qual miniquest crescerá em importância.

Ele também não transforma automaticamente um problema interessante em nova trama principal.

## Relação com a narrativa da campanha

`mestre/narrativa.md` continua sendo a identidade persistente.

```text
NARRATIVA
→ sobre o que a campanha é ao longo das temporadas.

ROTEIRO
→ o arco que está sendo jogado agora.
```

Uma temporada pode variar atmosfera, local, ameaça e ritmo sem apagar a identidade da campanha.

Mudança real da narrativa da campanha é uma decisão deliberada, não consequência automática de uma temporada diferente.

## Encerramento da temporada

Quando a condição de encerramento do roteiro for realmente alcançada:

```text
1. concluir somente a situação já em resolução;
2. não inventar um novo arco;
3. escrever o epílogo da temporada;
4. consolidar fichas e estado;
5. arquivar o roteiro encerrado;
6. perguntar: “E agora?”
```

### Epílogo

O epílogo registra **como a temporada realmente terminou**. Não decide um futuro que ainda não aconteceu.

Salvar em:

```text
campanhas/<nome>/livro/temporada-[N]-epilogo.md
```

Responder, conforme forem relevantes para aquela campanha:

```text
Onde as personagens terminaram?
Quais relações mudaram?
Quem está com quem?
Quem ainda vive ou trabalha junto?
Que conhecimento importante foi adquirido?
Que objetivos foram concluídos?
Que mudanças precisam permanecer nas fichas?
Que problemas realmente ficaram abertos?
```

As perguntas do epílogo acompanham o tipo de história. Em romance, relações podem ser centrais; em terror, sobreviventes, medos, perdas e ameaças conhecidas podem importar mais; em investigação, fatos confirmados e casos pendentes podem receber prioridade.

> **O epílogo consolida o resultado real da temporada. Não cria a próxima.**

## Arquivar o roteiro encerrado

Antes de substituir `mestre/roteiro.md`, preservar a temporada concluída em:

```text
campanhas/<nome>/mestre/temporadas/temporada-[N].md
```

O arquivo arquivado recebe:

```text
Status: ENCERRADA
```

O roteiro encerrado deixa de dirigir o jogo atual.

## “E agora?”

Depois do epílogo e da consolidação, perguntar simplesmente:

> **E agora?**

A resposta define a direção da próxima temporada.

Exemplos de resposta:

```text
quero explorar a vida dos três fora da cidade
quero uma temporada em Tamaran
quero alguns meses de cotidiano
quero uma temporada de terror
quero investigar um problema que ficou aberto
```

Um problema aberto no epílogo **não vira automaticamente a Temporada 2**.

```text
PROBLEMA CONTINUA EXISTINDO
≠
PRÓXIMA TEMPORADA É SOBRE ELE
```

Somente depois da resposta a “E agora?” criar o novo `mestre/roteiro.md`.

## Temporadas seguintes e fichas

Antes de iniciar uma nova temporada, não reconstruir todas as fichas do zero.

Usar:

```text
narrativa da campanha
+ novo roteiro
+ fichas consolidadas
+ epílogo anterior
```

Se o novo arco tornar importante uma área interpretativa ainda pouco definida, revisar apenas os blocos necessários conforme `jogador/1.3-criacao-da-ficha.md`.

## Regra final

> **Toda temporada nasce da narrativa da campanha, possui um roteiro próprio e uma condição de encerramento. Quando termina, o Narrador escreve um epílogo do que realmente ficou estabelecido, consolida as fontes, arquiva o roteiro e pergunta “E agora?”. Só a resposta a essa pergunta autoriza a criação da próxima temporada.**