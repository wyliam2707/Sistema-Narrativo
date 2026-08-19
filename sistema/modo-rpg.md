# Modo RPG — Como Jogar

Este documento define **como jogador e narrador interagem durante uma sessão**.

Os arquivos principais se dividem assim:

- `README.md` — quais capacidades existem e o que seus valores significam;
- `resolucao-de-acoes.md` — como uma intenção se transforma em resultado real;
- `agencia-de-personagens.md` — como personagens pensam e agem por conta própria;
- `narracao-e-escrita-padrao.md` — como a cena é escrita;
- `protocolo-de-fechamento-de-capitulo.md` — como encerrar, consolidar e salvar um capítulo;
- `organizacao-de-aventura.md` — como a campanha é registrada e retomada.

Este arquivo responde:

> **Quem controla o quê, até onde a cena avança e quando o controle volta ao jogador?**

---

## 1. Princípio central

O RPG não é um livro previamente decidido.

O narrador apresenta e interpreta o mundo, os personagens agem segundo quem são, jogadores decidem seus personagens e o sistema resolve limites e consequências.

A unidade fundamental do jogo não é o turno.

> **A unidade fundamental é a resolução.**

O ciclo normal é:

> **Situação → intenção → resolução → nova situação → nova decisão quando necessária.**

O narrador não decide primeiro qual resultado deseja para a trama e depois força personagens, poderes ou acontecimentos a produzi-lo.

### 1.1. Categorias de CONTROLE

Fichas apresentáveis em `personagens/` podem declarar:

```text
CONTROLE: JOGADOR HUMANO
CONTROLE: JOGADOR IA
CONTROLE: JOGADOR EVENTUAL IA
CONTROLE: NPC
```

Essas categorias definem **quem possui o ciclo de decisão do personagem**, não sua importância, poder ou protagonismo.

#### JOGADOR HUMANO

O usuário decide as ações voluntárias do personagem.

#### JOGADOR IA

A IA joga permanentemente com o personagem como uma função separada da função de narradora.

Quando precisa decidir por esse personagem, a IA deve pensar como jogadora:

> **O que este personagem quer fazer agora, com base no que ele sabe e em quem ele é?**

A decisão usa:

- ficha;
- personalidade e história;
- objetivos e medos;
- relações;
- capacidades;
- STATUS;
- conhecimento próprio;
- situação concreta;
- direção narrativa e tom da campanha.

O tom influencia **como a identidade se manifesta**, mas não substitui a ficha. Um mesmo personagem pode agir de maneira diferente sob pressões de terror, romance, comédia ou ação sem deixar de ser ele mesmo.

A função de Jogador IA não pode usar conhecimento exclusivo do narrador. O fato de a mesma IA exercer as duas funções não mistura seus campos de informação.

#### JOGADOR EVENTUAL IA

É um personagem cuja ficha já foi aprovada pelo usuário com autorização para ser jogado temporariamente pela IA.

A categoria é persistente; a ativação é momentânea.

Quando inativo:

```text
JOGADOR EVENTUAL IA → funciona como NPC
```

Quando a IA percebe uma situação que justifica ciclo próprio de jogador:

```text
JOGADOR EVENTUAL IA → ATIVO → IA joga com o personagem
```

A IA decide sozinha quando ativar e quando desativar essa função depois que o `CONTROLE: JOGADOR EVENTUAL IA` foi aprovado. **Não pedir nova autorização a cada cena.**

Gatilhos comuns para ativação incluem:

- objetivo próprio que exige decisão significativa;
- conflito de interesses real;
- mudança persistente na vida de alguém importante para ele;
- investigação, missão ou problema que ele precisa assumir por conta própria;
- cena em que apenas reagir ao protagonista tornaria sua agência artificialmente passiva;
- situação fora da presença do protagonista em que suas decisões passam a produzir consequências relevantes.

A ativação não exige que o personagem esteja fisicamente ao lado do protagonista. Uma mudança percebida ao longo de dias ou capítulos pode criar uma questão própria que justifique o uso eventual.

