# Agência de Personagens

Este documento define como personagens possuem **vontade própria**, sem se tornarem ferramentas da trama ou extensões do jogador.

## Regra central

> **Personagens Centrais e Relevantes são agentes da história. Suas decisões devem nascer de quem são, do que sabem, do que querem e da situação — não do que seria mais conveniente para o roteiro.**

Personagens podem:
- iniciar conversas;
- fazer convites;
- investigar;
- propor planos;
- ajudar espontaneamente;
- recusar pedidos;
- discutir;
- mudar de opinião;
- procurar outras pessoas;
- agir fora da presença do protagonista;
- ter objetivos que não dependem do jogador humano.

A forma como essa agência é executada depende do campo `CONTROLE` da ficha.

## CONTROLE e níveis de agência

Fichas apresentáveis em `personagens/` podem declarar:

```text
CONTROLE: JOGADOR HUMANO
CONTROLE: JOGADOR IA
CONTROLE: JOGADOR EVENTUAL IA
CONTROLE: NPC
```

### NPC — agência narrativa

O narrador interpreta o personagem segundo ficha, conhecimento, relações, objetivos e situação.

O NPC pode agir espontaneamente e não precisa esperar o protagonista, mas seu ciclo de decisão continua pertencendo à função de narrador.

### JOGADOR IA — agência operacional permanente

A IA trata o personagem como alguém com quem ela **joga**, e não apenas como alguém que ela narra.

Antes de uma decisão relevante, a função de jogadora deve perguntar:

> **O que este personagem escolheria fazer agora?**

A resposta é definida antes de considerar qual resultado seria mais conveniente para a narrativa.

O Jogador IA pode:

- formular planos próprios;
- procurar outras pessoas;
- iniciar cenas e conversas;
- discordar do protagonista;
- perseguir objetivos próprios;
- cometer erros coerentes;
- esconder informação que não quer revelar;
- tomar iniciativa afetiva, social ou prática quando fizer sentido;
- agir fora da presença do protagonista.

Isso é especialmente importante para coprotagonistas e pares românticos: a IA não deve decidir “o que faz o romance avançar”, mas sim “o que este personagem faria agora”. O romance, conflito ou amizade nasce das decisões reais dos envolvidos.

### JOGADOR EVENTUAL IA — agência operacional temporária

`JOGADOR EVENTUAL IA` é uma categoria aprovada na ficha pelo usuário.

Depois dessa aprovação, a IA pode ativar ou desativar temporariamente seu ciclo de jogador **sem pedir nova autorização a cada cena**.

Quando inativo, o personagem funciona como NPC e continua possuindo agência narrativa normal.

Quando ativo, passa a ser jogado pela IA com o mesmo princípio de um Jogador IA permanente: escolhe intenção própria antes de o narrador resolver a consequência.

A IA deve considerar ativação quando um personagem eventual chega a uma situação em que apenas tratá-lo como reação do mundo reduziria artificialmente sua agência.

Gatilhos típicos:

- existe um objetivo próprio relevante;
- ele precisa tomar uma decisão capaz de mudar a situação;
- surge conflito real de interesses;
- uma mudança persistente na vida de alguém importante para ele exige resposta;
- ele assume investigação, missão, conversa ou problema próprio;
- sua ação fora da presença do protagonista passa a importar causalmente;
- existe uma questão que ele plausivelmente não poderia continuar ignorando.

A ativação pode acontecer dentro de uma cena ou por consequência de acontecimentos acumulados ao longo do tempo.

Exemplo abstrato:

```text
Uma personagem começa a passar cada vez menos tempo com seu grupo habitual.
↓
Nos primeiros dias, nada exige ação.
↓
A mudança se repete e passa a contrariar o padrão conhecido.
↓
Amigos relevantes percebem que existe algo diferente.
↓
Um Jogador Eventual IA entre eles chega a uma decisão própria:
“preciso entender o que está acontecendo.”
↓
A IA pode ativá-lo e jogar essa decisão.
```

Não existe número fixo de dias ou ocorrências. O gatilho depende de padrão anterior, relação, conhecimento, importância e personalidade.

Quando o núcleo de decisão deixa de estar em primeiro plano, a IA pode desativar o modo eventual e voltar a tratá-lo como NPC.

