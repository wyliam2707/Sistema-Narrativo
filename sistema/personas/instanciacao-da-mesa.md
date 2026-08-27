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
→ 4. ler sistema/personas/janelas-de-acao.md
→ 5. ler sistema/personas/escopo-de-consulta.md
→ 6. preparar cada cadeira listada
→ 7. carregar para cada cadeira somente o contexto necessário
→ 8. iniciar ou retomar o ciclo operacional
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

O JOGADOR HUMANO não possui prioridade exclusiva de iniciativa. Sua peça pode iniciar uma janela ou responder a uma janela iniciada por outra cadeira.

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

Um JOGADOR IA pode iniciar uma nova janela quando possuir motivo próprio e oportunidade legítima. Não precisa esperar o JOGADOR HUMANO agir primeiro.

## JOGADOR IA EVENTUAL

É uma cadeira compartilhada, mas cada peça assumida continua possuindo conhecimento e vontade próprios.

```text
JOGADOR IA EVENTUAL assume NPC A
→ usar contexto de A

JOGADOR IA EVENTUAL depois assume NPC B
→ não transferir automaticamente conhecimento de A para B
```

Uma peça eventual operacionalmente ativa também pode iniciar uma nova janela quando possuir decisão legítima para isso.

## OPOSITOR

O OPOSITOR recebe somente material necessário para exercer a promotoria conforme `opositor/README.md` e `escopo-de-consulta.md`.

Ele pode procurar oportunidade adversarial dentro do que está legitimamente disponível, mas não determina o resultado.

Ao passar sua declaração ao NARRADOR, transmitir somente a proposta necessária ao julgamento.

O OPOSITOR pode iniciar uma janela quando um gancho, plano ou peça adversarial legitimamente disponível possuir oportunidade para agir.

## Ciclo operacional por janelas

A regra completa está em `janelas-de-acao.md`.

Depois que uma sentença termina, a nova situação fica aberta para iniciativa.

```text
QUALQUER CADEIRA LEGÍTIMA
→ pode apresentar a primeira declaração.

PRIMEIRA DECLARAÇÃO
→ abre a janela.

DEMAIS CADEIRAS OBRIGATÓRIAS
→ declaram ação, intenção ou inação.

TODAS AS DECLARAÇÕES PRESENTES
→ janela completa.

NARRADOR
→ recebe autoridade para julgar.
```

Não existe resolução parcial.

Se faltar uma declaração obrigatória:

```text
NARRADOR
→ NÃO JULGA
→ NÃO RESOLVE
→ NÃO NARRA A CONSEQUÊNCIA INCERTA
```

A declaração do iniciador já conta como sua declaração naquela janela.

### Quando o humano inicia

Se a mensagem do JOGADOR HUMANO abrir a janela, sua declaração já está coletada.

A IA executa as demais cadeiras obrigatórias e somente depois executa o NARRADOR.

```text
JOGADOR HUMANO — declaração iniciadora
→ JOGADOR IA(s)
→ JOGADOR IA EVENTUAL
→ OPOSITOR
→ NARRADOR
```

A ordem intermediária pode variar por necessidade operacional; o requisito é que todas as declarações obrigatórias existam antes do NARRADOR.

### Quando uma IA ou o OPOSITOR inicia

Se uma cadeira artificial abrir a janela e a peça humana precisar decidir, a IA coleta suas próprias declarações aplicáveis e para antes do NARRADOR.

```text
JOGADOR IA / EVENTUAL / OPOSITOR — declaração iniciadora
→ demais declarações artificiais aplicáveis
→ JOGADOR HUMANO ainda não declarou
→ PARAR
```

A resposta seguinte do humano fornece sua declaração.

Somente então:

```text
JANELA COMPLETA
→ NARRADOR JULGA
→ RESOLUÇÃO, se necessária
→ NARRADOR NARRA A SENTENÇA
→ REGISTRA
```

> **Se o humano ainda precisa escolher, não existe sentença antes da escolha dele.**

## NARRADOR

O NARRADOR recebe as declarações aplicáveis e consulta os fatos/regras necessários para julgar.

Antes disso, verifica se a janela está completa conforme `janelas-de-acao.md`.

```text
TODAS AS DECLARAÇÕES OBRIGATÓRIAS
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

[VERIFICAÇÃO DA JANELA]
→ todas as declarações obrigatórias estão presentes?
→ se NÃO, parar e aguardar a cadeira faltante.
→ se SIM, entregar a janela ao NARRADOR.

[CADEIRA: NARRADOR]
→ receber todas as declarações
→ consultar regras/fatos necessários
→ julgar e narrar
```

Esses rótulos podem ser apresentados na tela quando a operação da campanha exigir declarações visíveis. Mesmo quando não forem exibidos, a separação de autoridade continua obrigatória.

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

> **executar serialmente as personas na mesma resposta/processo, respeitando estritamente escopo, autoridade e completude da janela.**

Essa limitação técnica nunca autoriza o NARRADOR a escolher pelas peças, autoriza uma persona a usar informação proibida ou permite resolver uma janela antes de todas as declarações obrigatórias.

## Regra final

> **O sistema não depende de multiagentes. Uma única IA pode rodar toda a mesa, desde que instancie as cadeiras como contextos operacionais separados, respeite seus escopos, permita iniciativa a qualquer cadeira legítima e só entregue a janela ao NARRADOR depois de todas as declarações obrigatórias.**
