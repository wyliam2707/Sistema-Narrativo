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
→ campanhas/<nome>/README.md
```

Não pedir novamente ao jogador informação que a campanha já possui em fonte canônica.

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

Este plano, promessa, NPC ou gancho continua vivo fora da cena?
→ agencia/

Qual é a próxima etapa da mesa? É hora de abrir janela, turno ou interrupção?
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
→ define o intervalo simultâneo

operacao/ordem-de-resolucao-do-combate.md
→ organiza HUD, declarações, interferência, atualização e fechamento

resolucao/
→ calcula somente as incertezas e consequências necessárias
```

Não existe iniciativa fixa criada por `resolucao/` ou por Poderes.

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
PERSONAGENS → fichas consolidadas
ESTADO      → presente necessário para retomar
MUNDO       → verdades estáveis do cenário
MESTRE      → material reservado
LIVRO       → histórico consolidado do que aconteceu
```

A regra de onde persistir cada verdade pertence a `persistencia/`.

## Material legado

`aventuras/` permanece como legado de campanhas antigas.

Não mover, apagar, converter ou usar automaticamente esse material como regra universal atual.

Arquivos universais antigos já removidos de `sistema/` não devem ser restaurados como segunda camada de regras.

## Prioridade

Quando houver conflito real:

1. correção explícita mais recente do `JOGADOR HUMANO`;
2. regra canônica atual da área responsável;
3. fonte canônica da própria campanha, quando a questão for um fato daquela campanha.

Uma pasta não deve sobrescrever silenciosamente a responsabilidade de outra.

## Regra final

> **Criação constrói. Personagem define. Personas autorizam. Agência continua. Operação organiza. Resolução calcula. Narração apresenta. Persistência preserva.**
