# Organização e Persistência de uma Aventura

Este documento ensina como transformar as regras universais de `sistema/` em uma aventura concreta que possa ser retomada por outro chat ou outra IA sem depender de memória anterior.

## Estrutura recomendada

Cada campanha deve ficar em uma pasta própria e nascer com toda a sua estrutura materializada por `README.md`:

```text
aventuras/<nome-da-aventura>/
├── README.md
├── criacao.md
├── diretrizes/
│   ├── README.md
│   └── narracao.md
├── personagens/
│   └── README.md
├── mestre/
│   ├── README.md
│   └── viloes/
│       └── README.md
├── mundo/
│   └── README.md
├── relacionamento/
│   └── README.md
├── progressao/
│   └── README.md
├── cronologia/
│   └── README.md
├── estado/
│   ├── README.md
│   ├── inicio.md
│   └── atual.md
└── livro/
    └── README.md
```

Os `README.md` estruturais são criados junto com a campanha. `diretrizes/narracao.md` é criado e preenchido durante a Etapa 1 do protocolo, quando a direção narrativa da campanha é definida; `estado/inicio.md` e `estado/atual.md` surgem conforme o fluxo de criação e revisão.

Git não preserva diretórios vazios. Por isso, os `README.md` estruturais são parte da organização padrão e **devem ser criados junto com a campanha**, não apenas quando a pasta receber seu primeiro conteúdo real.

Cada `README.md` estrutural deve ser curto e suficiente para outra IA entender:

- a função da pasta;
- o que deve ser armazenado ali;
- o que não pertence ali quando houver risco de confusão;
- regras especiais de visibilidade, cânone ou persistência daquela área.

Esses arquivos permanecem mesmo depois que a pasta ganha outros conteúdos. Eles funcionam como legenda permanente da estrutura.

## Função de cada pasta

### `README.md`
É a porta de entrada da aventura.

Deve informar:
- premissa;
- protagonistas ou personagens centrais;
- ponto atual da campanha;
- hierarquia de cânone;
- quais diretrizes devem ser lidas antes de narrar;
- onde está o estado atual.

Durante a criação, o `README.md` da raiz pode ser provisório e apenas indicar que a campanha está em montagem e apontar para `criacao.md`. Depois da aprovação final, deve ser atualizado para a porta de entrada completa da campanha.

### `diretrizes/`
Define **como aquela aventura deve ser sentida, narrada e conduzida em termos de estilo local**.

O arquivo padrão é:

```text
diretrizes/narracao.md
```

Ele nasce da Etapa 1 — Direção narrativa e Cenário — e registra somente o que realmente importa para aquela campanha, por exemplo:

- gênero ou combinação de gêneros;
- tom principal e tons secundários;
- foco narrativo;
- ritmo;
- presença e natureza do humor;
- romance e intimidade, quando relevantes;
- atmosfera;
- elementos a enfatizar;
- elementos a evitar ou moderar;
- exceções ao modelo narrativo universal.

A lista não é obrigatória nem fechada. Uma campanha pode ser, por exemplo, comédia romântica, romance adulto, terror sobrenatural com romance, faroeste clássico ou qualquer combinação descrita pelo jogador.

Essas diretrizes pertencem à aventura e **não** ao sistema universal.

O `diretrizes/README.md` explica a função da pasta. `diretrizes/narracao.md` contém a direção narrativa concreta da campanha.

Toda aventura continua herdando `sistema/narracao-e-escrita-padrao.md`; `diretrizes/narracao.md` especifica a experiência local e substitui apenas aquilo que declarar de forma diferente.

### Separação entre `diretrizes/` e `mundo/`

Usar esta distinção:

> **Diretrizes dizem como a história deve ser narrada. Mundo diz o que existe na história.**

Exemplo:

```text
mundo/cenario.md: magia é pública e cotidiana.
diretrizes/narracao.md: magia cotidiana deve aparecer naturalmente, sem espetáculo obrigatório a cada uso.
```

Não duplicar automaticamente o mesmo texto nos dois lugares.

### `personagens/`
Contém as fichas estáveis e normalmente apresentáveis ao jogador de personagens Centrais e Relevantes.

A ficha responde principalmente:
- quem é;
- como costuma agir;
- quais capacidades possui;
- quais relações recorrentes da vida atual precisam ser acompanhadas.

O campo `CONTROLE` é metadado estrutural da ficha: define quem possui o ciclo de decisão daquele personagem e não é atributo mecânico.

Ferimentos, cansaço, condições temporárias, favores, acessos e relações circunstanciais não pertencem automaticamente à ficha permanente.

Antagonistas cuja ficha precise permanecer oculta durante o jogo não ficam aqui; usar `mestre/viloes/`.

