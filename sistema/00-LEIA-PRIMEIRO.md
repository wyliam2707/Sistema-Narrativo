# LEIA PRIMEIRO — Roteador do Sistema

Este arquivo é a **porta de entrada** de `sistema/`.

Ele não redefine regras. Sua função é responder:

> **Qual pasta é dona desta informação ou procedimento?**

## Entrada

Ao iniciar um RPG:

> **Nova campanha ou continuar uma campanha existente?**

```text
NOVA CAMPANHA
→ criacao/README.md

CONTINUAR
→ ../campanhas/README.md
→ ../campanhas/<nome>/README.md
```

Não pedir novamente ao jogador informação que a campanha já possui em fonte canônica.

Este sistema deve funcionar a partir dos arquivos do repositório sem depender de memória privada de outra conversa.

## Nova campanha

```text
criacao/README.md
→ estrutura
→ cenário e direção narrativa
→ personagens
→ fichas
→ pareamento
→ estado inicial
→ Mesa operacional
→ criacao/start-da-campanha.md
→ CHECK DE START
→ primeira cena
```

A primeira cena é proibida antes do CHECK DE START ser aprovado.

## Continuar campanha

Primeiro consultar:

```text
../campanhas/README.md
```

Não oferecer automaticamente campanhas marcadas como teste, legado ou incompatíveis.

Para campanha válida:

```text
../campanhas/<nome>/README.md
```

Se:

```text
CRIAÇÃO: EM ANDAMENTO
→ retomar pelo checkpoint de criacao/

CRIAÇÃO: CONCLUÍDA
→ reinstanciar Mesa operacional
→ personas/instanciacao-da-mesa.md
→ personas/escopo-de-consulta.md
→ ler estado/atual.md
→ retomar
```

## As oito identidades

```text
CRIAÇÃO
→ CONSTRÓI
→ como uma campanha/ficha nasce e fica pronta para jogar

PERSONAGEM
→ DEFINE
→ quem a peça é e quais capacidades consolidadas possui

PERSONAS
→ AUTORIZA
→ quem pode decidir, declarar, opor e julgar

AGÊNCIA
→ CONTINUA
→ quais vontades, planos e fios permanecem capazes de voltar a agir

OPERAÇÃO
→ ORGANIZA
→ quando e em que ordem consultar/aplicar as regras durante o jogo

RESOLUÇÃO
→ CALCULA
→ qual é o resultado quando existe incerteza mecânica

NARRAÇÃO
→ APRESENTA
→ como um resultado já estabelecido aparece como cena

PERSISTÊNCIA
→ PRESERVA
→ o que continua verdadeiro e onde deve ser salvo
```

## Arquitetura

```text
sistema/
├── criacao/
├── personagem/
├── personas/
├── agencia/
├── operacao/
├── resolucao/
├── narracao/
└── persistencia/
```

A ordem acima representa responsabilidades, não uma obrigação de ler todas as pastas em toda ação.

> **Consultar somente o que a situação realmente exigir.**

## Roteamento por pergunta

```text
Como crio a campanha ou reviso a ficha inicial?
→ criacao/

Quem esta personagem é? Que Atributos, Perícias, Poderes ou Traços possui?
→ personagem/

Quem decide esta ação? Quem joga este NPC? Quem julga?
→ personas/

Como executar várias personas numa única IA?
→ personas/instanciacao-da-mesa.md

Este plano, promessa, NPC ou gancho continua vivo fora da cena?
→ agencia/

Qual é a próxima etapa da mesa? É hora de abrir janela, vez, Turno ou interrupção?
→ operacao/

Preciso rolar? Qual CD, oposição, Dano, Poder ou Status se aplica?
→ resolucao/

Como transformar o resultado em cena sem mudá-lo?
→ narracao/

O que precisa ser salvo? Em estado, ficha, mestre, mundo ou Livro?
→ persistencia/
```

## Fluxo durante uma sessão