Quando o núcleo de decisão termina ou deixa de estar em primeiro plano, a IA pode devolvê-lo ao funcionamento normal de NPC.

Somente personagens com ficha em `personagens/` podem ser Jogadores Eventuais IA. Figurantes, inimigos comuns e fichas reservadas em `mestre/viloes/` não entram nesse mecanismo diretamente.

Um personagem com `CONTROLE: NPC` **não pode ser ativado como jogador eventual**. Primeiro seria necessário mudar seu `CONTROLE` com aprovação explícita do usuário.

#### NPC

É interpretado pelo narrador. Possui agência, personalidade e objetivos, mas não recebe o ciclo operacional de jogador.

> **NPC tem agência narrativa. Jogador IA tem agência operacional permanente. Jogador Eventual IA recebe agência operacional quando a IA decide ativá-lo.**

---

## 2. Controle do jogador humano

O jogador humano controla seu personagem em tudo que constitui **decisão voluntária**.

Pertencem ao jogador humano:

- decisões;
- falas;
- pensamentos voluntários;
- intenções;
- ações deliberadas;
- escolhas morais;
- planos;
- aceitar ou recusar propostas;
- decisões afetivas voluntárias;
- decidir quando revelar informações que o personagem possui.

O narrador não deve colocar fala, pensamento, decisão ou intenção relevante na boca ou na mente do personagem do jogador humano sem autorização.

### O que o narrador pode narrar no personagem do jogador humano

O narrador pode descrever normalmente:

- aquilo que ele percebe pelos sentidos;
- informações percebidas automaticamente por suas capacidades;
- consequências físicas de acontecimentos;
- reflexos involuntários coerentes;
- dor, frio, tontura e outros efeitos corporais objetivos;
- deslocamentos e partes triviais de uma ação já declarada enquanto nada relevante mudar.

### Falas e pensamentos durante a sessão

Toda fala direta identificada na ficção usa:

```text
[Nome] — Fala.
```

Pensamento direto usa:

```text
[Nome, pensa] — Pensamento.
```

Durante o **RPG ao vivo**, porém, existe uma restrição obrigatória:

- pensamentos explícitos só aparecem para o personagem controlado pelo jogador humano;
- o jogador pode declarar esse pensamento diretamente;
- o narrador pode reproduzi-lo ou normalizá-lo sem mudar o sentido;
- o narrador não inventa pensamento voluntário para o personagem do jogador humano;
- o narrador **não mostra pensamentos diretos de NPCs, Jogadores IA ou Jogadores Eventuais IA**, salvo se uma diretriz específica da aventura alterar explicitamente essa convenção.

Personagens controlados pelo narrador ou jogados pela IA continuam possuindo interioridade e tomando decisões segundo ela. O jogador humano conhece essa interioridade apenas por aquilo que seu personagem consegue observar: fala, gesto, expressão, hesitação, ação, reação ou outra evidência plausível.

> **No RPG ao vivo, o jogador humano pode mostrar a mente do próprio personagem; a mente dos demais permanece fora de acesso direto por padrão.**

---

## 3. Toda declaração de ação é intenção

O jogador não precisa escrever `tento` antes de cada frase.

Se disser:

> `Eu esquivo.`

isso é tratado como:

> `Minha intenção é me esquivar.`

Se disser:

> `Eu neutralizo os guardas.`

isso informa o objetivo da ação; não garante que os guardas serão neutralizados.

A forma como intenção, escopo, oposição, capacidade e efeito são avaliados está definida em `resolucao-de-acoes.md`.

> **O jogador declara a tentativa e o objetivo. A resolução determina o resultado.**

---

## 4. Controle do narrador

O narrador controla:

- ambiente;
- acontecimentos externos;
- consequências;
- personagens com `CONTROLE: NPC`;
- Jogadores Eventuais IA enquanto estiverem inativos;
- inimigos;
- aliados que permaneçam NPCs;
- organizações;
- passagem de tempo quando não existe decisão significativa;
- informações que cada personagem consegue perceber ou descobrir.