O `personagens/README.md` deve deixar essa separação explícita.

### `mestre/`
Área reservada ao narrador para informação que deve existir de forma persistente sem ser apresentada ao jogador antes de ser descoberta na ficção.

Ela **não é tecnicamente privada** para o proprietário do repositório. “Reservada” significa que o narrador ou outra IA não deve expor espontaneamente seu conteúdo durante o RPG.

A subpasta padrão:

```text
mestre/viloes/
```

pode guardar fichas completas de antagonistas importantes, recorrentes ou poderosos quando suas capacidades, objetivos ou segredos precisarem de continuidade própria.

Regras:
- inimigos comuns não exigem arquivo individual;
- um vilão importante pode receber ficha completa antes de aparecer diretamente;
- o narrador pode consultar essa ficha durante a sessão;
- informações ocultas não devem ser reveladas ao jogador até o protagonista descobri-las de forma plausível;
- uma capacidade já definida não deve ser alterada retroativamente apenas para contrariar o jogador ou recuperar dificuldade perdida;
- mudanças posteriores na ficha precisam nascer de acontecimentos reais da ficção.

Se um antagonista deixar de exigir sigilo, sua ficha pode continuar em `mestre/viloes/` ou ser migrada para `personagens/` quando isso melhorar a organização.

`mestre/README.md` e `mestre/viloes/README.md` devem existir desde a criação da campanha para lembrar outra IA de que essa área é reservada e de como usá-la sem vazar metaconhecimento.

### `mundo/`
Contém regras e fatos específicos do cenário:
- lugares;
- organizações;
- cosmologia;
- regras sobrenaturais locais;
- tecnologia;
- limitações específicas;
- fatos que personagens podem descobrir.

`mundo/cenario.md` deve se concentrar na realidade do mundo. Tom literário, ritmo, tratamento de romance, humor ou outras escolhas de experiência pertencem a `diretrizes/narracao.md`.

O ponto inicial da história não pertence a `mundo/`. A situação concreta aprovada antes da primeira cena fica em `estado/inicio.md`.

Uma regra específica do mundo não deve ser promovida automaticamente a regra universal do sistema.

### `relacionamento/`
Usar para vínculos Centrais ou complexos que precisem de mais contexto do que um valor `REL` consegue representar.

O arquivo pode registrar:
- natureza do vínculo;
- evolução;
- desejos conflitantes;
- limites;
- acontecimentos que mudaram a relação;
- trajetórias planejadas, sempre separando plano de fato ocorrido.

Relações circunstanciais que ainda podem voltar a importar, mas não fazem parte da vida recorrente do personagem, podem permanecer em `progressao/` em vez de poluir a ficha ou criar um arquivo de relacionamento dedicado.

### `progressao/`
Guarda **consequências duradouras que ainda possuem potencial causal futuro**, conforme `sistema/progressao-narrativa.md`.

Não é XP, lista de conquistas nem arquivo de tudo que aconteceu.

Pode registrar:
- relações circunstanciais relevantes;
- favores e dívidas;
- acessos conquistados ou perdidos;
- recursos ou grupos acionáveis;
- posições, títulos ou autoridade;
- restrições;
- promessas;
- inimigos e ameaças latentes;
- reputações locais quando ainda puderem produzir efeito;
- outras consequências antigas que possam voltar a mudar uma cena futura.

Exemplos:

```text
- Princesa Elara ficou favorável ao personagem [+2] após o resgate; relação circunstancial, fora da ficha.
- Acesso liberado ao Mercado de Armas de Karsk.
- Rei Alaric deve um favor importante.
- Corvos Cinzentos aceitam contratos do personagem.
- Capitão dos Corvos passou a odiá-lo [-2].
- Trigon passou a considerá-lo um inimigo pessoal.
```

Uma consequência pode permanecer adormecida por muitos capítulos e voltar quando houver motivo, oportunidade e agência para isso.

> **Progressão é memória útil do que ainda pode voltar a importar.**

### `cronologia/`
Índice rápido do que aconteceu.

Para cada acontecimento relevante, registrar quando possível:
- capítulo;
- dia/período relativo;
- local;
- personagens presentes;
- fato;
- consequência;
- informação que cada personagem passou a conhecer.

A cronologia ajuda o narrador a evitar conhecimento impossível e contradições de continuidade.

A diferença principal é:

> **Cronologia registra o que aconteceu. Progressão destaca o que ainda continua causalmente vivo.**

### `estado/inicio.md`
É o **marco inicial aprovado** da aventura.

Guarda a situação concreta exatamente antes da primeira cena:
- onde os personagens estavam;
- qual situação imediata existia;
- qual era o objetivo ou gatilho inicial;
- qual era o ponto em que o jogador receberia controle.

