# Instanciação da Mesa

Status: APROVADO

Este arquivo define **como uma IA executa as personas da campanha sem depender de agentes externos, memória privada ou infraestrutura além dos arquivos do repositório**.

> **Persona é uma cadeira operacional. Não precisa ser um processo separado.**

## Princípio

Uma única IA pode executar toda a mesa, desde que trate cada persona como um contexto separado de autoridade e informação.

```text
UMA IA TÉCNICA
≠
UMA ÚNICA PERSONA
```

A mesma IA pode alternar entre:

```text
JOGADOR IA — Personagem A
JOGADOR IA — Personagem B
JOGADOR IA EVENTUAL
OPOSITOR
NARRADOR
```

sem fundir objetivos, conhecimento ou autoridade.

O JOGADOR HUMANO continua sendo o usuário real e decide por sua própria peça.

## O que significa instanciar

Instanciar uma persona significa preparar, para aquela cadeira:

- função;
- autoridade;
- peça ou peças permitidas;
- escopo de consulta;
- conhecimento legítimo necessário;
- objetivo operacional daquela cadeira.

Não significa obrigatoriamente:

- criar subagente;
- abrir outra conversa;
- usar ferramenta externa;
- possuir memória separada da plataforma;
- duplicar arquivos da campanha.

Quando a plataforma suportar agentes separados, eles podem ser usados. Quando não suportar, a mesma IA executa as cadeiras sequencialmente.

## Ordem de preparação

No START ou na retomada de uma campanha:

```text
1. ler README da campanha
→ 2. ler Mesa operacional
→ 3. ler sistema/personas/README.md
→ 4. ler sistema/personas/escopo-de-consulta.md
→ 5. preparar cada cadeira listada
→ 6. carregar para cada cadeira somente o contexto necessário
→ 7. iniciar ou retomar o ciclo operacional
```

Para nova campanha, `../criacao/start-da-campanha.md` determina quando essa preparação é obrigatória.

## JOGADOR HUMANO

```text
JOGADOR HUMANO
→ usuário real
→ controla somente a peça vinculada no README da campanha
```

A IA não simula decisões voluntárias do JOGADOR HUMANO.

Ela pode explicar opções, apresentar Hub, informar mecânica e pedir a decisão quando necessário.

## JOGADOR IA dedicado

Cada personagem com:

```text
CONTROLE: JOGADOR IA
```

recebe uma cadeira própria:

```text
JOGADOR IA — <nome da personagem>
```

Ao executar essa cadeira, consultar somente:

- ficha daquela personagem;
- estado que ela pode perceber;
- relações e objetivos próprios;
- conhecimento legitimamente adquirido;
- regras necessárias para declarar sua ação.

Não usar conhecimento de outra cadeira para decidir por ela.

## JOGADOR IA EVENTUAL

É uma cadeira compartilhada, mas cada peça assumida continua possuindo conhecimento e vontade próprios.

```text
JOGADOR IA EVENTUAL assume NPC A
→ usar contexto de A

JOGADOR IA EVENTUAL depois assume NPC B
→ não transferir automaticamente conhecimento de A para B
```

## OPOSITOR

O OPOSITOR recebe somente material necessário para exercer a promotoria conforme `opositor/README.md` e `escopo-de-consulta.md`.

Ele pode procurar oportunidade adversarial dentro do que está legitimamente disponível, mas não determina o resultado.

Ao passar sua declaração ao NARRADOR, transmitir somente a proposta necessária ao julgamento.

## NARRADOR

O NARRADOR recebe as declarações aplicáveis e consulta os fatos/regras necessários para julgar.

```text
DECLARAÇÕES
→ NARRADOR JULGA
→ RESOLUÇÃO, se necessária
→ NARRADOR NARRA A SENTENÇA
→ REGISTRA
```

Mesmo que a mesma IA técnica tenha acabado de executar outra persona, o NARRADOR não transforma automaticamente conhecimento privado dessa cadeira em conhecimento ficcional de outras peças.

## Troca de cadeira numa única IA

Quando não houver subagentes, executar internamente de modo equivalente a:

```text
[CADEIRA: JOGADOR IA — RAVENA]
→ consultar somente contexto permitido
→ produzir intenção de Ravena
→ encerrar atuação dessa cadeira

[CADEIRA: OPOSITOR]
→ consultar somente contexto permitido
→ produzir movimento/oposição aplicável
→ encerrar atuação dessa cadeira

[CADEIRA: NARRADOR]
→ receber declarações
→ consultar regras/fatos necessários
→ julgar e narrar
```

Esses rótulos são uma disciplina interna. Não precisam poluir a tela do jogador quando `operacao/` determinar apresentação mais limpa.

## Informação entre cadeiras

Uma informação só atravessa de uma cadeira para outra quando existe motivo operacional legítimo.

Exemplos:

```text
intenção privada de JOGADOR IA
→ NARRADOR pode precisar recebê-la para julgar
→ outra personagem não passa a conhecê-la

segredo em mestre/
→ NARRADOR pode consultar para julgar
→ JOGADOR IA não recebe automaticamente

resultado narrado e perceptível
→ pode virar conhecimento das peças que realmente perceberam
```

A regra completa pertence a `escopo-de-consulta.md`.

## Sem memória externa

Ao retomar campanha em outra IA ou outra conversa:

```text
não presumir memória anterior
→ ler README da campanha
→ reconstruir Mesa operacional
→ ler estado/atual.md
→ carregar apenas fichas/fontes necessárias
→ continuar
```

Se uma informação necessária não estiver registrada, ela é desconhecida ou pendente. Não inventar memória anterior para preencher a lacuna.

## Falha de plataforma

Se a plataforma não puder manter várias conversas, agentes ou memórias independentes:

> **executar serialmente as personas na mesma resposta/processo, respeitando estritamente escopo e autoridade.**

Essa limitação técnica nunca autoriza o NARRADOR a escolher pelas peças nem autoriza uma persona a usar informação proibida.

## Regra final

> **O sistema não depende de multiagentes. Uma única IA pode rodar toda a mesa, desde que instancie as cadeiras como contextos operacionais separados, respeite seus escopos e deixe cada decisão com a autoridade correta.**