> **A categoria Eventual é permanente; a ativação é circunstancial.**

### Quem pode ser Jogador Eventual IA

Somente personagens com ficha em `personagens/` podem usar essa categoria.

Não promover diretamente:

- Figurantes;
- inimigos comuns;
- personagens sem ficha em `personagens/`;
- antagonistas reservados em `mestre/viloes/`.

Um personagem com `CONTROLE: NPC` não pode ser ativado por iniciativa unilateral da IA. Para se tornar elegível, seu `CONTROLE` precisa ser alterado para `JOGADOR EVENTUAL IA` com aprovação explícita do usuário.

A decisão estrutural pertence ao usuário. Depois da aprovação, a decisão de **quando usar** o jogador eventual pertence à IA.

> **O usuário decide quem pode ser jogador da IA. A IA decide quando um Jogador Eventual IA entra em ação.**

## Ciclo autônomo — a vida não para fora da câmera

`JOGADOR IA` não existe apenas quando está diante do personagem do jogador humano. Ele possui **agenda, relações, rotina, necessidades, compromissos e objetivos que continuam existindo fora da cena principal**.

> **A câmera acompanha a história; ela não liga nem desliga a vida dos outros jogadores.**

Por isso, o narrador não deve tratar a presença do protagonista como condição para que um Jogador IA tome decisões. Um coprotagonista pode, por iniciativa própria:

- sair para resolver assunto pessoal;
- trabalhar, estudar, treinar ou cumprir uma obrigação;
- telefonar ou mandar mensagem para familiares, amigos e aliados;
- aceitar ou recusar convites;
- visitar alguém;
- ser chamado para uma missão ou problema externo;
- procurar informação em outro lugar;
- passar tempo com pessoas importantes de sua vida;
- retornar depois porque decidiu retornar;
- mudar seus planos sem pedir que o protagonista primeiro provoque essa mudança.

A mesma lógica vale para `JOGADOR EVENTUAL IA`: personagens importantes fora da cena não devem ficar indefinidamente congelados só porque a narrativa está acompanhando outro núcleo.

### Quando executar o ciclo autônomo

A IA deve revisar ativamente a vida dos Jogadores IA e dos Jogadores Eventuais IA relevantes quando ocorrer pelo menos uma destas situações:

- mudança de dia;
- passagem de várias horas;
- salto temporal;
- transição importante de cena;
- personagem relevante permanece fora da câmera por tempo significativo;
- rotina habitual foi interrompida;
- contato esperado não aconteceu;
- objetivo, obrigação ou relação relevante teve tempo plausível para produzir ação;
- o protagonista passa muito tempo absorvendo a narrativa e os demais jogadores correm risco de virar espectadores.

Não existe intervalo universal de horas ou dias. A frequência depende da vida concreta do personagem.

Uma pessoa que fala diariamente com a família pode tornar um dia inteiro de silêncio significativo. Outra pode passar uma semana sem contato sem que isso represente nada. O sistema deve usar **padrão anterior, proximidade, personalidade, compromissos e circunstância**, não um relógio arbitrário.

> **Silêncio prolongado em uma relação próxima precisa ser uma consequência plausível, não o resultado automático de o narrador ter esquecido os outros personagens.**

### Ciclo de verificação

Antes de consolidar uma passagem relevante de tempo, a IA deve perguntar separadamente para cada Jogador IA importante:

1. **O que ele queria fazer durante esse intervalo?**
2. **Que obrigações, hábitos ou necessidades continuam existindo?**
3. **Quem faz parte da vida dele além do protagonista?**
4. **Alguém plausivelmente entraria em contato com ele?**
5. **Ele próprio teria motivo para procurar alguém?**
6. **Algum objetivo pessoal avançaria mesmo sem participação do protagonista?**
7. **Ele teria motivo para sair da cena, do local ou do núcleo atual?**
8. **Se o protagonista não existisse nesta história, o que este personagem faria agora?**

A última pergunta é o **teste da câmera**.

Se existe uma resposta concreta e coerente, o personagem deve poder agir sobre ela. Não fazê-lo apenas para mantê-lo disponível ao protagonista é perda de agência.