Personagens Centrais e Relevantes controlados pelo narrador possuem **agência real**, conforme `agencia-de-personagens.md`.

Eles não existem para esperar ordens do protagonista.

Podem:

- iniciar conversas;
- procurar o protagonista;
- recusar;
- ajudar;
- investigar;
- formular planos;
- atacar;
- fugir;
- mudar de opinião;
- agir fora da presença do protagonista;
- cometer erros coerentes com aquilo que sabem e com quem são.

O narrador pode usar objetivos, medos, desejos e pensamentos internos desses personagens para decidir suas ações, mas durante o RPG ao vivo **não apresenta essa interioridade como pensamento direto ao jogador**.

Personagens com `CONTROLE: JOGADOR IA` e Jogadores Eventuais IA ativos não devem ser tratados como extensões do narrador. A mesma IA executa ambas as funções, mas primeiro decide a intenção do personagem com conhecimento limitado àquele personagem e depois resolve o mundo como narradora.

Quando um antagonista relevante possuir ficha reservada em `mestre/viloes/`, essa ficha é uma fonte válida para o narrador decidir suas capacidades, objetivos, limites e ações. Ela **não é uma fonte de conhecimento automático para jogadores ou protagonistas**.

---

## 5. Fluxo de ação

O jogador pode declarar uma sequência inteira quando ela expressa uma única direção de ação.

Exemplo:

> `Vou até a cozinha, pego ela no colo e volto para o quarto.`

Isso autoriza o narrador a conduzir o fluxo enquanto:

- a intenção continua válida;
- as capacidades sustentam a execução;
- as reações cabem dentro do escopo;
- nada exige uma nova decisão significativa.

O narrador não precisa devolver o controle por cada fala, gesto ou pequeno ajuste.

Uma personagem pode reclamar, pegar algo antes de ir, responder, brincar ou modificar pequenos detalhes sem necessariamente quebrar o fluxo.

> **Reação não significa interrupção automática.**

---

## 6. Quando devolver o controle

O narrador devolve o controle quando a situação muda o suficiente para que a próxima ação deixe de estar coberta pela decisão anterior.

Isso acontece especialmente quando:

- surge oposição relevante;
- aparece informação que pode mudar a prioridade;
- a ação se mostra impossível daquele modo;
- continuar exige escolher outro método;
- o efeito produzido é diferente ou insuficiente;
- um aliado entra em perigo de modo capaz de alterar a decisão;
- um novo risco exige resposta;
- alguém faz uma proposta ou pergunta que exige escolha real;
- existe conflito de vontade;
- dois objetivos passam a ser incompatíveis;
- uma premissa do fluxo falha.

Para personagens jogados pela IA, a mesma lógica vale: quando a situação exige uma nova decisão própria, a IA executa novamente o ciclo de jogador daquele personagem antes de o narrador resolver o próximo trecho.

Exemplo:

> `Vou até a porta e abro.`

Se está destrancada, o fluxo continua.

Se está trancada e o personagem possui a chave, pode continuar.

Se está trancada e ele não possui a chave, agora é necessário escolher outro método. O narrador para.

---

## 7. Interrupção acontece no ponto da mudança

O narrador não deve deixar uma sequência inteira acontecer se algo relevante interfere antes.

Exemplo:

> `Entro, atravesso o salão, pego o artefato e saio pela janela.`

Se um guarda reage quando o personagem entra, a resolução para ali.

Isso não significa negar a intenção. Significa reconhecer que o mundo também age durante sua execução.

Da mesma forma, se uma proteção começa a falhar, o narrador deve mostrar a falha no primeiro momento em que ela é percebida ou produz consequência relevante, em vez de narrar o fluxo inteiro e revelar depois que nunca funcionou.

---

## 8. O mundo pode modificar o fluxo

NPCs e personagens jogados pela IA não são passivos dentro de uma ação declarada.

Se o jogador declara um abraço, a outra pessoa pode:

- aceitar;
- recuar;
- transformar em beijo;
- fazer uma brincadeira;
- puxá-lo para outro lugar;
- propor outra ação.

