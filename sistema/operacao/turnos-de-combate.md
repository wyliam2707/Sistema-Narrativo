# Turnos de Combate

Status: APROVADO

Este arquivo define **como o tempo e a ordem de ação são organizados quando existe combate ativo**.

As mecânicas de ataque, Dano, Cura, Mana, Poderes, Status, proteção, contenção e demais resoluções pertencem a `../resolucao/`.

> **Operação organiza o tempo e a ordem. Resolução calcula o resultado.**

## Regra central

Durante combate, a ficção é dividida em **rodadas de até 10 segundos**.

Todos os participantes pertencem ao mesmo intervalo de tempo, mas suas ações são **resolvidas em ordem de Iniciativa**.

```text
RODADA DE COMBATE
→ até 10 segundos
→ seguir a ordem de Iniciativa
→ resolver uma posição por vez
→ atualizar o estado imediatamente
→ depois seguir para a próxima posição
```

A Iniciativa existe para garantir uma ordem operacional clara e impedir que alguma peça seja esquecida durante a resolução.

## Iniciativa

Quando o combate começa, cada participante ativo faz:

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

Essa ordem permanece durante o combate.

### Empate

Em empate de Iniciativa:

```text
maior Controle age primeiro
→ persistindo o empate, somente os empatados rolam novamente
```

### Entrada posterior

Uma peça que entrar no confronto depois do início:

```text
rola Iniciativa
→ entra imediatamente na posição correspondente da ordem
```

A ordem só é refeita por uma regra específica ou quando um novo combate começa.

## Ordem operacional da rodada

No início do combate, o NARRADOR registra a ordem de Iniciativa.

Depois, cada rodada segue essa ordem integralmente:

```text
1. primeiro da Iniciativa
→ declarar intenção
→ configurar Poder, quando aplicável
→ resolver ação e defesas
→ aplicar consequências
→ atualizar estado

2. próximo da Iniciativa
→ repetir o mesmo procedimento

...

último da Iniciativa
→ resolver e atualizar

→ nova rodada, se o combate continuar
```

Cada participante ativo deve receber sua posição antes de a rodada terminar.

> **Não encerrar a rodada enquanto existir participante ativo ainda não processado na ordem de Iniciativa.**

## Janela de ação

A posição de Iniciativa concede uma **janela de ação** dentro daqueles até 10 segundos.

Ela não cria uma economia abstrata universal de “uma ação, uma ação bônus, um movimento”. A personagem declara uma intenção coerente e o sistema julga o que cabe naquela janela conforme a ficção e as regras específicas.

Uma declaração ampla não resolve várias rodadas de uma vez.

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

RODADA ATUAL
→ resolver somente o que cabe na janela atual
```

Se o objetivo continuar, a personagem recebe nova oportunidade quando sua próxima posição de Iniciativa chegar.

## Defesas e reações

Uma Defesa permitida pela ação acontece quando o ataque ou efeito é resolvido.

Ela **não consome a posição de Iniciativa** do defensor e não altera sua posição na rodada.

```text
atacante age
→ alvo realiza Defesa aplicável
→ resolve consequência
→ atualiza estado
→ segue a ordem
```

A defesa automática do JOGADOR HUMANO segue `ordem-de-resolucao-do-combate.md`.

Poderes, reações ou interrupções que possuam regra própria podem ocorrer fora da posição normal somente quando sua regra permitir explicitamente.

## Consequências antes da própria vez

Como o estado é atualizado após cada ação, uma consequência anterior pode alterar uma posição posterior da mesma rodada.

Exemplos:

- ficar Inconsciente;
- ser imobilizado;
- perder acesso a um recurso;
- mudar de posição;
- receber proteção;
- deixar o confronto.

Quando a posição daquela peça chegar, usar o **estado atual**, não o estado que existia no início da rodada.

Se a peça não puder mais agir, sua posição é processada e encerrada sem ação voluntária.

> **Resolveu, atualizou, depois chamou o próximo.**

## Início do combate

O combate começa quando existe confronto ativo em que várias peças podem agir ou se opor em intervalos curtos.

Ao entrar em combate:

```text
identificar participantes ativos
→ rolar Iniciativa
→ ordenar
→ apresentar a ordem
→ iniciar a primeira posição
```

Não é necessário esperar o primeiro Dano.

## Fechamento da rodada

A rodada termina depois que todas as posições de Iniciativa aplicáveis foram processadas.

Antes da nova rodada, o estado deve refletir todas as consequências estabelecidas, incluindo quando pertinente:

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

## Relação com as mecânicas

A Iniciativa determina **quando cada peça age**, não se a ação tem sucesso.

```text
OPERAÇÃO
→ Iniciativa, rodada e sequência

RESOLUÇÃO
→ testes, Defesa, Dano, Cura, Poderes, Status e custos

PERSISTÊNCIA
→ estado resultante
```

## Regra final

> **Combate usa rodadas de até 10 segundos e uma ordem fixa de Iniciativa. Iniciativa = 4d6 + Controle. Resolver cada participante do maior para o menor, aplicar a consequência e atualizar o estado antes de chamar o próximo. Defesas não consomem a posição de Iniciativa.**
