# LEIA PRIMEIRO — Como usar o Sistema Narrativo

Este diretório contém **regras universais e padrões de operação**. Ele deve permitir que um novo narrador — humano ou IA — entenda o sistema sem depender de outra conversa.

## REGRA DE PRIORIDADE MÁXIMA — Ciclo de Jogadores

Antes de qualquer outra regra operacional, leia `sistema/ciclo-de-jogadores.md`.

Quando houver mais de um jogador operacional, humano ou IA, **nenhum resultado pode ser narrado antes de todos os jogadores ativos terem declarado sua intenção para a mesma janela de resolução**.

O ciclo-base é:

```text
JOGADOR HUMANO declara
↓
JOGADOR IA [1] declara
↓
JOGADOR IA [2] declara
↓
outros Jogadores IA/Eventuais ativos declaram, se existirem
↓
NARRADOR resolve o conjunto
↓
NOVA SITUAÇÃO
```

Essa ordem de declaração não cria turnos rígidos nem conhecimento automático entre personagens. Cada jogador da IA decide usando somente o conhecimento legítimo do personagem que controla. As intenções podem ser favoráveis, contrárias, independentes, neutras ou apenas continuidade de algo já em andamento.

> **Jogadores escolhem intenções. Narrador descobre resultados.**

Nenhuma regra de ritmo, avanço automático ou resolução direta permite pular essa Janela de Declarações quando existe uma nova decisão significativa. A única prioridade superior é uma correção ou instrução explícita mais recente do usuário.

## Entrada do sistema

Quando o repositório for usado para iniciar um RPG, a primeira decisão é sempre:

> **Nova campanha ou continuar uma campanha existente?**

- **Nova campanha:** usar `sistema/criacao/README.md`.
- **Continuar:** consultar as campanhas realmente existentes em `campanhas/`, deixar o jogador escolher e abrir `campanhas/<nome>/README.md`.

O `README.md` da própria campanha indica onde consultar seu conteúdo e, enquanto a criação estiver em andamento, de onde retomar o processo.

Material antigo em `aventuras/` permanece preservado como legado. Não mover, apagar ou converter esse material automaticamente, e não usar `sistema/protocolo-de-criacao.md` como porta principal para novas campanhas.

Não pedir ao jogador para repetir informações que os arquivos já conseguem fornecer.

> **NOVA CAMPANHA → `sistema/criacao/README.md`**
>
> **CONTINUAR → `campanhas/<nome>/README.md`**

## Ordem de leitura

1. `sistema/ciclo-de-jogadores.md` — **regra operacional de prioridade máxima**: todos os jogadores ativos declaram antes de o Narrador resolver.
2. `sistema/README.md` — regras mecânicas, escala, atributos, perícias, poderes, Vida, Energia e linguagem de ficha.
3. `sistema/resolucao-de-acoes.md` — como uma intenção vira resultado: escopo, fluxo, interferência, oposição, limites, efeito e nova situação.
4. `sistema/informacao-e-descoberta.md` — como fatos existem, são percebidos, interpretados, investigados e transformados em conhecimento.
5. `sistema/modo-rpg.md` — como jogador e narrador interagem durante a sessão: controle, ritmo de avanço, interrupções, STATUS e comandos.
6. `sistema/agencia-de-personagens.md` — como personagens pensam, escolhem e agem por conta própria.
7. `sistema/progressao-narrativa.md` — como consequências duradouras, acessos, favores, relações latentes, ameaças e ganchos persistem sem XP ou progressão automática de poder.
8. `sistema/checklist-do-narrador.md` — referência operacional curta para aplicar as regras durante a sessão sem reler todos os documentos a cada resolução.
9. `sistema/narracao-e-escrita-padrao.md` — modelo narrativo e literário herdado por toda campanha, salvo exceção explícita.
10. `sistema/exemplo-de-estilo.md` — exemplo neutro para calibrar ritmo, diálogo, descrição e passagem de tempo.
11. Para criar uma campanha nova, `sistema/criacao/README.md` — processo canônico atual de criação.
12. `sistema/protocolo-de-fechamento-de-capitulo.md` — como `Salvar capítulo`, `Fechar capítulo` e `Concluir capítulo` consolidam a sessão, salvam o livro e atualizam continuidade.
13. Os documentos de organização e modelos ainda existentes no sistema podem ser consultados como referência complementar quando compatíveis com a estrutura atual.
14. Para continuar uma campanha atual, ler primeiro `campanhas/<nome>/README.md` e seguir o mapa de consulta indicado ali.

## Separação obrigatória