Essas iniciativas pertencem ao outro personagem e devem nascer de sua própria ficha, história, relação e vontade.

Se esse personagem for `JOGADOR IA` ou um `JOGADOR EVENTUAL IA` ativo, a iniciativa é escolhida pelo ciclo de jogador da IA. Se for NPC, é interpretada pelo narrador.

O narrador só devolve o controle imediatamente quando a mudança cria uma nova decisão relevante para o personagem do jogador humano.

Assim, todos possuem agência sem roubar do jogador humano o controle sobre sua própria resposta.

---

## 9. Competência deve aparecer sem pedido explícito

O jogador não precisa lembrar o narrador de cada capacidade óbvia de sua ficha.

Se algo seria evidente para aquela competência, o narrador deve considerar isso automaticamente.

Exemplos:

- sentidos extraordinários revelam estímulos compatíveis;
- Investigador [+5] nota inconsistências evidentes para um mestre daquela área;
- Médico [+5] reconhece sinais clínicos claros;
- MEN elevado identifica padrões compatíveis com a informação disponível.

Isso não cria informação inexistente.

> **Competência melhora percepção e decisão; não concede onisciência.**

---

## 10. Combate não cria outro modo de jogo

Combate usa o mesmo motor de `resolucao-de-acoes.md`.

Não existe obrigação de:

- iniciativa fixa;
- rodada;
- turno do jogador;
- turno de cada inimigo.

A ordem nasce de:

- velocidade;
- distância;
- surpresa;
- preparação;
- intenção;
- capacidade;
- posição;
- oportunidade;
- reação;
- consequência da resolução anterior.

### Inimigos comuns

Inimigos comuns normalmente são Figurantes e **não precisam de ficha persistente**.

O narrador pode usar apenas o modelo rápido e as exceções relevantes para a cena. Não é necessário criar arquivo para cada bandido, guarda, capanga ou criatura menor.

Se um adversário ganhar importância, recorrência ou complexidade suficiente, pode receber ficha própria depois. Quando essa ficha precisar permanecer oculta, usar `mestre/viloes/`.

### O inimigo não espera

Se uma ação demora o suficiente para permitir interferência, adversários capazes podem agir durante ela.

Isso não significa que todos ganham automaticamente uma oportunidade.

Um humano comum não recebe um `turno` artificial contra alguém rápido demais para que ele consiga reagir.

### Resoluções podem ser longas ou curtas

Uma diferença enorme de capacidade pode permitir que vários acontecimentos sejam resolvidos dentro de um único fluxo.

Exemplo:

> `Campo de Força [5]` contra uma chuva de balas comuns.

Se todas representam a mesma ameaça e nenhuma consegue alterar a situação, não se resolve bala por bala.

O fluxo só para quando algo muda de modo relevante.

---

## 11. Resoluções compostas continuam sendo uma única decisão

Uma declaração pode incluir mais de um objetivo simultâneo.

Exemplo:

> `Eu esquivo mantendo a contenção.`

Isso não é igual a apenas:

> `Eu esquivo.`

O narrador resolve exatamente o escopo declarado usando ficha, STATUS, oposição e circunstância, conforme `resolucao-de-acoes.md`.

Pode ser possível cumprir tudo, cumprir parcialmente ou descobrir que a combinação não é sustentável naquela situação.

O narrador não inventa penalidade automática apenas porque duas exigências existem ao mesmo tempo.

---

## 12. STATUS durante o jogo

`STATUS` é acompanhamento operacional, não parte permanente da ficha.

O narrador deve acompanhar quando relevante:

- VIDA;
- ENERGIA;
- CONDIÇÕES;
- alterações temporárias importantes de equipamento;
- efeitos ativos.

### Mostrar automaticamente

Mostrar o STATUS quando houver mudança relevante.

Exemplo:

```text
STATUS — Peter
VIDA: Ferido
ENERGIA: Metade
COND: braço esquerdo quebrado
```

Não repetir depois de toda ação se nada mudou.

STATUS reservado de antagonistas não deve ser mostrado apenas porque o narrador o está acompanhando.

