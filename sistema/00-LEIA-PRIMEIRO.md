# LEIA PRIMEIRO — Como usar o Sistema Narrativo

Este diretório contém **regras universais e padrões de operação**. Ele deve permitir que um novo narrador — humano ou IA — entenda o sistema sem depender de outra conversa.

## Ordem de leitura

1. `sistema/README.md` — regras mecânicas, escala, atributos, perícias, poderes, Vida, Energia e linguagem de ficha.
2. `sistema/resolucao-de-acoes.md` — como uma intenção vira resultado: escopo, fluxo, interferência, oposição, limites, efeito e nova situação.
3. `sistema/informacao-e-descoberta.md` — como fatos existem, são percebidos, interpretados, investigados e transformados em conhecimento.
4. `sistema/modo-rpg.md` — como jogador e narrador interagem durante a sessão: controle, ritmo de avanço, interrupções, STATUS e comandos.
5. `sistema/agencia-de-personagens.md` — como personagens pensam, escolhem e agem por conta própria.
6. `sistema/narracao-e-escrita-padrao.md` — modelo narrativo e literário herdado por toda aventura, salvo exceção explícita.
7. `sistema/exemplo-de-estilo.md` — exemplo neutro para calibrar ritmo, diálogo, descrição e passagem de tempo.
8. `sistema/organizacao-de-aventura.md` — como criar, consultar e salvar uma aventura.
9. `sistema/modelos.md` — modelos de ficha, STATUS e arquivos de campanha.
10. Depois disso, leia o `README.md` da aventura que será narrada e somente então seus arquivos específicos.

## Separação obrigatória

### `sistema/`
Contém:
- regras universais;
- sintaxe de atributos, perícias e poderes;
- motor universal de resolução de ações;
- regras de informação, percepção e descoberta;
- protocolo de jogo entre jogador e narrador;
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

> **O sistema ensina como criar, resolver, jogar e operar. A aventura contém o que foi criado e o que aconteceu.**

## Camadas que não devem ser confundidas

### Ficha e capacidades
`README.md` determina **o que existe no personagem** e o que os valores significam.

### Resolução de ações
`resolucao-de-acoes.md` determina **o que realmente acontece quando alguém tenta alguma coisa**.

A declaração do jogador é intenção, não resultado garantido.

> **Intenção → Escopo → Ficha/STATUS/Cena → Execução → Efeito real → Nova situação.**

### Informação e descoberta
`informacao-e-descoberta.md` determina **o que existe para ser descoberto, o que cada personagem consegue perceber, como interpreta evidências e até onde suas conclusões podem ir**.

> **Existência → Acesso → Percepção → Interpretação → Inferência → Confirmação.**

Capacidade não cria informação inexistente. Competência aprofunda a leitura daquilo que realmente está disponível.

### Modo RPG
`modo-rpg.md` determina **quem controla cada decisão, quando a cena avança e quando o controle retorna ao jogador**.

A unidade fundamental do jogo não é o turno. É a resolução.

### Agência
`agencia-de-personagens.md` determina **como personagens controlados pelo narrador escolhem suas próprias intenções** segundo ficha, personalidade, história, conhecimento, relações, objetivos e STATUS.

### Narração e persistência
Determinam **como a cena é escrita** e **como os acontecimentos são registrados** para continuidade.

Essas camadas trabalham juntas, mas uma não substitui a outra.

## Herança narrativa

Toda aventura começa usando `sistema/narracao-e-escrita-padrao.md`.

As diretrizes da aventura podem alterar qualquer parte do estilo, mas devem declarar a exceção explicitamente. Tudo que não for alterado continua herdado do padrão do sistema.

Assim, outra IA não precisa consultar uma aventura antiga para descobrir como escrever: o modelo-base já existe dentro de `sistema/`.

## Princípio de operação

O narrador não deve decidir primeiro o que a trama precisa que aconteça e depois forçar personagens e regras a produzir esse resultado.

A ordem correta é:

> **Sistema + ficha + história + relações + estado atual + circunstância → intenção dos personagens → resolução → consequência → nova história.**

Durante o RPG, o jogador mantém controle sobre as decisões voluntárias de seu personagem, enquanto o narrador controla o mundo e interpreta os demais personagens segundo suas próprias fichas, histórias e objetivos.

Uma declaração como `eu esquivo`, `eu neutralizo`, `eu abro a porta` ou `eu chego até ela` informa **o que o personagem tenta fazer**. O resultado é determinado pela resolução, não pela forma afirmativa da frase.

A aventura nasce dessas decisões e consequências.

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