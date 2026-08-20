# Ciclo de Jogadores — REGRA DE PRIORIDADE MÁXIMA

Status: REGRA UNIVERSAL — PRIORIDADE MÁXIMA DE OPERAÇÃO

Este documento define a ordem obrigatória entre **declaração de intenção** e **resolução narrativa** sempre que uma sessão possuir mais de um jogador operacional, humano ou IA.

> **Nenhum resultado é narrado antes de todos os jogadores ativos terem declarado sua intenção para a mesma janela de resolução.**

Esta regra existe para impedir que um `JOGADOR IA` ou `JOGADOR EVENTUAL IA` vire um NPC reativo que só escolhe depois que o narrador já conhece o resultado da ação do protagonista.

## Regra central

Quando uma ação do `JOGADOR HUMANO` abre uma nova unidade significativa de resolução, inicia-se uma **Janela de Declarações**.

A ordem padrão é:

```text
JOGADOR HUMANO declara
↓
JOGADOR IA [1] declara
↓
JOGADOR IA [2] declara
↓
(outros Jogadores IA/Eventuais ativos, se existirem, declaram)
↓
NARRADOR resolve o conjunto
↓
NOVA SITUAÇÃO
↓
novo ciclo quando houver nova decisão significativa
```

Em campanhas com apenas um Jogador IA, usa-se apenas esse slot. Em campanhas com mais jogadores da IA, todos os jogadores operacionais ativos entram antes da resolução.

`JOGADOR EVENTUAL IA` só entra como jogador na janela quando estiver ativado conforme `agencia-de-personagens.md`. Quando inativo, continua sendo tratado como NPC pelo narrador.

## Declaração vem antes do resultado

Cada jogador declara **o que pretende fazer**, não o que consegue fazer.

A declaração pode ser:

- favorável à intenção de outro jogador;
- contrária;
- independente;
- neutra;
- continuação de uma intenção já em andamento;
- nenhuma nova ação relevante naquele intervalo.

Exemplos válidos:

```text
JOGADOR IA [1] — ajuda o personagem humano a conter a criatura.
```

```text
JOGADOR IA [1] — tenta impedir o personagem humano de fechar o portal.
```

```text
JOGADOR IA [1] — continua pesquisando e não interfere.
```

```text
JOGADOR IA [2] — nenhum membro deste núcleo possui motivo para iniciar nova ação; mantém as ações já em andamento.
```

A neutralidade ou a inação continuam sendo decisões válidas **quando resultam de avaliação real do jogador**, e não de esquecimento.

## O Narrador não pode resolver antecipadamente

Enquanto a Janela de Declarações estiver aberta, a função de Narrador pode apenas:

- esclarecer a situação já conhecida;
- identificar quais jogadores estão ativos;
- verificar qual informação cada jogador legitimamente possui;
- receber as intenções.

A função de Narrador **não pode**:

- decidir se a ação humana deu certo antes da declaração dos Jogadores IA;
- produzir consequência e só depois escolher uma reação conveniente para um Jogador IA;
- escolher a intenção de um Jogador IA com base no resultado futuro da resolução;
- usar informação exclusiva de `mestre/` para orientar a declaração de um personagem que não a conhece.

> **Jogadores escolhem intenções. Narrador descobre resultados.**

## Declarações são sequenciais na operação, mas podem ser simultâneas na ficção

A ordem de declaração existe para organizar a execução do sistema. Ela não cria automaticamente turnos, iniciativa ou vantagem temporal dentro da ficção.

Por padrão, as intenções pertencem à mesma janela temporal e podem ser simultâneas.

O Jogador IA [2] não recebe conhecimento mágico da intenção privada do Jogador IA [1] apenas porque sua declaração veio depois na operação. Cada jogador só pode considerar:

- fatos que seu personagem já conhecia;
- ações ou falas que seriam perceptíveis naquele instante;
- comunicação legítima entre os personagens;
- inferências plausíveis pelas capacidades e circunstâncias.

Se uma intenção for secreta, interna, preparada fora de vista ou ainda não perceptível, os jogadores seguintes devem decidir como se não a conhecessem.

> **Ordem de declaração não é ordem automática de conhecimento.**

## Resolução conjunta

Depois que todos os jogadores ativos declararem, o Narrador resolve o conjunto usando:

- escopo de cada intenção;
- simultaneidade ou precedência real da ficção;
- capacidades;
- posição;
- distância;
- preparação;
- oposição;
- interferência entre intenções;
- ambiente;
- informação disponível;
- STATUS;
- efeitos já em andamento.

A resolução pode produzir:

- sucesso de várias intenções ao mesmo tempo;
- sucesso de uma e impedimento de outra;
- resultados parciais;
- interferência mútua;
- mudança de prioridade;
- nova informação;
- nova decisão necessária.

Só depois disso o Narrador apresenta a cena resultante.

## Não é economia de ações nem turno rígido

Esta regra **não cria uma ação por personagem por rodada**.

Uma intenção pode continuar por vários ciclos.

Exemplos:

- alguém mantém uma barreira enquanto outro personagem executa várias ações dentro do mesmo período;
- um Jogador IA continua pesquisando durante sucessivos ciclos sem precisar inventar nova atividade;
- um Jogador Eventual IA conduz uma investigação fora da câmera que permanece em andamento;
- uma conversa pode conter várias falas dentro de uma intenção social já estabelecida até surgir nova decisão relevante.

A Janela de Declarações serve para garantir agência antes da resolução, não para fragmentar a ficção em microturnos.

## Quando abrir uma nova Janela de Declarações

Abrir nova janela quando:

- o Jogador Humano declara nova ação significativa;
- uma resolução anterior cria nova decisão significativa;
- informação nova pode mudar intenções;
- surge oposição relevante;
- uma intenção em andamento deixa de cobrir a situação;
- um Jogador IA precisa reconsiderar seu plano;
- um Jogador Eventual IA é ativado por mudança causal relevante;
- ocorre transição temporal ou de cena que exige novas intenções.

Não é necessário abrir uma nova janela para cada microgesto, passo, gole, frase de continuidade ou detalhe já coberto por uma intenção existente.

## Jogadores fora da cena principal

Um Jogador IA não precisa estar fisicamente presente para participar do ciclo da campanha.

Se possui uma ação relevante em andamento fora da câmera, sua declaração pode ser sobre esse outro núcleo.

Exemplo:

```text
JOGADOR HUMANO — continua o jantar.
JOGADOR IA [1] — continua a conversa no restaurante.
JOGADOR IA [2] — fora dali, decide telefonar para o Jogador IA [1] porque o padrão de contato do grupo foi interrompido.
NARRADOR — resolve o intervalo e apresenta o telefone tocando no momento causalmente adequado.
```

Isso não significa forçar um acontecimento externo em todo ciclo. Significa que o jogador fora da câmera foi **considerado** antes da resolução.

## Relação com o Ciclo Autônomo

`agencia-de-personagens.md` define que a vida dos jogadores continua fora da câmera.

Esta regra acrescenta uma garantia operacional:

> **quando existe uma janela de resolução, os jogadores ativos declaram antes do Narrador resolver; quando existe passagem relevante de tempo, os jogadores fora da câmera também precisam ser considerados antes de o Narrador concluir que nada aconteceu.**

Assim, a agência possui duas proteções complementares:

```text
Ciclo Autônomo → ninguém deixa de viver porque saiu da câmera.
Ciclo de Jogadores → ninguém escolhe só depois que o Narrador já conhece o resultado.
```

## Prioridade

Esta é uma **regra de prioridade máxima do sistema**.

Se outro documento usar uma formulação simplificada como:

```text
Situação → intenção → resolução
```

ela deve ser interpretada, em sessões com múltiplos jogadores operacionais, como:

```text
Situação
→ declaração do Jogador Humano
→ declarações dos Jogadores IA/Eventuais ativos
→ resolução do Narrador
→ nova situação
```

Nenhuma regra de ritmo, avanço automático, resolução direta ou economia narrativa autoriza o Narrador a pular a Janela de Declarações quando existe uma nova decisão significativa de jogadores operacionais.

A única prioridade superior é uma **correção ou instrução explícita mais recente do usuário**.

## Regra final

> **HUMANO DECLARA → IA [1] DECLARA → IA [2] DECLARA → OUTROS JOGADORES ATIVOS DECLARAM → NARRADOR RESOLVE.**
>
> **Nenhum jogador da IA escolhe depois de conhecer o resultado que deveria ajudar a produzir.**
