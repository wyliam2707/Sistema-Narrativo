# Registro Reservado do Opositor

Status: REFORMULAÇÃO / NÃO IMPLEMENTADO

Este arquivo define como preservar o lado adversarial da trama fora do conhecimento dos jogadores.

O Registro Reservado é compartilhado operacionalmente entre `OPOSITOR` e `NARRADOR`.

Ele existe para que planos, prazos e processos de antagonistas continuem verdadeiros sem depender da memória da IA.

## O que pode ser registrado

Podem ser preservados:

- planos de vilões;
- objetivos adversariais;
- alvos;
- preparação em andamento;
- recursos legitimamente disponíveis;
- conhecimento de cada força;
- prazos;
- gatilhos;
- estágios de execução;
- deslocamentos;
- ataques planejados;
- sequestros planejados;
- armadilhas;
- consequências futuras já estabelecidas;
- outros processos internos do lado adversarial.

## Como um plano entra no Registro

O Opositor declara a intenção do lado adversarial.

```text
OPOSITOR
→ Vilão X começa a preparar um ataque para daqui a 5 dias.
```

O Narrador julga:

```text
possui fundamento?
possui conhecimento?
possui meios?
possui tempo?
possui oportunidade?
```

Se o plano for válido, o Narrador estabelece o processo e o prazo aplicáveis.

Somente então ele passa a ser verdade registrada.

```text
DECLARAÇÃO DO OPOSITOR
→ NARRADOR julga
→ processo adversarial estabelecido
→ REGISTRO RESERVADO preserva
```

## Exemplo

```text
VILÃO X
Plano: atacar a base dos Titãs
Estado: preparação em andamento
Prazo: ataque em 5 dias
Recursos: [somente os já estabelecidos]
Conhecimento: [somente o que o vilão realmente sabe]

VILÃO Y
Plano: sequestrar Fulano
Estado: preparação em andamento
Prazo: tentativa em 3 dias
```

## Plano não é sucesso

Registrar um plano significa apenas que ele existe e está em andamento.

Não significa que será concluído com sucesso.

O plano pode ser:

- descoberto;
- atrasado;
- interrompido;
- alterado;
- impedido;
- abandonado;
- derrotado por outra ação legítima.

Quando isso acontecer, o Registro deve ser atualizado para refletir o estado real.

## Passagem do tempo

Um processo adversarial registrado pode continuar fora da cena principal sem precisar ser redeclarado em todas as janelas.

O Opositor volta a agir quando:

- chega uma etapa do plano;
- o prazo vence;
- surge nova decisão adversarial;
- a situação muda;
- aparece nova oportunidade;
- uma força adversarial entra em campo.

## Fiscalização

O Opositor deve usar este Registro para impedir que planos e prazos internos sejam esquecidos.

```text
REGISTRO RESERVADO
→ ataque começa hoje.

OPOSITOR
→ traz o prazo para a janela.

NARRADOR
→ verifica o Registro.
→ reconhece a entrada do evento.
```

A fiscalização não cria nem antecipa o fato.

## Conhecimento compartimentado

O Opositor pode conhecer todo o material reservado necessário para administrar o lado adversarial.

Esse conhecimento não pertence automaticamente a cada vilão ou NPC.

```text
OPOSITOR SABE
≠
VILÃO SABE
```

Cada peça adversarial só pode agir com o conhecimento que ela própria possui legitimamente.

O Registro deve manter essa distinção quando ela for relevante.

## Sigilo

O conteúdo deste Registro não é fonte de decisão para Jogador Humano, Jogador IA ou Jogador IA Eventual enquanto não for descoberto legitimamente na ficção.

Se uma informação reservada for descoberta, o Narrador pode transferir o fato correspondente para o Registro apropriado da personagem que o descobriu.

## Regra final

> **O Registro Reservado do Opositor preserva o outro lado da trama: planos, processos, prazos e conhecimento adversarial já julgados como válidos. Ele mantém continuidade sem transformar plano em sucesso automático e sem transferir conhecimento secreto para personagens que não o possuem.**