### `sistema/`
Contém:
- regras universais;
- sintaxe de atributos, perícias e poderes;
- **ciclo universal de declaração dos jogadores antes da resolução**;
- motor universal de resolução de ações;
- regras de informação, percepção e descoberta;
- protocolo de jogo entre jogador e narrador;
- regras de agência;
- regras de progressão narrativa e consequências persistentes;
- processo canônico de criação de novas campanhas em `sistema/criacao/`;
- protocolo de fechamento e salvamento de capítulos;
- checklist operacional do narrador;
- modelo narrativo e literário padrão;
- método genérico de organização e persistência.

### `campanhas/<nome>/`
Contém os dados concretos das campanhas criadas pelo fluxo atual.

A estrutura-base é definida por `sistema/criacao/estrutura-da-campanha.md` e separa:

```text
PERSONAGENS → quem são as peças
ESTADO      → como as coisas estão agora
MUNDO       → o que existe
MESTRE      → o que é reservado à condução
LIVRO       → o que aconteceu
```

O `README.md` da campanha é sua porta de entrada operacional e, durante a criação, guarda somente o checkpoint necessário para retomar o processo.

### `aventuras/`
É material legado.

Campanhas antigas ali existentes permanecem preservadas até uma migração explícita. Não mover, apagar, reestruturar nem converter automaticamente esse conteúdo apenas porque o fluxo atual usa `campanhas/`.

> **O sistema ensina como criar, declarar, resolver, jogar e operar. A campanha contém o que foi criado e o que aconteceu.**

## Camadas que não devem ser confundidas

### Ciclo de Jogadores
`ciclo-de-jogadores.md` determina **quem declara antes de o Narrador poder resolver**.

Em uma sessão com múltiplos jogadores operacionais:

```text
Situação
→ JOGADOR HUMANO declara
→ JOGADORES IA/Eventuais ativos declaram
→ NARRADOR resolve
→ Nova situação
```

A ordem é operacional, não uma iniciativa automática dentro da ficção. Um jogador posterior não recebe conhecimento de uma intenção secreta apenas porque ela foi declarada antes no processo.

### Ficha e capacidades
`README.md` determina **o que existe no personagem** e o que os valores significam.

### Resolução de ações
`resolucao-de-acoes.md` determina **o que realmente acontece quando alguém tenta alguma coisa** depois que a Janela de Declarações pertinente foi concluída.

A declaração do jogador é intenção, não resultado garantido.

> **Intenções declaradas → Escopo → Ficha/STATUS/Cena → Execução → Efeito real → Nova situação.**

### Informação e descoberta
`informacao-e-descoberta.md` determina **o que existe para ser descoberto, o que cada personagem consegue perceber, como interpreta evidências e até onde suas conclusões podem ir**.

> **Existência → Acesso → Percepção → Interpretação → Hipótese → Investigação → Confirmação.**

Capacidade não cria informação inexistente. Competência aprofunda a leitura daquilo que realmente está disponível.

### Modo RPG
`modo-rpg.md` determina **quem possui o ciclo de decisão de cada personagem, quando a cena avança e quando o controle retorna ao jogador humano**.

As fichas podem usar categorias de `CONTROLE` definidas pelo sistema, incluindo jogador humano, jogadores IA e personagens operados eventualmente pela IA.

Jogadores IA possuem ciclo próprio de decisão e usam somente o conhecimento legítimo do personagem que controlam. Jogadores Eventuais IA alternam entre funcionamento de NPC e ciclo de jogador conforme as regras vigentes de agência e operação.

A unidade fundamental do jogo não é o turno. É a resolução, **precedida pela Janela de Declarações quando existem múltiplos jogadores operacionais**.

Durante o RPG ao vivo, toda fala direta usa `[Nome] — ...`. Pensamento direto usa `[Nome, pensa] — ...`, mas pensamentos explícitos aparecem somente para o personagem com `CONTROLE: JOGADOR HUMANO`, quando declarados ou autorizados pelo jogador humano. A interioridade dos demais personagens permanece oculta ao jogador humano por padrão e é percebida apenas por sinais disponíveis na ficção.

### Agência
`agencia-de-personagens.md` determina **como NPCs, Jogadores IA e Jogadores Eventuais IA formam suas próprias intenções** segundo ficha, personalidade, história, conhecimento, relações, objetivos, STATUS, direção narrativa e situação.

Quando houver uma Janela de Declarações, cada Jogador IA ativo forma sua intenção **antes** de o Narrador conhecer o resultado da resolução.

Antagonistas reservados ao narrador continuam sujeitos à mesma agência e às mesmas regras. O sigilo de sua ficha não permite alterar retroativamente capacidades para contrariar o jogador.

### Progressão narrativa
`progressao-narrativa.md` determina **quais consequências continuam vivas depois da cena e podem voltar a alterar possibilidades futuras**.

