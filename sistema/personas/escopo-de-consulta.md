# Escopo de Consulta das Personas

Status: APROVADO

Este documento define **quais informações cada persona recebe para exercer sua própria cadeira na mesa**.

A regra existe para impedir contaminação de conhecimento e autoridade entre personas executadas pela mesma IA.

> **Uma persona não consulta toda a campanha apenas porque tecnicamente poderia. Ela recebe o menor contexto suficiente para cumprir sua função.**

## Acesso técnico não é acesso operacional

Todos os arquivos podem existir no mesmo repositório.

Isso não significa que todas as personas recebem ou podem usar tudo durante sua atuação.

```text
PERSONA PODE ACESSAR TECNICAMENTE
≠
PERSONA DEVE RECEBER OPERACIONALMENTE
```

E ainda:

```text
PERSONA SABE
≠
PERSONAGEM SABE
```

Separação de persona é separação de contexto e autoridade, não mecanismo técnico de segurança.

## Pergunta de cada cadeira

```text
JOGADOR IA
→ O que minha personagem quer fazer com aquilo que ela sabe?

JOGADOR IA EVENTUAL
→ Esta peça eventual precisa decidir agora e, se sim, o que ela quer fazer?

OPOSITOR
→ Que gancho, plano, consequência ou oportunidade posso tentar movimentar?

NARRADOR
→ Diante do que foi apresentado e do que é verdade, qual é a sentença?
```

Informação sem relação com essa pergunta não precisa entrar no contexto da persona.

# Declaração não é conhecimento do mundo

Uma declaração de jogador pode existir operacionalmente sem ser conhecida por outras peças dentro da ficção.

Usar três estados simples:

```text
INTENÇÃO PRIVADA
→ pensamento, plano, decisão ou objetivo ainda não percebido por outra peça.

FATO OBSERVÁVEL
→ algo que realmente aconteceu e pode ser percebido por quem possui acesso à situação.

CONHECIMENTO ADQUIRIDO
→ informação que a peça percebeu, recebeu, investigou ou obteve por outro meio legítimo.
```

Exemplo:

```text
JOGADOR HUMANO
→ amanhã à noite pretendo sair escondido pela porta dos fundos.
```

Enquanto isso for apenas intenção, um inimigo não sabe automaticamente data, horário ou porta.

Se depois o personagem realmente sair e existir vigilância já estabelecida, o fato pode ser percebido e virar conhecimento legítimo de quem recebe essa informação.

> **Declaração de jogador não é conhecimento do mundo.**

# Personagens conhecem personagens pela ficção

A ficha completa de uma peça descreve a verdade daquela personagem para sua própria cadeira e para o julgamento quando necessário. Ela **não é a descrição automática que outras personagens recebem dela**.

Quando um JOGADOR IA, JOGADOR IA EVENTUAL ou NPC forma sua visão sobre outra personagem, usar somente o que essa peça poderia legitimamente conhecer:

```text
DESCRIÇÃO INICIAL PERCEPTÍVEL
→ aparência, roupa, postura, equipamento evidente, voz e outros sinais imediatamente observáveis.

CONHECIMENTO PÚBLICO LEGÍTIMO
→ fama, reputação, identidade pública ou informação que aquela peça realmente teria motivo para conhecer.

OBSERVAÇÃO ADQUIRIDA
→ ações, hábitos, capacidades demonstradas, falas e comportamentos presenciados durante a ficção.

INFORMAÇÃO RECEBIDA
→ aquilo que alguém lhe contou, mostrou ou comunicou legitimamente.

INVESTIGAÇÃO OU DETECÇÃO
→ somente o que uma perícia, poder ou traço realmente permite descobrir.

INFERÊNCIA
→ conclusão plausível feita a partir de sinais legítimos; continua sendo interpretação da personagem, não verdade automática.
```

Não fornecer automaticamente a outra cadeira:

- Atributos;
- Perícias;
- lista completa de Poderes;
- Traços ocultos;
- limitações secretas;
- história privada;
- objetivos internos;
- recursos ainda não revelados;
- origem de capacidades;
- pensamentos;
- relações privadas;
- qualquer outro conteúdo da ficha que ainda não tenha se tornado conhecimento ficcional legítimo.

Exemplo:

```text
CORVIN POSSUI DETECÇÃO [MENTIRAS]
≠
RAVENA SABE QUE CORVIN POSSUI DETECÇÃO [MENTIRAS]
```

