# Status

Esta pasta reúne regras que descrevem o **estado atual do personagem** durante o jogo.

Diferente de Traços, que representam características permanentes ou duradouras, Status descreve condições ou consequências que estão acontecendo **agora** com o personagem e que podem mudar conforme a ficção.

## Escopo

As regras desta pasta serão construídas para abranger:

- **Vida** — quantidade de dano que o personagem consegue suportar e o que acontece quando sua Vida é reduzida.
- **Dano** — como ferimentos e outras consequências reduzem Vida.
- **Cura** — como Vida perdida pode ser restaurada e quais limites se aplicam.
- **Efeitos Básicos** — estados temporários ou consequências imediatas que alteram a situação do personagem.

Por enquanto, os Efeitos Básicos consolidados são apenas **efeitos nocivos**.

## Efeitos Nocivos

Os efeitos nocivos estão organizados por **famílias** em [`nocivos/`](nocivos/).

Cada família representa uma função reutilizável que pode ser causada por Poderes, perigos ou outras fontes do sistema.

### Progressão de Efeitos

Cada família organiza até **3 efeitos relacionados em uma progressão**.

A progressão representa resultados possíveis dentro da mesma categoria de efeito. Ela **não é uma sequência obrigatória de estados** e um efeito anterior não precisa ser aplicado antes de um efeito posterior.

Ao tentar produzir um efeito mais avançado da família, a resolução pode resultar em um efeito anterior da mesma progressão.

Exemplo:

**Posição: Caído → Movido → Conduzido**

Uma tentativa de **Conduzir** pode resultar apenas em **Movido**, enquanto uma tentativa de **Mover** pode resultar apenas em **Caído**.

Da mesma forma, em **Influência**, uma tentativa de **Dominar** pode resultar apenas em **Compelido** ou **Enfeitiçado**, conforme a resolução.

Um mesmo estado pode aparecer em mais de uma família quando cumprir exatamente a mesma função, sem receber uma nova definição mecânica apenas por estar em outra progressão.

### Sobreposição entre efeitos

Cada família de Status é resolvida **separadamente**.

> **Em cada família, apenas o melhor efeito fica ativo. Famílias diferentes coexistem normalmente.**

Assim, vários efeitos podem estar presentes ao mesmo tempo desde que pertençam a famílias diferentes.

Exemplo: um personagem pode sofrer ao mesmo tempo o melhor efeito de **Aflição** aplicável a ele e o melhor efeito de **Contenção** aplicável a ele. Um não substitui nem desativa o outro porque pertencem a famílias diferentes.

Quando dois ou mais efeitos pertencem à **mesma família**, apenas o efeito mais forte fica ativo.

- se dois efeitos tiverem a mesma força, permanece o de maior duração;
- **durações não se somam**: receber várias aplicações do mesmo efeito não acumula suas durações;
- uma nova aplicação pode **renovar a duração** do mesmo efeito: compare a duração restante com a duração completa da nova aplicação e mantenha a maior;
- se o efeito mais fraco possuir duração menor ou igual à do mais forte, ele é descartado;
- se o efeito mais fraco possuir duração maior, ele fica inativo enquanto o mais forte estiver ativo e sua duração continua passando normalmente;
- quando o efeito mais forte terminar, o mais fraco volta a valer se ainda restar duração.

Exemplo: receber **Cego [Cena]** dez vezes, mesmo de dez fontes diferentes, continua resultando apenas em **Cego [Cena]**. As dez aplicações não se transformam em dez Cenas de duração.

Exemplo: um personagem está sob **Cego [Hora]** e falta apenas 1 minuto para o efeito terminar. Se receber novamente **Cego [Hora]**, a duração volta para **1 hora**. A nova duração substitui a duração restante porque é maior; ela não é somada ao tempo que ainda faltava.

Exemplo: **Paralisado** domina **Imóvel** e **Lento** por pertencerem todos à família Contenção. Porém um efeito de **Aflição** continua ativo normalmente ao mesmo tempo, pois pertence a outra família.

A fonte do efeito não muda essa regra: efeitos da mesma família competem entre si mesmo quando vierem de fontes diferentes.

As famílias atuais são:

- **[Sentidos](nocivos/sentidos.md)** — Ofuscado; Cego, Surdo ou Mudo; Privado.
- **[Contenção](nocivos/contencao.md)** — Lento; Imóvel; Paralisado.
- **[Terror](nocivos/terror.md)** — Abalado; Apavorado; Aterrorizado.
- **[Exaustão](nocivos/exaustao.md)** — Fatigado; Exausto; Inconsciente.
- **[Perturbação](nocivos/perturbacao.md)** — Desorientado; Confuso; Atordoado.
- **[Aflição](nocivos/aflicao.md)** — 1 de dano; 1d3 de dano; 1d6 de dano por turno.
- **[Posição](nocivos/posicao.md)** — Caído; Movido; Conduzido.
- **[Influência](nocivos/influencia.md)** — Enfeitiçado; Compelido; Dominado.
- **[Ruína](nocivos/ruina.md)** — Desprevenido; Exposto; Indefeso.
- **[Debilitação](nocivos/debilitacao.md)** — Fraco; Debilitado; Prostrado.

## Como interpretar um Efeito

Cada efeito deve dizer principalmente:

1. **Efeito mecânico** — uma indicação objetiva quando uma pincelada mecânica for necessária.
2. **Efeito narrativo** — a base ficcional do que aconteceu com o personagem.
3. **Remoção** — o que encerra ou remove o efeito quando isso fizer parte de sua própria definição.

As regras são uma **base para o Narrador construir a ficção**, com mecânicas apenas onde elas ajudam a resolver a incerteza.

Um efeito não precisa listar todas as consequências possíveis. Se uma consequência for evidente pela própria situação, ela é resolvida pela ficção. As regras não devem criar exceções para cada consequência de estar cego, imóvel, atordoado, indefeso ou sob qualquer outro efeito.

Da mesma forma, um efeito não determina automaticamente como uma personagem reage, salvo quando sua própria definição estabelece uma impossibilidade ou controle específico. A agência continua sendo respeitada.

## Limites desta pasta

Esta pasta **não define por enquanto**:

- como um Poder aplica um efeito;
- qual Atributo é usado para resistir;
- custo de Mana;
- alcance, área ou quantidade de alvos;
- duração geral de efeitos.

Essas regras pertencem aos capítulos apropriados do sistema.

## Princípios

1. Status descreve o que está acontecendo **agora** com o personagem.
2. Traços descrevem aquilo que o personagem **é, possui ou carrega como característica**.
3. Poderes e outras regras podem criar, remover ou modificar efeitos, mas não substituem suas definições.
4. A ficção vem antes da exceção mecânica: resultados evidentes não precisam de uma regra adicional apenas para confirmá-los.
5. Nenhum valor, duração, penalidade ou consequência mecânica deve ser presumido sem regra explícita.
6. Um efeito deve ter leitura mecânica e narrativa clara o bastante para ser usado por um Narrador humano ou por uma IA sem depender de contexto externo.