Não existe XP ou recompensa mecânica automática por missão. A campanha progride por consequências: relações latentes, acessos, favores, recursos, posições, restrições, inimigos, promessas e outros efeitos duradouros que ainda tenham potencial causal.

> **Progressão não significa ficar mais forte. Significa acumular história que ainda pode voltar a importar.**

### Criação de campanha
`sistema/criacao/README.md` determina **como transformar uma ideia em uma campanha pronta para jogar** no fluxo atual.

A criação segue, em alto nível:

```text
Nome da campanha
→ Direção narrativa e cenário
→ Protagonista
→ Personagens com agência de jogador
→ Início da história
→ Revisão mecânica e aprovação
```

O conteúdo concreto é salvo diretamente em `campanhas/<nome>/` conforme `sistema/criacao/estrutura-da-campanha.md`.

A criação mantém checkpoint no `README.md` da própria campanha, persiste blocos mecânicos somente depois de aprovados e termina consolidando `estado/atual.md` antes da primeira cena.

> **Conceito primeiro. Mecânica depois.**

### Fechamento e salvamento de capítulo
`protocolo-de-fechamento-de-capitulo.md` determina **como transformar o material jogado em capítulo literário canônico e atualizar as fontes de continuidade**.

Os comandos `Salvar capítulo`, `Fechar capítulo` e `Concluir capítulo` são equivalentes.

O protocolo para a ficção no ponto atual, consulta as fontes necessárias, consolida somente os acontecimentos válidos, remove metacomunicação e versões descartadas, salva em `livro/` e atualiza as fontes de continuidade apenas quando pertinente.

Quando material reservado do narrador for relevante, ele pode ser consultado e atualizado sem expor ao livro ou ao jogador informações que não foram descobertas na ficção ou que não pertençam legitimamente ao ponto de vista adotado.

> **A consolidação melhora a forma; não muda os fatos.**

### Checklist operacional
`checklist-do-narrador.md` resume as regras já estabelecidas em uma sequência de consulta rápida durante a sessão.

Ele não substitui os arquivos completos nem cria exceções. Em caso de dúvida, prevalece a regra detalhada do documento correspondente.

### Narração e persistência
Determinam **como a cena é escrita** e **como os acontecimentos são registrados** para continuidade.

Essas camadas trabalham juntas, mas uma não substitui a outra.

## Herança narrativa

Toda campanha começa usando `sistema/narracao-e-escrita-padrao.md` salvo quando a própria campanha estabelecer uma exceção explícita.

A direção narrativa específica fica registrada nas fontes da própria campanha conforme o processo atual de criação. Tudo que não for alterado localmente continua herdado do padrão do sistema.

## Princípio de operação

O narrador não deve decidir primeiro o que a trama precisa que aconteça e depois forçar personagens e regras a produzir esse resultado.

A ordem correta é:

> **Sistema + direção narrativa + ficha + história + relações + estado atual + circunstância → declarações de todos os jogadores ativos → resolução → consequência → nova história.**

Durante o RPG, cada personagem segue o ciclo indicado por `CONTROLE`.

Uma declaração como `eu esquivo`, `eu neutralizo`, `eu abro a porta` ou `eu chego até ela` informa **o que o personagem tenta fazer**. Antes de o resultado ser resolvido, os demais jogadores operacionais ativos recebem sua própria oportunidade de declarar intenção para a mesma janela.

A campanha nasce dessas decisões e consequências.

## Continuidade

Ao continuar uma campanha em outro chat ou com outra IA, não dependa de memória de conversa anterior. Consulte os arquivos da campanha.

Para campanhas do fluxo atual, começar sempre por:

```text
campanhas/<nome>/README.md
```

Esse arquivo orienta quais fontes devem ser consultadas e onde o jogo ou a criação devem ser retomados.

O registro persistente deve permitir reconstruir o necessário para continuar corretamente sem pedir ao jogador que reconte o que os arquivos já registram.

Ao consultar `mestre/`, separar rigorosamente **o que o narrador sabe** daquilo que cada personagem pode saber.

## Prioridade

Quando houver conflito, siga primeiro uma correção explícita mais recente do usuário.

Depois disso, dentro das regras universais do sistema, `sistema/ciclo-de-jogadores.md` possui **prioridade operacional máxima** sobre formulações simplificadas de fluxo presentes em outros documentos: nenhuma resolução de nova decisão significativa pode ocorrer antes das declarações dos jogadores operacionais ativos.

Em seguida, para campanhas do fluxo atual, use as fontes e a hierarquia indicadas no `README.md` da própria campanha. Nunca invente retroativamente uma regra, poder, relação ou acontecimento apenas para resolver uma dificuldade da cena.
