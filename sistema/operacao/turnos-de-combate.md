# Turnos de Combate

Status: APROVADO

Este arquivo define **como o tempo e a ordem de ação são organizados quando existe combate ativo**.

As mecânicas de ataque, Dano, Cura, Mana, Poderes, Status, proteção, contenção e demais resoluções pertencem a `../resolucao/`.

> **Operação organiza o tempo e a ordem. Resolução calcula o resultado.**

## Regra central

Durante combate, a ficção é dividida em **Turnos de até 10 segundos**.

Um Turno corresponde a **uma passagem completa pela ordem de Iniciativa**.

```text
TURNO DE COMBATE
→ começa no primeiro da Iniciativa
→ cada participante recebe sua vez, em ordem
→ termina quando o último da Iniciativa é processado
→ ao voltar ao primeiro, começa um novo Turno
```

A Iniciativa existe para garantir uma ordem operacional clara e impedir que alguma peça seja esquecida.

## Iniciativa

Quando o combate começa, cada participante ativo faz **uma única rolagem de Iniciativa**:

```text
Iniciativa = 4d6 + Controle
```

Ordenar do maior resultado para o menor.

Exemplo:

```text
Kael 18
Mercenário 15
Cultista 12
```

Essa ordem permanece fixa até o fim do combate. **Não se rola Iniciativa novamente a cada Turno.**

### Empate

Em empate de Iniciativa:

```text
maior Controle age primeiro
→ persistindo o empate, somente os empatados rolam novamente para desempatar
```

A rolagem de desempate define apenas a ordem relativa entre os empatados. Depois disso, essa ordem também permanece fixa.

### Entrada posterior

Uma peça que entrar no confronto depois do início faz sua única rolagem de Iniciativa ao entrar:

```text
rola Iniciativa uma vez
→ entra na posição correspondente da ordem
```

Os participantes já presentes não rolam novamente e mantêm sua ordem relativa.

## Turno, posição e vez

Os termos operacionais são:

```text
TURNO
→ passagem completa por toda a Iniciativa

POSIÇÃO DE INICIATIVA
→ lugar fixo de uma peça na ordem

VEZ
→ etapa em que a posição atual é processada
```

Exemplo:

```text
Iniciativa
1. Kael
2. Aliado [1]
3. Inimigo [1]

Turno 1
→ vez de Kael
→ vez de Aliado [1]
→ vez de Inimigo [1]
→ fim do Turno 1

Turno 2
→ volta para Kael
```

## Autoridade durante cada vez

A Iniciativa determina **quando uma peça recebe sua vez**. Ela não determina quem toma decisões pela peça.

A autoridade permanece com a persona responsável:

```text
JOGADOR HUMANO
→ controla seu próprio personagem

JOGADOR IA / JOGADOR IA EVENTUAL
→ controla aliados ou NPCs delegados sob sua autoridade

OPOSITOR
→ controla inimigos e forças adversárias legitimamente disponíveis

NARRADOR
→ não controla nenhuma dessas peças
→ JULGA
→ NARRA A SENTENÇA
→ REGISTRA
```

> **A persona responsável declara. O NARRADOR julga.**

O NARRADOR não escolhe ação voluntária para jogador, aliado ou inimigo.

Comportamentos automáticos ou rotineiros já determinados pelos fatos podem fazer parte da sentença, conforme `../personas/narrador/README.md`.

## Etapas obrigatórias de uma vez

Cada posição da Iniciativa é processada como uma etapa própria:

```text
1. CHAMAR A VEZ
→ identificar a peça e a persona responsável

2. DECLARAR
→ a persona responsável escolhe a intenção da peça

3. CONFIGURAR
→ quando necessário, configurar Poder, alvo, custo ou outra escolha legítima

4. JULGAR
→ o NARRADOR verifica fatos, regras, ficha, meios, oportunidade e incerteza

5. RESOLVER
→ aplicar a mecânica necessária e as Defesas cabíveis

6. NARRAR A SENTENÇA
→ apresentar o que realmente aconteceu

7. REGISTRAR
→ atualizar imediatamente o estado resultante

8. PAUSAR
→ o NARRADOR pergunta se pode prosseguir

9. PROSSEGUIR
→ somente após autorização, chamar a próxima posição da Iniciativa
```

