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
10. `sistema/protocolo-de-criacao.md` — processo de nova campanha: nome, estrutura completa, direção narrativa e cenário, personagens, início, revisão e conversão mecânica posterior.
11. `sistema/protocolo-de-fechamento-de-capitulo.md` — como `Salvar capítulo`, `Fechar capítulo` e `Concluir capítulo` consolidam a sessão, salvam o livro e atualizam continuidade.
12. `sistema/organizacao-de-aventura.md` — como consultar, organizar e salvar uma aventura.
13. `sistema/modelos.md` — modelos de direção narrativa, ficha, STATUS, Progressão, READMEs estruturais e arquivos de campanha.
14. Depois disso, leia o `README.md` da aventura que será narrada e somente então seus arquivos específicos.

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
- protocolo de fechamento e salvamento de capítulos;
- checklist operacional do narrador;
- modelo narrativo e literário padrão;
- método genérico de organização e persistência.

### `aventuras/<nome>/`
Contém apenas dados daquela história:
- criação e revisão, enquanto a campanha estiver sendo montada;
- direção narrativa específica em `diretrizes/narracao.md`;
- personagens concretos;
- material reservado do narrador em `mestre/`, quando existir;
- mundo e regras específicas;
- relações;
- progressões narrativas e consequências ainda vivas;
- outras exceções ou complementos de narração daquela aventura;
- cronologia;
- estado atual;
- capítulos ou registro canônico do que aconteceu.

A estrutura de uma nova aventura nasce completa: cada pasta estrutural deve possuir desde o começo um `README.md` curto explicando sua função. Isso materializa as pastas no Git e permite que outra IA compreenda a organização mesmo antes de existirem arquivos de conteúdo dentro delas.

Esses `README.md` estruturais permanecem como legenda da organização. Eles não substituem fichas, estado, cronologia, Progressão ou capítulos e não devem virar depósitos de acontecimentos da campanha.

`mestre/` pode conter fichas e informações que outra IA precisa conhecer para manter a continuidade, mas que **não devem ser apresentadas ao jogador como conhecimento do protagonista** antes de serem descobertas na ficção.

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
`modo-rpg.md` determina **quem possui o ciclo de decisão de cada personagem, quando a cena avança e quando o controle retorna ao jogador humano**.

As fichas podem usar:

```text
JOGADOR HUMANO
JOGADOR IA
JOGADOR EVENTUAL IA
NPC
```

Jogadores IA possuem ciclo próprio de decisão e usam somente o conhecimento legítimo do personagem que controlam. Jogadores Eventuais IA alternam entre funcionamento de NPC e ciclo de jogador conforme as regras de `modo-rpg.md`.

A unidade fundamental do jogo não é o turno. É a resolução.

Durante o RPG ao vivo, toda fala direta usa `[Nome] — ...`. Pensamento direto usa `[Nome, pensa] — ...`, mas pensamentos explícitos aparecem somente para o personagem com `CONTROLE: JOGADOR HUMANO`, quando declarados ou autorizados pelo jogador humano. A interioridade de `NPC`, `JOGADOR IA` e `JOGADOR EVENTUAL IA` permanece oculta ao jogador humano por padrão e é percebida apenas por sinais disponíveis na ficção.

### Agência
`agencia-de-personagens.md` determina **como NPCs, Jogadores IA e Jogadores Eventuais IA formam suas próprias intenções** segundo ficha, personalidade, história, conhecimento, relações, objetivos, STATUS, direção narrativa e situação.

A diferença está em quem executa o ciclo de decisão:

```text
NPC → narrador
Jogador IA → IA como jogadora
Jogador Eventual IA → IA como jogadora quando ativado
```

Antagonistas reservados ao narrador continuam sujeitos à mesma agência e às mesmas regras. O sigilo de sua ficha não permite alterar retroativamente capacidades para contrariar o jogador.

### Progressão narrativa
`progressao-narrativa.md` determina **quais consequências continuam vivas depois da cena e podem voltar a alterar possibilidades futuras**.

Não existe XP ou recompensa mecânica automática por missão. A campanha progride por consequências: relações latentes, acessos, favores, recursos, posições, restrições, inimigos, promessas e outros efeitos duradouros que ainda tenham potencial causal.

> **Progressão não significa ficar mais forte. Significa acumular história que ainda pode voltar a importar.**

### Criação de campanha
`protocolo-de-criacao.md` determina **como transformar uma ideia em uma aventura pronta para jogar**.

A criação usa quatro etapas conceituais:

1. Direção narrativa e Cenário;
2. Protagonista;
3. Personagens relevantes;
4. Início da história.

A primeira etapa separa duas perguntas:

```text
Que tipo de história o jogador quer viver? → diretrizes/narracao.md
Em que mundo essa história acontece?       → mundo/cenario.md
```

Gênero e tom não são opções fechadas. O jogador pode combinar livremente comédia, romance, romance adulto, terror, ação, investigação, faroeste, drama ou qualquer outra direção desejada.

Assim que o nome da campanha é definido, a estrutura completa é criada com `README.md` em cada pasta estrutural e `criacao.md` para acompanhar o processo.