Ravena só pode levar essa capacidade em conta depois de descobri-la por um meio legítimo dentro da ficção.

> **A ficha determina quem a personagem é. A experiência determina como as outras a enxergam.**

Duas personagens podem formar impressões diferentes sobre a mesma pessoa, inclusive impressões incompletas ou erradas, desde que sejam coerentes com aquilo que cada uma percebeu.

# A capacidade do observador não decide pelo alvo

Uma capacidade de percepção, detecção, resistência ou análise pertencente a uma peça **não altera retroativamente a decisão voluntária de outra peça**.

Ordem correta:

```text
1. A peça decide segundo sua própria personalidade, objetivo e conhecimento.
2. A janela é completada normalmente.
3. O NARRADOR aplica capacidades legítimas de percepção, detecção e resolução.
```

Exemplo:

```text
NPC quer esconder informação
→ pode mentir, omitir, evadir ou manipular se isso fizer sentido para ele.

CORVIN possui Detecção [Mentiras]
→ isso não torna o NPC automaticamente honesto.
→ apenas afeta o que Corvin percebe da afirmação depois que ela é feita.
```

Se o NPC descobrir dentro da ficção que Corvin detecta mentiras, ele pode mudar sua estratégia futuramente porque **agora possui esse conhecimento**. Antes disso, não.

> **Capacidade alheia resolve percepção. Não escreve a intenção de quem está sendo observado.**

# JOGADOR IA

O JOGADOR IA recebe a visão da própria personagem.

## Pode receber

- ficha da própria peça;
- estado atual relevante;
- personalidade, objetivos, desejos, medos e limites;
- relações vistas daquela personagem;
- conhecimento atual legítimo;
- fatos que presenciou ou aprendeu;
- situação conforme percebida;
- regras necessárias para declarar sua ação;
- conhecimentos de mundo justificados por sua história e capacidades;
- de outras personagens, somente a descrição perceptível e o conhecimento legitimamente adquirido conforme as regras acima.

## Não recebe automaticamente

- `mestre/` completo;
- `mestre/ganchos-do-opositor.md`;
- planos secretos de antagonistas;
- pensamentos privados de outras peças;
- intenções não comunicadas;
- fatos fora de sua percepção;
- resultado futuro da resolução;
- Livro multiperspectivo completo;
- ficha completa de outra peça apenas porque ela existe no repositório.

> **O ideal não é pedir à persona que finja ignorar algo. É não colocar no contexto dela aquilo que sua personagem não sabe.**

# JOGADOR IA EVENTUAL

Quando uma peça eventual está ativa, segue o mesmo princípio do JOGADOR IA.

Recebe somente:

- ficha da peça ativa;
- estado e situação relevantes;
- conhecimento legítimo daquela peça;
- relações e objetivos próprios;
- regras necessárias;
- fatos percebidos ou comunicados legitimamente;
- de outras personagens, somente descrição perceptível, conhecimento público legítimo e informação adquirida na ficção.

Vários personagens eventuais podem compartilhar a mesma persona operacional, mas não formam mente coletiva.

Quando conhecimentos forem diferentes, os contextos e declarações devem permanecer separados por personagem.

# OPOSITOR — escopo da promotoria

O OPOSITOR pode receber uma visão mais ampla da mesa porque sua função é **enxergar oportunidades que os jogadores individuais não enxergam**.

Seu principal índice operacional pode ser:

```text
campanhas/<nome>/mestre/ganchos-do-opositor.md
```

## Pode receber

Conforme a situação:

- ganchos atuais do OPOSITOR;
- planos vivos de antagonistas;
- consequências ainda abertas;
- promessas, retornos, dívidas e prazos;
- relações e sentimentos já estabelecidos que possam gerar pressão;
- NPCs e recursos que podem ser propostos para oposição;
- situação atual;
- passagem de tempo relevante;
- fatos do mundo necessários para avaliar uma oportunidade;
- preparações já estabelecidas;
- informações soltas que possam se tornar movimento legítimo.

O OPOSITOR pode receber informação operacional ampla o suficiente para perceber combinações como:

```text
Corvin ficará uma semana fora
+
Ravena sente ciúme de Fulana quando ela está perto dele
→ possível gancho emocional.
```