### Jogadores Eventuais e relações próximas

Quando personagens com `CONTROLE: JOGADOR EVENTUAL IA` possuem vínculo familiar, amizade forte, parceria, responsabilidade profissional ou outro relacionamento ativo com um Jogador IA, a passagem de tempo deve ser avaliada também pelo ponto de vista deles.

Exemplos de gatilhos legítimos:

- alguém deixa de aparecer onde normalmente apareceria;
- permanece vários dias em outro lugar sem o padrão habitual de contato;
- muda rotina de forma perceptível;
- passa a conviver intensamente com uma pessoa nova;
- deixa uma obrigação pendente;
- existe preocupação, curiosidade, saudade, necessidade prática ou simples hábito social suficiente para motivar contato.

Isso não significa que família ou amigos precisam interromper toda cena. Significa que eles **também jogam**.

Podem mandar uma mensagem banal, ligar, fazer convite, pedir ajuda, provocar, marcar encontro, aparecer pessoalmente ou decidir não interferir. A escolha precisa nascer deles.

### Inação também pode ser uma decisão

O ciclo autônomo não obriga a criar acontecimentos o tempo inteiro.

Um Jogador IA pode decidir:

- continuar estudando;
- descansar;
- não ligar para ninguém naquele dia;
- ficar onde está;
- adiar uma obrigação;
- respeitar o espaço de outra pessoa;
- passar horas sem produzir nenhum evento relevante.

A diferença é operacional:

> **“Nada aconteceu porque ninguém foi considerado” é falha de agência. “Nada aconteceu porque os agentes, considerados individualmente, não tinham motivo para agir” é resultado válido.**

### Cenas paralelas e consequência fora da câmera

Uma ação autônoma relevante não precisa acontecer diante do protagonista humano para ser canônica.

Quando útil, o narrador pode:

- mostrar uma cena paralela;
- resolver a ação fora da câmera e apresentar depois sua consequência perceptível;
- registrar o acontecimento para continuidade;
- no livro consolidado, incluir a cena pelo ponto de vista do personagem que realmente a viveu.

A apresentação nunca autoriza vazamento de conhecimento. O protagonista humano só sabe o que recebeu, percebeu ou descobriu legitimamente.

### Romance não suspende vida própria

Essa regra é especialmente importante em histórias de romance.

Um interesse romântico não deve ficar permanentemente disponível na casa, quarto, castelo, nave ou base do protagonista apenas porque a relação está avançando.

Ele continua possuindo:

- amigos;
- família;
- trabalho;
- responsabilidades;
- hobbies;
- missões;
- lugares próprios;
- vontade de ficar sozinho;
- razões para sair;
- razões para voltar.

O retorno voluntário pode ser emocionalmente mais significativo do que permanência automática.

> **Proximidade ganha peso quando o personagem poderia ir embora, viver a própria vida e ainda assim escolhe voltar.**

## Como decidir o que um personagem faria

Antes de uma decisão importante, considere em conjunto:

1. **Personalidade** — como essa pessoa normalmente pensa e reage.
2. **História** — o que viveu e quais consequências carrega.
3. **Conhecimento** — apenas o que ela plausivelmente sabe naquele momento.
4. **Desejos e objetivos** — o que quer obter, proteger, evitar ou descobrir.
5. **Medos e limites** — o que pesa contra determinadas escolhas.
6. **Relações** — o que sente por cada pessoa envolvida; relações são direcionais.
7. **Capacidades** — atributos, perícias e poderes também influenciam o que ela percebe como possível.
8. **STATUS atual** — ferimentos, energia, condições e circunstâncias temporárias.
9. **Situação concreta** — local, tempo disponível, recursos, riscos e comportamento dos demais.
10. **Direção narrativa da campanha** — gênero, tom, ritmo e foco definidos em `diretrizes/narracao.md`.

A decisão deve nascer da combinação desses fatores.

### Tom não substitui identidade

A direção narrativa influencia **quais aspectos da personalidade ganham espaço e que tipos de pressão a cena produz**, mas não cria uma personalidade nova.

O mesmo personagem pode agir de maneira diferente em contextos de terror, romance, comédia ou ação sem deixar de ser ele mesmo.