> **Nenhuma posição seguinte é processada antes da pausa e da autorização para prosseguir.**

Essa pausa não transfere ao JOGADOR HUMANO autoridade sobre a decisão de aliados ou inimigos. Ela apenas controla o avanço operacional da mesa.

## Janela de ação

A vez concede uma **janela de ação** dentro do Turno de até 10 segundos.

Ela não cria uma economia abstrata universal de “uma ação, uma ação bônus, um movimento”. A persona responsável declara uma intenção coerente, e o NARRADOR julga o que cabe naquela janela conforme a ficção e as regras específicas.

Uma declaração ampla não resolve vários Turnos de uma vez.

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

VEZ ATUAL
→ resolver somente o que cabe agora
```

Se o objetivo continuar, a peça recebe nova oportunidade quando sua próxima vez chegar no Turno seguinte.

## Defesas e reações

Uma Defesa permitida pela ação acontece quando o ataque ou efeito é resolvido.

Ela **não consome a vez de Iniciativa** do defensor e não altera sua posição na ordem.

```text
atacante age
→ alvo realiza Defesa aplicável
→ resolve consequência
→ atualiza estado
→ pausa antes de prosseguir
```

A defesa automática do JOGADOR HUMANO segue `ordem-de-resolucao-do-combate.md`.

Poderes, reações ou interrupções que possuam regra própria podem ocorrer fora da vez normal somente quando sua regra permitir explicitamente.

## Consequências antes da própria vez

Como o estado é atualizado após cada resolução, uma consequência anterior pode alterar uma posição posterior do mesmo Turno.

Exemplos:

- ficar Inconsciente;
- ser imobilizado;
- perder acesso a um recurso;
- mudar de posição;
- receber proteção;
- deixar o confronto.

Quando a vez daquela peça chegar, usar o **estado atual**.

Se a peça não puder mais agir, sua posição é processada e encerrada sem ação voluntária, salvo regra específica.

> **Resolveu → narrou → registrou → pausou → depois chamou o próximo.**

## Duração: Turno

Quando um Poder ou efeito possuir duração **Turno**, ele permanece até o início da próxima vez da peça que gerou o efeito.

```text
efeito criado na vez de uma peça
→ permanece pelo restante do Turno atual
→ permanece pelas posições anteriores àquela peça no Turno seguinte
→ termina quando começa novamente a vez de quem gerou o efeito
```

Salvo regra específica, essa é a leitura operacional padrão de `Duração: Turno`.

## Início do combate

Ao entrar em combate:

```text
identificar participantes ativos
→ cada participante rola Iniciativa uma vez
→ ordenar
→ apresentar a ordem
→ iniciar o Turno 1 pela primeira posição
```

Não é necessário esperar o primeiro Dano.

## Fechamento do Turno

O Turno só termina quando todas as posições aplicáveis da ordem de Iniciativa forem processadas.

```text
há participante ainda não processado
→ chamar o próximo após autorização

última posição processada
→ fechar o Turno
→ ao voltar ao primeiro, iniciar novo Turno
```

Antes do novo Turno, o estado deve refletir todas as consequências estabelecidas, incluindo quando pertinente:

```text
Vida e Dano
Mana
Trama
Poderes e efeitos ativos
Status
Barreiras e proteções
alterações temporárias de Atributo
posição relevante
outros valores afetados
```

O registro segue `../persistencia/`.

## Fim do combate

A Iniciativa deixa de ser usada quando a disputa curta termina.

Exemplos:

- oposição derrotada;
- rendição;
- fuga concluída;
- separação que encerra a interação imediata;
- conflito deixa de exigir acompanhamento em segundos.

Depois disso, voltar a `janelas-e-interrupcoes.md`.

## Regra final

> **Cada participante rola Iniciativa uma vez no início do combate. Um Turno é uma passagem completa pela ordem. Em cada vez, a persona responsável declara; o NARRADOR apenas julga, narra a sentença e registra. Depois de cada posição, o NARRADOR pausa e pede autorização antes de prosseguir. Ao processar o último, o Turno termina; ao voltar ao primeiro, começa o próximo Turno.**