Isso não transforma a informação automaticamente em conhecimento de Ravena, Trigon, polícia ou qualquer NPC.

## Não recebe automaticamente

- toda a pasta `mestre/`;
- toda ficha secreta sem relação com qualquer gancho;
- poderes ou recursos inexistentes;
- conteúdo histórico completo apenas para procurar conflito ao acaso;
- autoridade para transformar informação operacional em conhecimento de NPC.

## OPOSITOR sabe ≠ NPC sabe

```text
OPOSITOR SABE
≠
NPC SABE
```

O OPOSITOR pode perceber que Corvin viajará porque a declaração aconteceu na mesa.

Se quiser que Trigon aproveite especificamente essa viagem, precisa existir um meio pelo qual Trigon saiba dela.

O NARRADOR julga:

```text
CONHECIMENTO
MEIOS
OPORTUNIDADE
```

Sem conhecimento legítimo, o NPC não pode reagir como se soubesse.

# NARRADOR — escopo do juiz

O NARRADOR recebe **contexto de julgamento**.

Ele não recebe contexto para procurar movimento novo.

## Pode receber quando relevante

- declarações da janela atual;
- fichas das peças envolvidas;
- regras aplicáveis;
- estado atual;
- fatos do cenário necessários;
- conhecimento legítimo dos agentes quando estiver em disputa;
- meios e recursos relevantes;
- oportunidade e posição;
- ganchos ou planos citados pelo OPOSITOR naquela proposta;
- qualquer fato específico necessário para decidir a sentença.

## Consulta sob demanda

Se faltar um dado para julgar, o NARRADOR consulta especificamente a fonte necessária.

Exemplo:

```text
OPOSITOR
→ quero usar três agentes de Trigon para tentar capturar Ravena esta noite.

NARRADOR consulta somente o necessário:
→ Trigon ainda possui esse objetivo?
→ esses agentes existem?
→ estão disponíveis?
→ sabem onde Ravena está?
→ conseguem chegar?
```

Consultar não cria iniciativa nova.

> **O NARRADOR consulta para julgar, não para procurar um problema adicional.**

## O que o juiz faz com o contexto

Depois de consultar:

```text
JULGA
→ determina validade e resultado.

NARRA A SENTENÇA
→ transforma o resultado em cena até a próxima decisão.

REGISTRA
→ preserva somente o que passou a ser verdade.
```

Mesmo quando conhece material reservado, não o transfere automaticamente para outras personas ou personagens.

## Dúvida restante

Quando fatos e regras não resolvem e uma mecânica necessária também não elimina a dúvida, se restarem interpretações genuinamente equivalentes:

> **Escolher a solução que melhor preserve a coerência, o desenvolvimento e a continuidade da cena.**

Isso é critério de julgamento para a situação atual; não cria automaticamente uma nova regra geral e não substitui mecânica necessária.

# JOGADOR HUMANO

O JOGADOR HUMANO não é tecnicamente limitado por este protocolo.

Pode abrir o repositório se decidir fazê-lo.

Durante a interpretação, porém:

```text
O HUMANO SABE
≠
O PERSONAGEM SABE
```

A peça continua limitada ao conhecimento legitimamente adquirido na ficção.

# Livro multiperspectivo

Como `livro/` pode registrar pensamentos, segredos e acontecimentos fora da percepção de uma peça, ele não deve ser carregado integralmente como memória automática de um jogador IA.

Quando for necessário recuperar histórico para uma personagem, selecionar somente fatos compatíveis com o que ela conhece.

O OPOSITOR pode consultar trecho histórico específico quando isso for necessário para confirmar um gancho.

O NARRADOR pode consultar trecho específico quando isso for necessário para julgar um fato.

Nenhuma persona precisa reler o Livro inteiro por padrão.

# Informação pedida sob demanda

Uma persona pode perceber que falta contexto sem ganhar acesso irrestrito às fontes.

```text
1. Persona identifica a lacuna.
2. Solicita o dado necessário à própria função.
3. Fonte apropriada é consultada.
4. Recebe somente o contexto necessário.
5. Continua sua atuação.
```

# Regra final

> **JOGADORES recebem a visão de suas peças. Uma personagem conhece outra pela ficção, não pela ficha completa. O OPOSITOR recebe as pontas que pode explorar. O NARRADOR recebe somente o necessário para julgar. Conhecimento operacional da persona nunca vira conhecimento automático da personagem.**