Cada etapa é salva como `PENDENTE DE REVISÃO`. A aplicação de atributos, perícias, poderes e demais conceitos numéricos acontece somente na revisão posterior.

Aliados relevantes podem começar apenas com nomes e fichas estruturais ainda vazias. Inimigos comuns não precisam de arquivo individual. Antagonistas importantes podem receber ficha reservada em `mestre/viloes/` quando isso passar a ser necessário.

> **Direção narrativa primeiro. Mundo e conceito depois. Mecânica por último.**

### Fechamento e salvamento de capítulo
`protocolo-de-fechamento-de-capitulo.md` determina **como transformar o material jogado em capítulo literário canônico e atualizar as fontes de continuidade**.

Os comandos `Salvar capítulo`, `Fechar capítulo` e `Concluir capítulo` são equivalentes.

O protocolo para a ficção no ponto atual, consulta as fontes necessárias, consolida somente os acontecimentos válidos, remove metacomunicação e versões descartadas, salva em `livro/` e atualiza cronologia, Progressão, fichas, relacionamentos e estado apenas quando pertinente.

No livro consolidado, falas continuam identificadas como `[Nome] — ...`, enquanto pensamentos de qualquer personagem podem aparecer como `[Nome, pensa] — ...` quando forem coerentes com a cena e não alterarem o cânone.

Quando material reservado do narrador for relevante, ele pode ser consultado e atualizado sem expor ao livro ou ao jogador informações que não foram descobertas na ficção ou que não pertençam legitimamente ao ponto de vista literário adotado.

> **A consolidação melhora a forma; não muda os fatos.**

### Checklist operacional
`checklist-do-narrador.md` resume as regras já estabelecidas em uma sequência de consulta rápida durante a sessão.

Ele não substitui os arquivos completos nem cria exceções. Em caso de dúvida, prevalece a regra detalhada do documento correspondente.

### Narração e persistência
Determinam **como a cena é escrita** e **como os acontecimentos são registrados** para continuidade.

Essas camadas trabalham juntas, mas uma não substitui a outra.

## Herança narrativa

Toda aventura começa usando `sistema/narracao-e-escrita-padrao.md`.

Durante a criação, `diretrizes/narracao.md` registra a direção narrativa específica escolhida para aquela campanha. Esse arquivo pode definir gênero, combinação de gêneros, tom, foco, ritmo, humor, romance/intimidade, atmosfera, ênfases ou outras escolhas locais.

As diretrizes da aventura podem alterar qualquer parte do estilo, mas devem declarar a exceção explicitamente. Tudo que não for alterado continua herdado do padrão do sistema.

Assim, outra IA não precisa consultar uma aventura antiga para descobrir como escrever: primeiro lê o modelo-base e depois a direção narrativa da campanha atual.

## Princípio de operação

O narrador não deve decidir primeiro o que a trama precisa que aconteça e depois forçar personagens e regras a produzir esse resultado.

A ordem correta é:

> **Sistema + direção narrativa + ficha + história + relações + estado atual + circunstância → intenção dos personagens → resolução → consequência → nova história.**

Durante o RPG, cada personagem segue o ciclo indicado por `CONTROLE`: o jogador humano decide por `JOGADOR HUMANO`; a IA como jogadora decide por `JOGADOR IA` e por `JOGADOR EVENTUAL IA` quando ativado; o narrador controla o mundo e interpreta `NPC` e `JOGADOR EVENTUAL IA` quando inativo.

Uma declaração como `eu esquivo`, `eu neutralizo`, `eu abro a porta` ou `eu chego até ela` informa **o que o personagem tenta fazer**. O resultado é determinado pela resolução, não pela forma afirmativa da frase.

A aventura nasce dessas decisões e consequências.

## Continuidade

Ao continuar uma aventura em outro chat ou com outra IA, não dependa de memória de conversa anterior. Consulte os arquivos da aventura.

O registro persistente da aventura deve permitir reconstruir:
- que tipo de história deve ser narrada e com qual tom;
- quem cada personagem é;
- o que cada um pode fazer;
- quais antagonistas ou segredos reservados ao narrador ainda estão ativos, quando existirem;
- o que já aconteceu;
- o que cada personagem plausivelmente sabe;
- quais relações mudaram;
- quais consequências antigas ainda podem voltar a importar;
- como todos estão no momento atual;
- quais exceções de narração valem naquela campanha.

Os `README.md` estruturais ajudam a localizar rapidamente cada tipo de informação, mas a continuidade factual continua pertencendo aos arquivos canônicos correspondentes.

Ao carregar uma campanha, consultar `diretrizes/narracao.md` antes de narrar novas cenas.

Ao consultar `mestre/`, separar rigorosamente **o que o narrador sabe** daquilo que o protagonista pode saber.

## Prioridade

Quando houver conflito, siga primeiro uma correção explícita mais recente do usuário. Depois, use a hierarquia de cânone definida no `README.md` da própria aventura. Nunca invente retroativamente uma regra, poder, relação ou acontecimento apenas para resolver uma dificuldade da cena.
