# Turnos de Combate

Status: APROVADO

Este arquivo define **como o tempo é dividido quando existe combate ativo**.

As mecânicas de ataque, Dano, Cura, Mana, Poderes, Status, proteção, contenção e demais resoluções pertencem a `../resolucao/`.

> **Operação organiza o tempo. Resolução calcula o resultado.**

## Regra central

Durante combate, a ficção é dividida em **turnos simultâneos de até 10 segundos**.

Esses 10 segundos pertencem a todas as peças envolvidas.

O turno não concede uma única ação e não cria uma economia abstrata de ações.

Ele limita quanto da disputa pode ser resolvido antes que todos recebam nova oportunidade de decidir.

```text
TURNO DE COMBATE
→ até 10 segundos compartilhados
→ todas as peças podem agir, reagir ou interferir
→ o NARRADOR julga o mesmo intervalo para todos
```

## Ordem operacional do turno

Cada turno usa as mesmas cadeiras da mesa:

```text
1. JOGADOR HUMANO declara para o turno
↓
2. JOGADORES IA aplicáveis declaram, cada um por sua peça
↓
3. JOGADOR IA EVENTUAL declara pelas peças ativas, se houver
↓
4. OPOSITOR declara pelas peças e recursos adversários disponíveis
↓
5. NARRADOR JULGA o intervalo
↓
6. NARRADOR NARRA A SENTENÇA
↓
7. NARRADOR REGISTRA o estado resultante
↓
8. próximo turno, se o combate continuar
```

A ordem de declaração organiza autoridade. Ela **não determina automaticamente a ordem cronológica das ações** dentro do turno.

## Simultaneidade

As peças estão agindo dentro do mesmo intervalo.

O NARRADOR julga precedência e interferência conforme os fatos e as regras aplicáveis, incluindo quando relevante:

- velocidade;
- distância;
- surpresa;
- preparação;
- posição;
- oportunidade;
- mecanismo da ação;
- ação já iniciada;
- interferência entre as peças.

Exemplo:

```text
JOGADOR
→ saco a arma e atiro.

OPOSITOR
→ o guarda, que já estava com a arma apontada, dispara.

NARRADOR
→ julga a precedência dentro dos mesmos segundos do turno.
```

Declarar primeiro não significa agir primeiro.

Quando duas intenções realmente competirem pelo mesmo instante e nenhum fato estabelecer precedência, a resolução pode usar uma **oposição comum** com os Atributos coerentes de cada abordagem.

Esse teste resolve somente aquela precedência local e não cria iniciativa para os turnos seguintes.

## Declaração ampla em combate

Uma declaração ampla continua sendo uma intenção válida, mas não pode resolver antecipadamente vários intervalos de oposição.

Exemplo:

```text
JOGADOR
→ entro na sala e mato todo mundo.
```

Leitura operacional:

```text
OBJETIVO
→ entrar na sala
→ tentar derrotar todos os adversários
```

O primeiro turno resolve somente aquilo que realmente pode ocorrer dentro de até 10 segundos.

Durante o mesmo intervalo, os adversários também podem:

- atacar;
- fugir;
- procurar cobertura;
- render-se;
- usar poderes;
- pedir ajuda;
- mudar de posição;
- executar outra ação legítima.

> **A intenção ampla define o objetivo. O turno impede que o objetivo apague as ações e reações das outras peças.**

Se o objetivo continuar depois da sentença, no turno seguinte a peça pode simplesmente declarar que continua o mesmo plano ou alterá-lo diante da nova situação.

## Limite da sentença

A sentença de combate não pode atravessar o turno.

Ela termina no primeiro destes limites:

```text
SURGE NOVA DECISÃO RELEVANTE ANTES DO LIMITE
→ parar no ponto causal da mudança

CHEGA AO LIMITE DE 10 SEGUNDOS
→ fechar o turno
```

Assim, mesmo uma intenção que levaria muito mais tempo precisa ser acompanhada turno a turno enquanto o combate permanecer ativo.

## Fechamento mecânico

Antes do próximo turno, todas as consequências mecânicas produzidas pelo intervalo resolvido devem estar aplicadas ao estado atual.

Isso inclui somente quando for pertinente:

```text
Vida e Dano
Mana
Trama, quando aplicável
Poderes e seus efeitos ativos
Status
Barreiras e proteções
alterações temporárias de Atributo
posição relevante
outros valores afetados
```

Nenhum desses cálculos é redefinido aqui.

Usar as fontes atuais:

```text
../resolucao/combate-e-dano.md
../resolucao/vida.md
../resolucao/mana.md
../resolucao/poderes/
../resolucao/status/
../personagem/trama.md
```

O registro final segue `../persistencia/`.

> **Antes do próximo turno, a mesa precisa saber como cada peça realmente terminou o intervalo anterior.**

## Início do combate

O relógio de turnos começa quando existe confronto ativo em que várias peças podem agir, reagir ou interferir em intervalos curtos e concorrentes.

Não é necessário esperar o primeiro ataque causar Dano.

Uma perseguição imediata, invasão já contestada, duelo, troca de poderes ou outra disputa física em tempo curto pode justificar a entrada em turnos.

## Fim do combate

O relógio deixa de ser necessário quando a disputa curta e concorrente termina.

Exemplos:

- oposição derrotada;
- rendição;
- fuga efetivamente concluída;
- separação que encerra a interação imediata;
- conflito deixa de exigir acompanhamento em segundos.

Depois disso, volta a valer `janelas-e-interrupcoes.md`.

## Relação com as mecânicas

Turno de 10 segundos **não altera as regras de resolução**.

```text
OPERAÇÃO
→ define o intervalo e a oportunidade de decisão

RESOLUÇÃO
→ define testes, Defesa, Dano, Cura, Poderes, Status, custos e demais consequências

PERSISTÊNCIA
→ guarda o estado resultante
```

Se uma mecânica possui duração, custo, aplicação ou referência temporal própria, seguir a regra específica dela. O turno apenas fornece o relógio comum do combate.

## Regra final

> **Em combate, todas as peças compartilham turnos simultâneos de até 10 segundos. A ordem de declaração não é iniciativa; uma intenção ampla não resolve vários turnos de uma vez; as mecânicas continuam em `resolucao/`; e cada turno termina com um estado claro para o intervalo seguinte.**