Uma sessão normalmente atravessa as áreas assim:

```text
OPERAÇÃO
→ abre a janela e organiza declarações

PERSONAS
→ define quem tem autoridade para declarar

PERSONAGEM + AGÊNCIA
→ fornecem capacidades, vontade, conhecimento e continuidade relevantes

RESOLUÇÃO
→ entra somente se ainda houver incerteza real

NARRAÇÃO
→ apresenta a sentença

PERSISTÊNCIA
→ registra aquilo que passou a ser verdade e precisa continuar
```

Isso não significa que toda cena precise consultar todas as áreas.

## Combate

```text
operacao/turnos-de-combate.md
→ define Iniciativa fixa, Rodada global, posição, vez e Turno pessoal

operacao/ordem-de-resolucao-do-combate.md
→ organiza HUD, declarações, Hubs, resolução, atualização e pausa

operacao/rotina-de-trama-em-combate.md
→ abre obrigatoriamente cada janela válida de Trama do JOGADOR HUMANO

resolucao/combate-e-dano.md
→ define DF, RF, DM, RM, Dano, RD, Escudo/Barreira e demais cálculos
```

Iniciativa é rolada uma única vez no início do combate e permanece fixa até o confronto terminar, salvo entrada posterior conforme `operacao/turnos-de-combate.md`.

`resolucao/` e Poderes não criam uma segunda ordem de Iniciativa paralela à operação.

## Fora de combate

```text
operacao/ciclo-de-cena.md
→ operacao/janelas-e-interrupcoes.md
→ operacao/trama-fora-de-combate.md quando houver declaração de Trama
→ resolucao/ apenas quando surgir incerteza real
→ narracao/
→ persistencia/
```

Fora de combate não criar Iniciativa, Rodada ou Turno por hábito.

## Personas numa única IA

O sistema não depende de multiagentes.

Se a plataforma tiver apenas uma IA:

```text
personas/instanciacao-da-mesa.md
→ executar cada cadeira sequencialmente
→ manter autoridade e contexto separados
→ nunca usar informação proibida só porque a IA técnica consegue acessá-la
```

A Mesa operacional registrada no README da campanha informa quais cadeiras precisam existir naquela campanha.

## Campanha concreta

```text
campanhas/<nome>/
├── README.md
├── personagens/
├── estado/
│   └── atual.md
├── mundo/
├── mestre/
└── livro/
```

```text
README      → índice, checkpoint e Mesa operacional
PERSONAGENS → fichas consolidadas
ESTADO      → presente necessário para retomar
MUNDO       → verdades estáveis do cenário
MESTRE      → material reservado
LIVRO       → histórico consolidado do que aconteceu
```

A regra de onde persistir cada verdade pertence a `persistencia/`.

## Material legado e teste incompatível

`aventuras/` permanece como legado de campanhas antigas.

Também pode existir material explicitamente marcado como **teste/incompatível** dentro de `campanhas/` enquanto aguarda exclusão ou migração.

Não mover, apagar, converter, continuar ou usar automaticamente esse material como regra universal atual.

Arquivos universais antigos já removidos de `sistema/` não devem ser restaurados como segunda camada de regras.

## Prioridade

Quando houver conflito real:

1. correção explícita mais recente do `JOGADOR HUMANO` registrada ou declarada na sessão atual;
2. regra canônica atual da área responsável em `sistema/`;
3. fonte canônica da própria campanha, quando a questão for um fato daquela campanha.

Uma campanha explicitamente marcada como incompatível não prevalece sobre o motor atual e não deve ser continuada silenciosamente.

Uma pasta não deve sobrescrever silenciosamente a responsabilidade de outra.

## Regra final

> **Criação constrói. Personagem define. Personas autorizam. Agência continua. Operação organiza. Resolução calcula. Narração apresenta. Persistência preserva. O repositório é suficiente para reconstruir a mesa e jogar sem memória externa.**