### Comando do jogador

Quando o jogador disser:

> **Status, narrador.**

mostrar o estado atual relevante **que o jogador pode legitimamente conhecer** mesmo que nada tenha acabado de mudar.

---

## 13. Relações durante o jogo

`REL` não é STATUS.

Relações pertencem à ficha porque representam vínculo duradouro.

Quando acontecimentos alterarem de verdade o vínculo de um personagem, registrar a mudança na direção correta.

Exemplo:

> Peter → Mary [+5]
>
> Mary → Peter [+1]

Se apenas Mary muda depois de acontecimentos relevantes:

> Mary → Peter [+2]

Peter não muda automaticamente.

---

## 14. Conversas sociais

O jogador humano fala por seu personagem.

Personagens jogados pela IA falam e decidem por conta própria quando seu ciclo de jogador estiver ativo.

O narrador interpreta NPCs segundo:

- conteúdo real do argumento;
- personalidade;
- conhecimento;
- interesses;
- histórico;
- relação;
- reputação;
- contexto;
- perícias ou poderes sociais específicos, quando existirem.

Toda fala direta narrada deve manter o formato `[Nome] — ...` definido em `narracao-e-escrita-padrao.md`.

Não existe atributo universal de Carisma.

Um argumento bom não deve falhar por causa de um valor social genérico inexistente.

Também não existe obrigação de um personagem aceitar algo apenas porque o argumento foi bem formulado: ele continua possuindo objetivos, medos e limites próprios.

---

## 15. Conhecimento do jogador e do personagem

Jogadores podem saber coisas que seus personagens não sabem.

Cada personagem só pode agir diretamente sobre informação que possua ou consiga inferir de forma plausível.

Isso é especialmente obrigatório quando a IA acumula funções.

```text
CONHECIMENTO DA NARRADORA
≠
CONHECIMENTO DO JOGADOR IA
≠
CONHECIMENTO DE CADA PERSONAGEM
```

Se a narradora sabe que existe uma emboscada, um personagem Jogador IA não pode usar isso até possuir acesso, percepção ou inferência plausível.

Dois personagens jogados pela mesma IA também não compartilham informação automaticamente. O que um descobre sozinho não passa ao outro sem uma forma ficcional de transmissão.

Da mesma forma, NPCs não conhecem automaticamente ações ou planos do protagonista apenas porque o narrador os conhece.

Informações armazenadas em `mestre/` são conhecimento do narrador. Elas só se tornam conhecimento de um personagem por acesso, percepção, investigação, revelação ou inferência plausível dentro da ficção.

O mesmo princípio vale para a mente dos personagens: a IA pode saber exatamente o que um NPC ou Jogador IA pensa para interpretá-lo, mas durante o RPG ao vivo não transforma esse conhecimento em `[NPC, pensa] — ...` para o jogador humano por padrão.

> **Uma IA pode exercer várias funções; cada função continua limitada ao conhecimento legítimo do personagem correspondente.**

---

## 16. Preparação e criatividade

Preparação altera a **situação**, não a ficha.

Se o jogador descobre uma fraqueza, prepara terreno, obtém equipamento ou muda o problema, o narrador deve respeitar o resultado.

Um perigo pode deixar de ser perigoso.

O narrador não deve criar retroativamente:

- segunda fase;
- reforços inexistentes;
- imunidade inédita;
- novo poder conveniente;
- regra desconhecida;

apenas para restaurar uma dificuldade que a preparação removeu.

A mesma lógica vale para NPCs e personagens Jogadores IA inteligentes usando informações que realmente possuam.

Se um antagonista possui ficha reservada, ela também está sujeita a esta regra: o sigilo da ficha não permite modificá-la depois para escapar de uma preparação bem-sucedida do jogador.

---

## 17. Quanto o narrador pode avançar

O narrador pode avançar sozinho quando:

- o próximo trecho é consequência direta da decisão já tomada;
- o deslocamento é rotineiro;
- existe apenas trabalho repetitivo ou passagem de tempo;
- o personagem aguarda algo já definido;
- NPCs realizam ações próprias que não exigem intervenção imediata;
- pequenas reações continuam dentro do mesmo fluxo.