Depois que a campanha começa, `estado/inicio.md` não acompanha o avanço da história e não deve ser sobrescrito a cada capítulo. Ele permanece como referência canônica do ponto de partida.

Se uma correção de continuidade alterar retroativamente o próprio começo da campanha, corrigir `estado/inicio.md` de forma explícita; fora disso, tratá-lo como marco histórico estável.

> **`estado/inicio.md` responde “onde esta história começou?”.**

### `estado/atual.md`
É o **savegame operacional** da aventura.

Ele não substitui fichas, Progressão nem capítulos. Guarda apenas como as coisas estão no momento exato em que a história parou.

Para personagens Centrais e Relevantes, pode registrar:
- VIDA atual;
- ENERGIA atual;
- CONDIÇÕES;
- danos temporários de equipamento;
- efeitos ativos;
- localização;
- situação imediata.

Exemplo:

```text
## Peter Parker
VIDA: Ferido
ENERGIA: Metade
COND: costela machucada
Local: telhado do laboratório
Efeito ativo: nenhum
```

Informação operacional que precise continuar secreta não deve ser colocada num `estado/atual.md` que a aventura trate como fonte apresentável ao jogador; mantê-la na área reservada do narrador quando necessário.

> **`estado/atual.md` responde “onde esta história está agora?”.**

O `estado/README.md` deve explicar desde o começo a diferença entre `inicio.md` e `atual.md`.

### `livro/`
Contém o registro canônico consolidado do que realmente aconteceu, em capítulos ou outra forma narrativa definida pelas diretrizes da aventura.

O material jogado é matéria-prima; o capítulo consolidado é o registro principal dos fatos quando a aventura adotar esse modelo.

## FICHA x STATUS x PROGRESSÃO

### FICHA
É referência estável do personagem.

Guarda características relativamente permanentes:
- identidade;
- descrição e personalidade;
- atributos;
- perícias;
- poderes;
- equipamento recorrente importante;
- relações recorrentes que realmente façam parte de sua vida atual.

### STATUS
É memória operacional de curto prazo.

Guarda:
- Vida;
- Energia;
- Condições;
- efeitos temporários;
- danos temporários;
- situação imediata.

### PROGRESSÃO
É memória de consequências que podem atravessar o tempo sem precisar ocupar a ficha.

Guarda aquilo que:
- nasceu de acontecimentos reais;
- continua válido;
- pode voltar a alterar escolhas, acessos, reações, ameaças ou oportunidades;
- não precisa estar ativo na cena atual.

> **Ficha = quem o personagem é. Status = como ele está agora. Progressão = o que sua vida deixou para trás e ainda pode voltar a importar.**

## Quando mostrar STATUS ao jogador

O narrador deve mostrar/atualizar STATUS:
- quando houver mudança importante de Vida;
- quando Energia mudar de faixa;
- quando surgir ou desaparecer uma condição relevante;
- quando uma consequência temporária mudar substancialmente as opções do personagem;
- sempre que o jogador pedir `status, narrador` ou equivalente.

Não repetir STATUS a cada ação se nada importante mudou.

Para Figurantes e inimigos comuns, normalmente basta acompanhar narrativamente enquanto permanecerem na cena; não é necessário persistir cada detalhe nem criar arquivo individual.

## Quando alterar a ficha permanente

A ficha **não evolui por XP, missões concluídas, tempo jogado ou recompensa automática**.

Ela permanece estável por padrão.

Só deve ser alterada quando a própria ficção realmente mudou o personagem, por exemplo:
- transformação corporal permanente;
- aquisição ou perda real de uma capacidade;
- remoção permanente de um poder;
- aprendizado efetivamente estabelecido pela história quando isso for parte concreta da ficção;
- mudança estrutural de identidade ou personalidade sustentada por acontecimentos;
- uma relação circunstancial passou a integrar de fato a vida recorrente do personagem.

Isso não é progressão mecânica. É atualização de continuidade.

O campo `CONTROLE` é exceção a essa lógica de evolução ficcional: ele não muda por acontecimentos normais da história e só deve ser alterado por decisão explícita do usuário.

Uma relação direcional deve ser alterada somente na ficha de quem mudou, e apenas quando aquele vínculo merecer acompanhamento recorrente. Relações circunstanciais podem continuar em `progressao/`.

> **A ficha muda quando o personagem mudou, não porque a história decidiu premiá-lo.**

Para fichas reservadas em `mestre/viloes/`, vale a mesma regra: não alterar capacidades estabelecidas apenas porque o jogador encontrou uma solução eficaz.

## O que entra na Progressão

Ao encerrar uma cena, capítulo ou arco, perguntar:

> **O que aconteceu aqui que ainda pode alterar uma decisão, oportunidade, relação, acesso, obrigação, ameaça ou reação futura?**

Registrar apenas isso.

Não registrar automaticamente:
- toda pessoa que ficou irritada;
- todo figurante ferido;
- todo elogio;
- toda pequena dívida social;
- fatos já encerrados sem futuro plausível.

Exemplo:

> `Mercenário aleatório ficou irritado porque teve o pé quebrado.`

normalmente não merece Progressão.

Mas:

> `Darek, líder de uma companhia mercenária, sobreviveu à humilhação e jurou vingança.`

pode merecer, mesmo que só volte a importar centenas de capítulos depois.

Se Darek passar a exigir capacidades e objetivos próprios de forma persistente, o narrador pode criar sua ficha reservada em `mestre/viloes/` sem transformar todo inimigo menor em personagem arquivado.

## Fechamento de capítulo

Ao encerrar um capítulo ou bloco canônico:

1. Consolidar em `livro/` somente os acontecimentos realmente válidos.
2. Remover comandos, correções fora da história, tentativas descartadas e versões substituídas.
3. Atualizar `cronologia/` com fatos e conhecimentos relevantes.
4. Atualizar `progressao/` com consequências que ainda possam produzir efeito futuro e remover/arquivar as que foram encerradas.
5. Atualizar fichas somente quando a própria ficção tiver alterado de forma real e duradoura o personagem.
6. Atualizar arquivos de `relacionamento/` quando houver evolução complexa importante de vínculos recorrentes.
7. Sobrescrever `estado/atual.md` com o ponto exato de continuação.
8. Remover do STATUS condições que já terminaram.
9. Atualizar material em `mestre/` somente quando fatos ou consequências reais tiverem alterado aquilo que o narrador precisa acompanhar em segredo.

`estado/inicio.md` **não é atualizado no fechamento normal de capítulo**. Ele continua preservando o ponto inicial aprovado da campanha.

Os `README.md` estruturais também não são registros de sessão e normalmente não precisam mudar em cada fechamento. Atualizá-los apenas quando a própria função ou organização da pasta mudar.

## Hierarquia de cânone

Cada aventura deve definir sua própria hierarquia no `README.md`.

Como padrão recomendado:

1. correção explícita mais recente do usuário;
2. capítulos consolidados em `livro/`;
3. diretrizes canônicas da aventura;
4. material reservado do narrador em `mestre/`, quando aplicável;
5. personagens, mundo e relacionamentos consolidados;
6. progressão narrativa vigente;
7. cronologia;
8. `estado/atual.md` para o estado operacional presente;
9. material antigo ou rascunho apenas como referência.

`estado/inicio.md` é a referência canônica específica para reconstruir o **ponto de partida aprovado** da campanha. Ele não compete com `estado/atual.md` sobre o presente e não deve ser usado para desfazer acontecimentos posteriores.

Material em `mestre/` pode definir verdades ainda desconhecidas pelo protagonista, mas não pode contradizer fatos já consolidados em fontes superiores nem ser reescrito retroativamente para vencer o jogador.

`estado/atual.md` é autoridade sobre o **agora**, mas não pode contradizer um fato canônico sem que exista um acontecimento posterior que explique a mudança.

`progressao/` é autoridade prática sobre consequências ainda vivas, mas não pode inventar fatos que não existam no livro, cronologia ou demais fontes canônicas.

Os `README.md` estruturais descrevem **organização**, não acontecimentos. Eles não têm prioridade para contradizer conteúdo canônico; sua função é orientar onde cada tipo de informação deve ser encontrado.

## Continuação em outro chat

Para retomar uma campanha sem contexto anterior:

1. ler o sistema universal;
2. ler o `README.md` da aventura;
3. consultar os `README.md` estruturais das áreas que forem necessárias para compreender onde cada informação está;
4. ler `diretrizes/narracao.md` e outras diretrizes indicadas;
5. ler as fichas dos personagens presentes ou centrais;
6. consultar `mestre/` silenciosamente quando houver antagonistas ou segredos relevantes para a continuação;
7. consultar relações e mundo relevantes;
8. consultar a Progressão relevante para personagens, locais e organizações envolvidos;
9. ler a cronologia suficiente para entender a situação;
10. ler `estado/atual.md`;
11. consultar o último capítulo consolidado quando necessário;
12. consultar `estado/inicio.md` apenas quando for necessário reconstruir ou conferir o ponto de partida original;
13. só então continuar a narrativa.

Ao consultar `mestre/`, outra IA deve usar a informação para manter continuidade **sem apresentá-la ao jogador como conhecimento do protagonista**.

> **Nunca depender de “lembrar da conversa anterior” quando os arquivos da aventura existem.**