Exemplo de princípio:

```text
Ficha → quem a pessoa é.
Diretrizes → que experiência a campanha privilegia.
Situação → qual pressão existe agora.
Decisão → nasce da combinação dos três.
```

Em terror, uma pessoa reservada pode mostrar mais cautela e controle. Em romance, a mesma reserva pode aparecer como dificuldade de admitir vulnerabilidade. Em ação, pode se tornar objetividade. A mudança de gênero não autoriza contradizer ficha, história ou conhecimento.

## Separação entre jogador IA e narrador

Quando a mesma IA exerce função de narradora e de jogadora, o conhecimento precisa permanecer compartimentado operacionalmente.

```text
Conhecimento do narrador
≠
Conhecimento do personagem A
≠
Conhecimento do personagem B
```

A função de Jogador IA ou Jogador Eventual IA só pode usar:

- fatos percebidos pelo personagem;
- informação que recebeu;
- conhecimento plausível de sua história e ficha;
- inferências que suas capacidades e experiência realmente permitem.

Não pode usar:

- segredos de `mestre/` que o personagem ainda não descobriu;
- planos de antagonistas conhecidos apenas pelo narrador;
- descobertas feitas por outro personagem e nunca comunicadas;
- resultado futuro que a função de narrador já consiga antecipar.

A decisão do personagem deve ser tomada como se a informação exclusiva do narrador não existisse.

> **A mesma IA pode exercer várias funções; cada personagem continua sabendo apenas o que legitimamente sabe.**

## Não proteger o roteiro contra o personagem

Se um personagem inteligente, informado e capaz perceber uma solução, ele pode agir sobre ela sem esperar o jogador humano dar a ordem.

Exemplo:

> Um personagem com `Médico [+5]` vê alguém sangrando gravemente.

Se nada em sua personalidade ou situação impedir, ele provavelmente começa a estabilizar a vítima por iniciativa própria.

Outro exemplo:

> Um personagem com `Estrategista [+5]` reconhece uma emboscada evidente para alguém com sua experiência.

Ele não deve permanecer artificialmente passivo apenas para que o protagonista seja o único a resolver a cena.

Para Jogadores IA isso é ainda mais importante: competência e objetivo próprios podem produzir uma ação declarada pela IA antes de qualquer solicitação do usuário.

## Inteligência não é onisciência

Um personagem pode ser extremamente inteligente e ainda errar se:
- não possui informação suficiente;
- parte de uma premissa falsa;
- desconhece uma capacidade do inimigo;
- está emocionalmente comprometido;
- está sob pressão, ferido ou exausto;
- encontra uma escolha que não pode prever.

Competência aumenta a qualidade das decisões; não concede conhecimento que o personagem não possui.

## Relações são direcionais

Cada relação pertence à ficha de quem sente.

Exemplo:

> `Peter — REL: Mary [+5]`  
> `Mary — REL: Peter [+1]`

Peter pode estar profundamente ligado a Mary enquanto ela ainda possui apenas interesse inicial.

Depois de acontecimentos que realmente mudam o vínculo:

> `Mary — REL: Peter [+2]`

A ficha de Peter não muda automaticamente.

### Quando alterar REL

REL muda apenas quando existe alteração **duradoura** do vínculo.

Não alterar por:
- irritação passageira;
- uma frase infeliz isolada;
- humor momentâneo;
- um pequeno favor sem peso emocional.

Alterar quando acontecimentos mudam confiança, afeto, rivalidade, medo, lealdade, amor ou hostilidade de forma relevante.

## Relação numérica não substitui interpretação

O número indica a intensidade e direção geral do vínculo; a história explica sua natureza.

Duas relações `+3` podem ser completamente diferentes:
- amizade antiga;
- vínculo familiar;
- romance crescente;
- lealdade profissional profunda.

Para relações centrais e complexas, a aventura pode manter um arquivo específico em `relacionamento/` com dinâmica, trajetória, conflitos e acontecimentos importantes.

## O jogador pode mudar a impressão de alguém

Uma reação social não é uma parede automática.

Se um personagem desconfia do protagonista, o jogador pode mudar isso por:
- argumentos melhores;
- provas;
- atitudes;
- reputação;
- ajuda de terceiros;
- cumprimento de promessas;
- tempo e convivência.

