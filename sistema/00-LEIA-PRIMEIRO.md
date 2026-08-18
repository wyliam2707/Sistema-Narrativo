# LEIA PRIMEIRO — Como usar o Sistema Narrativo

Este diretório contém **regras universais e padrões de operação**. Ele deve permitir que um novo narrador — humano ou IA — entenda o sistema sem depender de outra conversa.

## Entrada do sistema

Quando o repositório for usado para iniciar um RPG, a primeira decisão é sempre:

> **Nova campanha ou continuar uma campanha existente?**

- **Nova campanha:** usar `sistema/protocolo-de-criacao.md`.
- **Continuar:** listar as campanhas realmente existentes em `aventuras/`, deixar o jogador escolher e carregar a aventura a partir de seus próprios arquivos.

Se uma aventura escolhida possuir `criacao.md` ainda em andamento, retomar a criação do ponto registrado em vez de iniciar a narrativa.

Não pedir ao jogador para repetir informações que os arquivos já conseguem fornecer.

## Ordem de leitura

1. `sistema/README.md` — regras mecânicas, escala, atributos, perícias, poderes, Vida, Energia e linguagem de ficha.
2. `sistema/resolucao-de-acoes.md` — como uma intenção vira resultado: escopo, fluxo, interferência, oposição, limites, efeito e nova situação.
3. `sistema/informacao-e-descoberta.md` — como fatos existem, são percebidos, interpretados, investigados e transformados em conhecimento.
4. `sistema/modo-rpg.md` — como jogador e narrador interagem durante a sessão: controle, ritmo de avanço, interrupções, STATUS e comandos.
5. `sistema/agencia-de-personagens.md` — como personagens pensam, escolhem e agem por conta própria.
6. `sistema/progressao-narrativa.md` — como consequências duradouras, acessos, favores, relações latentes, ameaças e ganchos persistem sem XP ou progressão automática de poder.
7. `sistema/checklist-do-narrador.md` — referência operacional curta para aplicar as regras durante a sessão sem reler todos os documentos a cada resolução.
8. `sistema/narracao-e-escrita-padrao.md` — modelo narrativo e literário herdado por toda aventura, salvo exceção explícita.
9. `sistema/exemplo-de-estilo.md` — exemplo neutro para calibrar ritmo, diálogo, descrição e passagem de tempo.
10. `sistema/protocolo-de-criacao.md` — processo de nova campanha: nome, quatro etapas conceituais, salvamento pendente de revisão e conversão mecânica posterior.
11. `sistema/organizacao-de-aventura.md` — como consultar, organizar e salvar uma aventura.
12. `sistema/modelos.md` — modelos de ficha, STATUS, Progressão e arquivos de campanha.
13. Depois disso, leia o `README.md` da aventura que será narrada e somente então seus arquivos específicos.

## Separação obrigatória

### `sistema/`
Contém:
- regras universais;
- sintaxe de atributos, perícias e poderes;
- motor universal de resolução de ações;
- regras de informação, percepção e descoberta;
- protocolo de jogo entre jogador e narrador;
- regras de agência;
- regras de progressão narrativa e consequências persistentes;
- protocolo de criação de novas campanhas;
- checklist operacional do narrador;
- modelo narrativo e literário padrão;
- método genérico de organização e persistência.

### `aventuras/<nome>/`
Contém apenas dados daquela história:
- criação e revisão, enquanto a campanha estiver sendo montada;
- personagens concretos;
- mundo e regras específicas;
- relações;
- progressões narrativas e consequências ainda vivas;
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

> **Existência → Acesso → Percepção → Interpretação → Hipótese → Investigação → Confirmação.**

Capacidade não cria informação inexistente. Competência aprofunda a leitura daquilo que realmente está disponível.

### Modo RPG
`modo-rpg.md` determina **quem controla cada decisão, quando a cena avança e quando o controle retorna ao jogador**.

A unidade fundamental do jogo não é o turno. É a resolução.

### Agência
`agencia-de-personagens.md` determina **como personagens controlados pelo narrador escolhem suas próprias intenções** segundo ficha, personalidade, história, conhecimento, relações, objetivos e STATUS.

### Progressão narrativa
`progressao-narrativa.md` determina **quais consequências continuam vivas depois da cena e podem voltar a alterar possibilidades futuras**.

Não existe XP ou recompensa mecânica automática por missão. A campanha progride por consequências: relações latentes, acessos, favores, recursos, posições, restrições, inimigos, promessas e outros efeitos duradouros que ainda tenham potencial causal.

> **Progressão não significa ficar mais forte. Significa acumular história que ainda pode voltar a importar.**

### Criação de campanha
`protocolo-de-criacao.md` determina **como transformar uma ideia em uma aventura pronta para jogar**.

A criação usa quatro etapas conceituais:

1. Cenário;
2. Protagonista;
3. Personagens relevantes;
4. Início da história.

Cada etapa é salva como `PENDENTE DE REVISÃO`. A aplicação de atributos, perícias, poderes e demais conceitos numéricos acontece somente na revisão posterior.

> **Conceito primeiro. Mecânica depois.**

### Checklist operacional
`checklist-do-narrador.md` resume as regras já estabelecidas em uma sequência de consulta rápida durante a sessão.

Ele não substitui os arquivos completos nem cria exceções. Em caso de dúvida, prevalece a regra detalhada do documento correspondente.

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
- quais consequências antigas ainda podem voltar a importar;
- como todos estão no momento atual;
- quais exceções de narração valem naquela campanha.

## Prioridade

Quando houver conflito, siga primeiro uma correção explícita mais recente do usuário. Depois, use a hierarquia de cânone definida no `README.md` da própria aventura. Nunca invente retroativamente uma regra, poder, relação ou acontecimento apenas para resolver uma dificuldade da cena.