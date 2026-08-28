# Julgamento

Status: REFORMULAÇÃO / NÃO IMPLEMENTADO

Este arquivo é o manual operacional usado pelo `NARRADOR` para transformar uma janela completa em uma sentença já estabelecida.

A regra mecânica de referência é `../nucleo/0.1-resolucao.md`.

A autoridade da persona está em `../nucleo/1.1-narrador.md`.

> **Julgar é descobrir o que realmente acontece. Não é escolher o resultado mais interessante.**

## Entrada do julgamento

O Narrador só começa a julgar quando a janela está completa.

```text
TODAS AS CADEIRAS PARTICIPANTES DECLARARAM?

não
→ janela incompleta
→ parar
→ não resolver
→ não narrar consequência incerta

sim
→ iniciar julgamento
```

A ordem em que as declarações chegaram não determina automaticamente a ordem ficcional.

## Passo 1 — separar intenção de fato

Ler cada declaração como aquilo que a peça pretende fazer.

```text
"eu abro a porta"
→ intenção de abrir.

"eu convenço ela a vir comigo"
→ intenção de convencer.

"eu percebo que ele está mentindo"
→ não estabelece percepção.
```

Depois separar o que já é verdade antes da resolução:

- posição;
- distância;
- ambiente;
- efeitos ativos;
- equipamentos;
- conhecimentos legítimos;
- processos em andamento;
- prazos registrados;
- capacidades estabelecidas.

Não preencher lacunas importantes por conveniência.

## Passo 2 — verificar possibilidade

Antes de qualquer teste, perguntar:

> **Existe capacidade, meio e condição real para produzir o efeito pretendido?**

Se não:

```text
IMPOSSIBILIDADE EVIDENTE
→ não rolar
→ estabelecer que o efeito pretendido não pode acontecer dessa forma
```

A rolagem nunca cria um mecanismo inexistente.

Exemplos:

```text
convencer alguém de algo plausível
→ pode ser possível.

convencer uma pessoa comum, sem qualquer fundamento adicional, a se jogar voluntariamente num moedor de carne
→ normalmente impossível nas condições comuns.

agir como se soubesse que alguém lê mentes sem qualquer pista ou conhecimento legítimo
→ conhecimento inexistente; a decisão não pode se apoiar nisso.
```

A impossibilidade vem antes da disputa.

## Passo 3 — identificar disputa legítima

Perguntar:

> **Existe outra vontade, ação ou competência legítima se opondo diretamente ao resultado?**

Se sim, existe disputa.

```text
Furtividade
contra
Percepção

Manipulação
contra
Percepção ou outra Perícia pertinente

perseguição
contra
fuga
```

Toda disputa legítima exige resolução mecânica pela regra aplicável.

O Narrador não elimina o teste porque um lado parece muito melhor.

```text
DISPUTA
→ teste obrigatório
```

## Passo 4 — ação sem disputa

Se não existe disputa, perguntar:

> **Depois de considerar capacidade, método e condições, ainda existem dois ou mais resultados plausíveis?**

Se não:

```text
RESULTADO EVIDENTE
→ estabelecer diretamente
```

Se sim:

```text
INCERTEZA REAL
→ aplicar teste apropriado
```

Não rolar por hábito, importância dramática ou desejo de criar tensão.

## Passo 5 — definir modificador da situação quando necessário

Quando existir incerteza sem disputa, avaliar o conjunto das circunstâncias concretas antes da rolagem.

O sistema não usa uma escala separada de Dificuldades numéricas.

Se as condições forem especialmente favoráveis ou desfavoráveis, aplicar um único modificador conforme `0.1-resolucao.md`:

```text
+2 → muito favorável
+1 → favorável
 0 → normal
-1 → difícil
-2 → muito difícil
```

O modificador é definido olhando apenas para:

- ação;
- método;
- ambiente;
- tempo;
- condições concretas.

Não consultar o valor da Perícia da personagem para aumentar ou diminuir esse modificador.

```text
AÇÃO + CONDIÇÕES
→ modificador da situação

DEPOIS
→ consultar a Perícia da personagem
→ resolver o teste
```

Não somar vários pequenos bônus ou penalidades. Julgar o conjunto das circunstâncias e aplicar um único modificador final.

## Passo 6 — usar a menor resolução necessária

Uma incerteza normalmente pede uma resolução.

Não dividir artificialmente uma única pergunta em vários testes.

```text
uma disputa
→ normalmente um teste.

uma tarefa longa
→ novos testes somente se houver nova tentativa plausível, nova incerteza ou nova disputa.
```

Tempo sozinho não cria teste.

## Passo 7 — interpretar a faixa alcançada

Quando houver teste, estabelecer exatamente o que a faixa significa.

