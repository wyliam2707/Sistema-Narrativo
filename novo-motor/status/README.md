# Status

Esta pasta reúne regras que descrevem o **estado atual do personagem** durante o jogo.

Diferente de Traços, que representam características permanentes ou duradouras, Status descreve condições que estão acontecendo **agora** com o personagem e que podem mudar conforme a ficção.

## Escopo

As regras desta pasta serão construídas para abranger:

- **Vida** — quantidade de dano que o personagem consegue suportar e o que acontece quando sua Vida é reduzida.
- **Dano** — como ferimentos e outras consequências reduzem Vida.
- **Cura** — como Vida perdida pode ser restaurada e quais limites se aplicam.
- **Efeitos Básicos** — estados temporários que alteram o personagem.

Por enquanto, os Efeitos Básicos consolidados são apenas **efeitos nocivos**.

## Efeitos Nocivos

Os efeitos nocivos estão organizados por **famílias** em [`nocivos/`](nocivos/).

Cada família representa uma função reutilizável que pode ser causada por Poderes, perigos ou outras fontes do sistema.

Uma família possui no máximo **3 graus ou estados principais**. Um mesmo estado pode aparecer em mais de uma família quando cumprir a mesma função, sem precisar receber uma nova definição mecânica apenas por estar em outra progressão.

As famílias atuais são:

- **[Sentidos](nocivos/sentidos.md)** — Ofuscado; Cego, Surdo ou Mudo; Inconsciente.
- **[Contenção](nocivos/contencao.md)** — Lento; Imóvel; Paralisado.
- **[Terror](nocivos/terror.md)** — Abalado; Apavorado; Paralisado.
- **[Exaustão](nocivos/exaustao.md)** — Fatigado; Exausto; Inconsciente.
- **[Perturbação](nocivos/perturbacao.md)** — Abalado; Confuso; Atordoado.
- **[Aflição](nocivos/aflicao.md)** — dano contínuo em graus 1, 2 e 3.
- **[Posição](nocivos/posicao.md)** — Caído; Movido; Conduzido.
- **[Influência](nocivos/influencia.md)** — Enfeitiçado; Compelido; Dominado.
- **[Defesa](nocivos/defesa.md)** — Desprevenido; Vulnerável; Indefeso.
- **[Debilitação](nocivos/debilitacao.md)** — Fraco; Debilitado; Inconsciente.

## Como interpretar um Status

Cada Status deve dizer principalmente:

1. **Efeito mecânico** — o que muda objetivamente enquanto o estado se aplica.
2. **Efeito narrativo** — como essa condição pode alterar a situação dentro e fora de combate.
3. **Remoção** — o que encerra ou remove o estado quando isso fizer parte de sua própria definição.

O efeito mecânico não substitui a ficção. Ficar cego, imóvel, apavorado ou enfraquecido pode produzir consequências narrativas muito maiores do que uma simples penalidade em dados, dependendo da situação.

Da mesma forma, um Status não determina automaticamente como uma persona reage, salvo quando sua própria regra estabelecer uma impossibilidade ou controle específico. A agência continua sendo respeitada.

## Limites desta pasta

Esta pasta **não define por enquanto**:

- como um Poder aplica um Status;
- qual Atributo é usado para resistir;
- custo de Energia;
- alcance, área ou quantidade de alvos;
- duração geral de efeitos.

Essas regras pertencem aos capítulos apropriados do sistema.

## Princípios

1. Status descreve o que está acontecendo **agora** com o personagem.
2. Traços descrevem aquilo que o personagem **é, possui ou carrega como característica**.
3. Poderes e outras regras podem criar, remover ou modificar Status, mas não substituem suas definições.
4. Nenhum valor, duração, penalidade ou consequência deve ser presumido sem regra explícita.
5. Um Status deve ter leitura mecânica e narrativa clara o bastante para ser usado por um Narrador humano ou por uma IA sem depender de contexto externo.
