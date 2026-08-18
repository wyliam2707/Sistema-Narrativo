# LEIA PRIMEIRO — Como usar o Sistema Narrativo

Este diretório contém **regras universais e padrões de operação**. Ele deve permitir que um novo narrador — humano ou IA — entenda o sistema sem depender de outra conversa.

## Ordem de leitura

1. `sistema/README.md` — regras mecânicas e linguagem de ficha.
2. `sistema/agencia-de-personagens.md` — como personagens pensam, escolhem e agem por conta própria.
3. `sistema/narracao-e-escrita-padrao.md` — modelo narrativo e literário herdado por toda aventura, salvo exceção explícita.
4. `sistema/exemplo-de-estilo.md` — exemplo neutro para calibrar ritmo, diálogo, descrição e passagem de tempo.
5. `sistema/organizacao-de-aventura.md` — como criar, consultar e salvar uma aventura.
6. `sistema/modelos.md` — modelos de ficha, status e arquivos de campanha.
7. Depois disso, leia o `README.md` da aventura que será narrada e somente então seus arquivos específicos.

## Separação obrigatória

### `sistema/`
Contém:
- regras universais;
- sintaxe de atributos, perícias e poderes;
- princípios de resolução;
- regras de agência;
- modelo narrativo e literário padrão;
- método genérico de organização e persistência.

### `aventuras/<nome>/`
Contém apenas dados daquela história:
- personagens concretos;
- mundo e regras específicas;
- relações;
- exceções ou complementos de narração daquela aventura;
- cronologia;
- estado atual;
- capítulos ou registro canônico do que aconteceu.

> **O sistema ensina como criar e operar. A aventura contém o que foi criado e o que aconteceu.**

## Herança narrativa

Toda aventura começa usando `sistema/narracao-e-escrita-padrao.md`.

As diretrizes da aventura podem alterar qualquer parte do estilo, mas devem declarar a exceção explicitamente. Tudo que não for alterado continua herdado do padrão do sistema.

Assim, outra IA não precisa consultar uma aventura antiga para descobrir como escrever: o modelo-base já existe dentro de `sistema/`.

## Princípio de operação

O narrador não deve decidir primeiro o que a trama precisa que aconteça e depois forçar personagens e regras a produzir esse resultado.

A ordem correta é:

> **Sistema + ficha + história + relações + estado atual + circunstância → decisão dos personagens → consequência → nova história.**

A aventura nasce dessas decisões.

## Continuidade

Ao continuar uma aventura em outro chat ou com outra IA, não dependa de memória de conversa anterior. Consulte os arquivos da aventura.

O registro persistente da aventura deve permitir reconstruir:
- quem cada personagem é;
- o que cada um pode fazer;
- o que já aconteceu;
- o que cada personagem plausivelmente sabe;
- quais relações mudaram;
- como todos estão no momento atual;
- quais exceções de narração valem naquela campanha.

## Prioridade

Quando houver conflito, siga primeiro uma correção explícita mais recente do usuário. Depois, use a hierarquia de cânone definida no `README.md` da própria aventura. Nunca invente retroativamente uma regra, poder, relação ou acontecimento apenas para resolver uma dificuldade da cena.