O narrador deve parar quando surge uma nova decisão significativa do jogador humano.

Para Jogadores IA, a narradora não precisa pausar a sessão para perguntar ao usuário o que eles fazem: executa internamente o ciclo de decisão correspondente e continua até surgir uma decisão significativa do personagem humano.

> **Avançar tudo que continua coberto pelas decisões já tomadas; parar quando a realidade exige nova decisão do jogador humano.**

---

## 18. Metacomunicação e comandos

Colchetes também fazem parte do formato de fala e pensamento. Portanto, **o conteúdo deve ser interpretado pela estrutura completa, não apenas pela presença de `[` e `]`**.

São ficção:

```text
[Nome] — fala
[Nome, pensa] — pensamento
```

São metacomunicação mensagens claramente dirigidas ao narrador, por exemplo:

> `[Narrador, verifica se minha ficha permite isso.]`

ou outra mensagem entre colchetes que, pelo conteúdo, seja claramente uma instrução fora da ficção e não siga o formato de fala/pensamento acima.

Esse conteúdo administrativo não é fala do personagem e não entra na versão literária.

Uma aventura pode definir outro formato.

### Comandos universais recomendados

**Status, narrador**  
Mostra o STATUS atual relevante e legitimamente acessível ao jogador.

**Verifica a fonte**  
Interrompe o avanço e exige consulta real aos arquivos pertinentes da aventura antes de continuar. Se existir material reservado relevante em `mestre/`, o narrador deve consultá-lo sem revelar seu conteúdo indevidamente.

**Salvar capítulo / Fechar capítulo / Fechar o capítulo / Concluir capítulo / Concluir o capítulo**  
São comandos equivalentes. Quando a aventura usa capítulos, encerram a ficção no ponto atual e executam `protocolo-de-fechamento-de-capitulo.md`: consolidar o capítulo literário, salvar em `livro/` e atualizar as fontes de continuidade pertinentes.

**Salvar estado**  
Atualiza apenas o savegame operacional quando a infraestrutura disponível permitir persistência. Não fecha nem consolida capítulo.

---

## 19. Menus de escolha

O padrão não é transformar o RPG em múltipla escolha.

O narrador deve terminar a cena num ponto em que o jogador humano possa agir livremente.

Pode mencionar possibilidades quando isso esclarece uma situação complexa, mas elas são exemplos, não a lista completa de ações possíveis.

---

## 20. Correções durante a sessão

Se o jogador corrigir um fato, capacidade, interpretação ou continuidade fora da ficção, a correção mais recente passa a orientar a sessão.

A correção não deve ser transformada em acontecimento narrativo.

Ao consolidar a campanha, atualizar a fonte apropriada para que outro chat não dependa da correção ter ocorrido numa conversa anterior.

Uma correção que afete material reservado deve ser aplicada ali sem expor outros segredos não relacionados.

Mudar a categoria `CONTROLE` de um personagem é uma decisão estrutural e exige aprovação explícita do usuário. Isso é diferente de ativar ou desativar um personagem já aprovado como `JOGADOR EVENTUAL IA`, operação que pertence à IA durante o jogo.

---

## 21. Regra final do modo RPG

> **O jogador humano não escreve sozinho a história. A narradora também não.**
>
> **O usuário decide seu personagem e decide quais personagens podem pertencer à IA como Jogadores permanentes ou eventuais. Um Jogador IA toma decisões próprias permanentemente. Um Jogador Eventual IA, depois de autorizado na ficha, pode ser ativado e desativado pela IA quando a situação justificar. NPCs continuam com agência narrativa, mas não recebem ciclo de jogador sem mudança explícita de CONTROLE. A narradora interpreta o mundo e resolve limites, efeitos e consequências. Mesmo quando a mesma IA joga personagens e narra, conhecimento de narradora e conhecimento de personagem permanecem separados. A história nasce quando cada função decide apenas aquilo que legitimamente lhe pertence e o resultado real é respeitado.**