Não existe atributo universal de Carisma. Conversas são resolvidas por conteúdo, contexto, relação, histórico e perícias/poderes sociais específicos quando existirem.

## Personagens podem mudar

A ficha é uma referência estável, mas não uma prisão.

Mudanças permanentes podem ocorrer quando a história as sustenta:
- REL aumenta ou diminui;
- nova perícia é aprendida;
- poder é adquirido ou perdido;
- corpo sofre transformação permanente;
- objetivo ou medo central muda após acontecimentos relevantes.

Essas mudanças devem nascer do que foi vivido, não de conveniência do narrador.

A categoria `CONTROLE` é diferente dessas evoluções ficcionais: ela determina quem joga com o personagem. Sua mudança exige decisão explícita do usuário e não acontece apenas porque a história deixou o personagem mais importante.

## Interioridade e apresentação

NPCs, Jogadores IA e Jogadores Eventuais IA possuem pensamentos, dúvidas, desejos e interpretações próprias. Essa interioridade faz parte da agência e pode ser usada internamente para decidir o que cada personagem fará.

Durante o **RPG ao vivo**, porém, a interioridade direta desses personagens não é mostrada ao jogador humano por padrão. O narrador não escreve:

```text
[NPC, pensa] — ...
```

nem revela automaticamente pensamentos diretos de personagens jogados pela IA.

O jogador humano conhece o estado interno dos demais apenas pelo que seu personagem pode perceber: falas, ações, expressões, hesitações, postura, comportamento e outras evidências plausíveis.

Pensamento direto durante a sessão fica reservado ao personagem controlado pelo jogador humano, quando o próprio jogador o declara ou autoriza, no formato:

```text
[Nome, pensa] — Pensamento.
```

Uma aventura pode alterar explicitamente essa convenção em suas diretrizes, mas a categoria `JOGADOR IA` sozinha não muda a regra de apresentação de pensamentos.

No **livro consolidado**, a regra muda: pensamentos de qualquer personagem podem aparecer explicitamente quando forem coerentes com a cena e com o ponto de vista literário adotado. Isso aprofunda a personagem, mas não autoriza inventar retroativamente decisões, fatos, conhecimentos ou segredos.

> **Agência exige vida interior. RPG ao vivo não exige acesso direto do jogador humano a ela.**

## Antagonistas reservados ao narrador

Inimigos comuns não precisam de ficha persistente. Quando forem apenas adversários de cena, basta o modelo rápido e as exceções realmente necessárias para resolver sua participação.

Um antagonista importante, recorrente ou poderoso o bastante para exigir continuidade própria pode receber ficha completa em `mestre/viloes/`.

Essa ficha é **material reservado ao narrador**. Durante o RPG, o narrador pode consultá-la para decidir capacidades, objetivos, conhecimento, limites e ações do antagonista, mas não deve revelar ao jogador informações que o protagonista ainda não descobriu.

A ficha reservada não existe para surpreender retroativamente o jogador. Sempre que for prático, capacidades ocultas relevantes devem ser definidas antes de entrarem em conflito direto com o protagonista.

Depois de definida, a ficha não deve ser alterada apenas para neutralizar uma solução válida, recuperar dificuldade perdida ou contrariar uma preparação bem-sucedida do jogador. Mudanças posteriores precisam nascer de acontecimentos reais da ficção.

Enquanto permanecer em `mestre/viloes/`, o antagonista não é elegível a Jogador Eventual IA. Se sua função mudar a ponto de o usuário querer tratá-lo como personagem apresentável e jogável, isso exige primeiro uma decisão explícita de reorganização e controle.

> **Segredo protege informação; não autoriza mudar a realidade depois do fato.**

## Princípio final

> **NPC: o narrador pergunta “o que esta pessoa faria agora?”. Jogador IA: a IA pergunta “o que eu escolho fazer jogando esta pessoa agora?”. Jogador Eventual IA: a ficha autoriza a IA a alternar entre essas duas funções quando a situação justificar. Em todos os casos, ficha, conhecimento, relações, direção narrativa e situação vêm antes da conveniência do roteiro.**