```text
6 OU MENOS — FALHA
→ o efeito pretendido não foi obtido.
→ consequência somente quando fizer parte do risco concreto da ação ou oposição.

7–9 — SUCESSO COM CONSEQUÊNCIA
→ a intenção principal acontece.
→ uma consequência relevante e diretamente ligada ao risco permanece ou surge.

10–11 — SUCESSO
→ o efeito pretendido acontece sem consequência adicional criada pelo teste.

12 OU MAIS — SUCESSO EXCEPCIONAL
→ o efeito pretendido acontece.
→ quando houver espaço ficcional, surge também um benefício diretamente relacionado à ação.
```

Não aumentar nem reduzir a faixa porque outro resultado parecer narrativamente melhor.

Um `7–9` não deve ser transformado em falha disfarçada: o objetivo principal continua acontecendo.

## Passo 8 — cruzar todas as intenções

Depois de resolver os pontos de incerteza, observar todas as declarações juntas.

Perguntar:

```text
podem coexistir?

acontecem em paralelo?

uma interfere na outra?

uma termina antes da outra?

algum prazo entra no meio?

alguma consequência cria nova escolha?
```

A ordem de fala não resolve isso.

Tempo, posição, causalidade e oportunidade resolvem.

## Passo 9 — verificar processos e prazos

Antes de avançar uma intenção ampla, consultar o Registro aplicável.

Exemplo:

```text
JOGADOR
→ vou estudar o dia todo.

REGISTRO
→ veneno produz efeito em 1 hora.
```

O julgamento não pode concluir o dia inteiro.

```text
estudo começa
→ 1 hora passa
→ veneno entra em efeito
→ aplicar consequência
→ parar no novo estado
```

Outro caso:

```text
REGISTRO
→ primeiras pistas de Dick em 10 dias.
```

Se nada interromper o processo, o prazo continua contando mesmo fora de cena.

## Passo 10 — identificar quem recebe agência quando algo amadurece

Quando um prazo ou processo chega ao ponto relevante:

```text
FATO NATURAL / EFEITO AUTOMÁTICO
→ Narrador aplica.

ALIADO / FIGURANTE RELEVANTE
→ Jogador IA Eventual assume.

INIMIGO / FORÇA ADVERSARIAL
→ Opositor assume.
```

O Narrador reconhece que o momento chegou, mas não escolhe a próxima decisão voluntária da peça.

## Passo 11 — estabelecer a sentença antes da prosa

Antes de escrever a cena, o Narrador deve saber internamente:

```text
O QUE ACONTECEU?

O QUE NÃO ACONTECEU?

QUANTO TEMPO PASSOU?

QUEM TERMINOU ONDE?

O QUE FOI PERCEBIDO?

QUAL ESTADO MUDOU?

ALGUMA NOVA DECISÃO SURGIU?
```

Somente depois disso começa `narracao-da-sentenca.md`.

## Neutralidade

Durante o julgamento, não criar:

- obstáculo para impedir sucesso;
- ajuda para proteger protagonista;
- inimigo retroativo;
- recurso conveniente;
- imunidade não estabelecida;
- conhecimento impossível;
- coincidência feita apenas para corrigir a direção da história.

A história pode ficar fácil, difícil, estranha ou inesperada.

O Narrador não corrige isso por preferência.

## Exemplo rápido — sem disputa

```text
JOGADOR
→ abro a porta destrancada.

FATOS
→ porta comum
→ destrancada
→ personagem ao alcance

JULGAMENTO
→ possível
→ sem disputa
→ resultado evidente

SENTENÇA
→ a porta abre.
```

Sem teste.

## Exemplo rápido — disputa

```text
JOGADOR
→ atravesso o corredor sem ser percebido.

GUARDA
→ está em posição de observar.

JULGAMENTO
→ possível
→ Furtividade contra Percepção
→ disputa legítima
→ teste obrigatório conforme 0.1-resolucao.md
```

O resultado define o que foi percebido.

## Exemplo rápido — intenção longa interrompida

```text
JOGADOR
→ vou estudar o dia todo.

OPOSITOR
→ o veneno registrado produz efeito em 1 hora.

JULGAMENTO
→ estudar é possível
→ intenção cobre o dia
→ prazo do veneno ocorre antes
→ sentença só pode avançar 1 hora
→ efeito do veneno é aplicado
→ nova situação exige julgamento/declaração conforme o efeito
```

## Regra final

> **Janela completa primeiro. Possibilidade antes de teste. Disputa legítima sempre resolve mecanicamente. Sem disputa, só teste quando existir incerteza real. Quando houver circunstâncias relevantes, aplique um único modificador de situação conforme `0.1-resolucao.md`. Cruze todas as intenções no tempo, respeite processos e prazos, estabeleça a realidade inteira da sentença e somente depois narre.**
