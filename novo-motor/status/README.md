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

As famílias atuais são:

- **[Sentidos](nocivos/sentidos.md)** — Ofuscado; Cego, Surdo ou Mudo; Privado.
- **[Contenção](nocivos/contencao.md)** — Lento; Imóvel; Paralisado.
- **[Terror](nocivos/terror.md)** — Abalado; Apavorado; Aterrorizado.
- **[Exaustão](nocivos/exaustao.md)** — Fatigado; Exausto; Inconsciente.
- **[Perturbação](nocivos/perturbacao.md)** — Desorientado; Confuso; Atordoado.
- **[Aflição](nocivos/aflicao.md)** — 1 de dano; 1d3 de dano; 1d6 de dano por turno.
- **[Posição](nocivos/posicao.md)** — Caído; Movido; Conduzido.
- **[Influência](nocivos/influencia.md)** — Enfeitiçado; Compelido; Dominado.
- **[Defesa](nocivos/defesa.md)** — Desprevenido; Exposto; Indefeso.
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
- custo de Energia;
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
