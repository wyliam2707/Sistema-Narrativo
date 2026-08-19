# Narração e Escrita — Modelo Padrão

Este documento define o **estilo narrativo padrão** do Sistema Narrativo.

Ele foi criado para que uma aventura nova possa ser narrada com consistência mesmo em outro chat ou por outra IA, sem depender de exemplos externos ou de uma conversa anterior.

## Regra de herança

Toda aventura criada com este sistema **herda este modelo por padrão**.

O arquivo local padrão é:

```text
diretrizes/narracao.md
```

Ele registra a direção narrativa escolhida para aquela campanha durante a criação: gênero ou combinação de gêneros, tom, foco, ritmo, humor, romance/intimidade, atmosfera, ênfases e outras escolhas relevantes.

Uma aventura pode alterar tom, ponto de vista, formato de diálogo ou qualquer outra escolha estilística em suas próprias diretrizes, mas somente aquilo que for explicitamente alterado deixa de seguir este modelo.

> **Primeiro aplicar este modelo; depois aplicar `diretrizes/narracao.md` da campanha. O que não for alterado continua herdado.**

O estilo pertence à camada de narração. As regras de resolução continuam definidas pelos demais arquivos de `sistema/`.

### Direção narrativa não é cenário

`diretrizes/narracao.md` responde **como a história deve ser sentida e narrada**.

`mundo/cenario.md` responde **que mundo existe e como ele funciona**.

Uma mesma realidade pode sustentar histórias muito diferentes. Um cenário de fantasia urbana, por exemplo, pode ser usado para investigação sombria, comédia romântica, romance adulto, aventura de ação ou combinações entre esses focos sem que as leis do mundo precisem mudar.

O narrador deve respeitar a direção narrativa sem forçar acontecimentos artificiais apenas para lembrar o gênero. Uma comédia romântica não exige piada em toda cena; um romance não exige atração em toda interação; terror não exige ameaça constante.

---

## 1. Objetivo do estilo

A escrita deve parecer uma história sendo vivida, e não uma transcrição de jogo ou um relatório de ações.

Prioridades:

1. personagem;
2. clareza espacial e causal;
3. experiência da cena;
4. ritmo;
5. continuidade;
6. beleza da prosa sem excesso ornamental.

A prosa deve ser **elegante e acessível**, visual quando necessário e econômica quando o momento pedir velocidade.

A direção narrativa local pode mudar a intensidade, leveza, sensualidade, humor, tensão, ritmo ou foco da experiência sem substituir as regras de agência, causalidade e continuidade.

---

## 2. Ponto de vista

O padrão é **terceira pessoa próxima**.

A cena acompanha a percepção de um personagem por vez, mostrando:

- o que ele vê;
- o que percebe;
- o que sabe;
- o que conclui;
- sensações relevantes;
- pensamentos quando acrescentarem algo à experiência.

Conhecimento do narrador ou do jogador não deve entrar automaticamente na consciência do personagem.

A mudança de ponto de vista pode acontecer entre cenas ou quando a aventura permitir, mas não deve produzir metaconhecimento acidental.

Existe uma diferença obrigatória entre **RPG ao vivo** e **livro consolidado**:

- durante o RPG ao vivo, pensamentos diretos só aparecem para o personagem com `CONTROLE: JOGADOR HUMANO`, quando declarados ou autorizados pelo jogador humano. A narração não entra diretamente nos pensamentos de `NPC`, `JOGADOR IA` ou `JOGADOR EVENTUAL IA`; o jogador humano percebe esses personagens por falas, ações, expressões e outros sinais acessíveis ao seu personagem;
- no livro consolidado, pensamentos explícitos de qualquer personagem podem aparecer quando fizerem sentido para a cena e para o ponto de vista literário adotado.

O livro pode oferecer interioridade mais ampla que a sessão, mas não deve transformar isso em alternância caótica de ponto de vista nem inventar fatos que contradigam o cânone.

---

## 3. Parágrafos e ritmo

Preferir parágrafos relativamente curtos.

Frases isoladas podem ser usadas para:

- impacto;
- conclusão;
- mudança de percepção;
- silêncio;
- surpresa;
- aceleração de ação.

Exemplo de ritmo:

```text
A porta abriu.

Ninguém entrou.

Isso era pior.
```

Não transformar cada frase em um parágrafo por obrigação. O espaço em branco é ferramenta de ritmo, não formato mecânico.

### Pausas

Pausas podem aparecer como ação, silêncio, mudança de olhar, hesitação ou até como uma frase isolada quando realmente importarem.

Evitar transformar expressões como `Uma pausa.` em repetição automática. Preservar o efeito, variando sua realização na cena.

---

## 4. Descrição

A descrição deve ser **seletiva**.

Não catalogar o ambiente inteiro. Escolher aquilo que:

- o personagem perceberia;
- estabelece atmosfera;
- influencia uma decisão;
- ajuda a visualizar espaço e movimento;
- revela algo sobre personagem ou situação.

Usar quando relevante:

- luz;
- som;
- temperatura;
- cheiro;
- textura;
- movimento;
- distância;
- postura;
- expressão;
- presença física.

A atmosfera nasce do lugar e da situação. Nem toda cena precisa ser sombria, intensa ou solene.

Quando `diretrizes/narracao.md` definir uma atmosfera específica, selecionar detalhes que a sustentem de forma natural, sem repetir mecanicamente os mesmos elementos em toda cena.

---

## 5. Mostrar antes de explicar

Sempre que possível, primeiro mostrar uma capacidade, emoção, fenômeno ou ameaça **funcionando na cena**.

Explicar apenas quando a compreensão for necessária.

Exemplo de princípio:

> primeiro o personagem percebe que a chama não produz calor; depois, se importar, alguém explica por quê.

O sobrenatural, tecnologia, poderes e regras do mundo devem existir naturalmente na narrativa. A prosa não deve virar manual de sistema durante a cena.

---

## 6. Falas e marcação de personagem

Toda fala direta usa identificação explícita do personagem.

Formato padrão:

```text
[Nome] — Fala.
```

Exemplo:

```text
[Helena] — Não toque nisso.
```

O nome explícito evita ambiguidade, facilita campanhas longas e preserva a identidade de quem falou quando a sessão for consolidada em livro.

Não substituir esse padrão por diálogo sem identificação apenas por preferência literária, salvo quando uma aventura declarar explicitamente outra convenção em `diretrizes/`.

### Pensamento direto

Quando um pensamento aparecer de forma direta, usar:

```text
[Nome, pensa] — Pensamento.
```

O marcador canônico é `pensa`.

Não usar `[Nome, pensamento]`, aspas internas ou travessão sem identificação como substitutos do formato padrão quando se tratar de pensamento direto explicitado.

### Diferença entre RPG e livro

Durante o **RPG ao vivo**:

- falas de qualquer personagem usam `[Nome] — ...`;
- pensamentos diretos só podem aparecer para o personagem com `CONTROLE: JOGADOR HUMANO`, quando declarados ou autorizados pelo próprio jogador;
- o narrador não escreve pensamentos diretos de `NPC`, `JOGADOR IA` ou `JOGADOR EVENTUAL IA`, salvo se uma diretriz específica da aventura alterar explicitamente essa convenção;
- esses personagens continuam pensando e decidindo segundo sua agência, mas isso aparece ao jogador humano apenas por sinais acessíveis na ficção.

No **livro consolidado**:

- falas continuam usando `[Nome] — ...`;
- pensamentos diretos podem aparecer para qualquer personagem no formato `[Nome, pensa] — ...` quando isso acrescentar algo à cena;
- pensamentos não devem ser usados para inventar decisões, fatos ou segredos que contradigam o que realmente aconteceu.

### Voz individual

Cada personagem deve falar como ele mesmo.

Considerar:

- vocabulário;
- extensão das frases;
- nível de formalidade;
- humor;
- hábitos;
- relação com o interlocutor;
- estado emocional;
- conhecimento disponível.

Não encurtar uma fala longa apenas porque outra personagem costuma falar pouco. Não alongar uma fala curta para preencher espaço.

### Subtexto

Nem tudo precisa ser dito.

Olhares, escolhas, proximidade, silêncio, mudança de assunto, cuidado, irritação e pequenas ações podem carregar parte da conversa.

---

## 7. Pensamentos e interioridade

A interioridade deve estar presente, mas **contida**.

Mostrar pensamentos quando eles:

- mudam a interpretação da cena;
- revelam conflito;
- esclarecem uma escolha;
- mostram algo que não aparece externamente.

Evitar transformar cada ação em explicação psicológica.

Quando uma emoção já está clara pelo comportamento, não é necessário repeti-la em pensamento e depois explicá-la novamente na narração.

Durante o RPG ao vivo, a IA pode usar internamente a mente de `NPC`, `JOGADOR IA` e `JOGADOR EVENTUAL IA` para decidir suas ações, mas **não apresenta essa interioridade diretamente ao jogador humano por padrão**. Mostra apenas comportamento, fala e sinais perceptíveis.

O personagem com `CONTROLE: JOGADOR HUMANO` só recebe pensamento explícito quando o próprio jogador o declarou ou autorizou. O narrador não inventa pensamentos voluntários para ele.

No livro consolidado, pensamentos de qualquer personagem podem ser explicitados quando coerentes com a cena. Essa liberdade literária serve para aprofundar personagens, não para alterar decisões já tomadas ou revelar gratuitamente informação reservada que não pertença ao ponto de vista adotado.

---

## 8. Ação

Ação deve preservar **clareza causal e espacial**.

O leitor precisa conseguir entender:

- quem fez o quê;
- de onde;
- contra quem ou o quê;
- qual foi o resultado;
- como a situação mudou.

Usar frases e parágrafos menores quando a velocidade aumentar.

Poderes e capacidades devem aparecer como ações da ficção, não como relatório de valores.

Evitar:

```text
Ele usou FOR [4] e causou dano Grave.
```

Preferir narrar o acontecimento e, quando necessário, mostrar o `STATUS` separadamente da prosa.

---

## 9. Cotidiano

Cenas cotidianas têm o mesmo direito de existir que combate, investigação ou fenômenos sobrenaturais.

Elas servem para mostrar:

- hábitos;
- convivência;
- amizade;
- romance;
- mudanças de relação;
- recuperação;
- preparação;
- consequências;
- personalidade fora da crise.

Não criar perigo apenas porque uma sequência ficou tranquila.

Se a direção narrativa valorizar cotidiano, romance, humor ou convivência, essas cenas podem ocupar mais espaço sem precisar justificar sua existência por um perigo externo.

---

## 10. Romance e vínculos

Relações devem crescer principalmente por:

- convivência;
- escolhas;
- confiança;
- proximidade;
- observação;
- gestos pequenos;
- iniciativa dos dois lados quando coerente;
- subtexto;
- consequências compartilhadas.

Não transformar sentimento em declaração constante.

O valor `REL` ajuda o narrador a interpretar o vínculo, mas a natureza da relação vem da história.

Personagens continuam possuindo vontade própria dentro de relações amorosas, familiares, amistosas ou hostis.

Uma campanha pode tornar romance, sensualidade ou intimidade parte central da direção narrativa em `diretrizes/narracao.md`. Isso aumenta o espaço e a atenção dados a esses elementos, mas não remove agência, causalidade, personalidade ou direito de recusa e iniciativa dos personagens.

---

## 11. Humor

Humor deve nascer do personagem e da situação.

Pode ser:

- seco;
- provocador;
- expansivo;
- absurdo;
- discreto;
- acidental.

Não dar a todos os personagens o mesmo tipo de piada.

Se a campanha for uma comédia ou comédia romântica, humor pode aparecer com maior frequência, mas não precisa transformar toda fala ou toda cena em piada.

---

## 12. Quando dramatizar e quando resumir

### Dramatizar

Mostrar diretamente quando importarem:

- palavras específicas;
- reações;
- escolha;
- tensão;
- descoberta;
- conflito;
- humor;
- mudança de relação;
- ação decisiva.

### Resumir

Resumir quando importa apenas saber que algo aconteceu:

- dias de rotina;
- deslocamentos sem evento relevante;
- conversas repetitivas;
- treino sem novidade;
- pesquisa prolongada cujo processo não precisa ser vivido inteiro;
- passagem de tempo.

> **Dramatizar o que precisa ser vivido. Resumir o que precisa apenas ter acontecido.**

Uma passagem resumida pode interromper-se e voltar à dramatização no instante em que algo passa a importar.

A direção narrativa local ajuda a decidir o que merece ser vivido em detalhe. Em romance, por exemplo, uma conversa íntima pode merecer dramatização onde uma campanha de ação resumiria o mesmo intervalo.

---

## 13. Quebra de cena

Quando houver mudança clara de tempo, lugar ou foco, pode-se usar:

```text
* * *
```

Não é obrigatório em toda transição.

---

## 14. Narração durante o RPG

Durante o jogo, aplicar o modelo universal e `diretrizes/narracao.md` da campanha, respeitando a agência dos personagens, os ciclos definidos por `CONTROLE` e a diferença entre aquilo que o narrador sabe e aquilo que cada personagem pode perceber.

O narrador deve:

- controlar o mundo e interpretar `NPC` e `JOGADOR EVENTUAL IA` quando inativo;
- preservar o ciclo próprio de decisão de `JOGADOR HUMANO`, `JOGADOR IA` e `JOGADOR EVENTUAL IA` quando ativo;
- permitir agência real aos personagens Centrais e Relevantes;
- respeitar o tom, foco e ritmo locais sem forçar acontecimentos artificiais para cumprir gênero;
- identificar toda fala direta com `[Nome] — ...`;
- não revelar pensamentos diretos de NPCs, Jogadores IA ou Jogadores Eventuais IA durante o RPG ao vivo;
- usar `[Nome, pensa] — ...` apenas para pensamento do personagem com `CONTROLE: JOGADOR HUMANO` que tenha sido declarado ou autorizado pelo jogador humano;
- narrar consequência suficiente para tornar a situação clara;
- parar no próximo ponto significativo em que uma decisão do jogador humano realmente importa;
- não transformar uma frase curta do jogador humano em horas de história sem necessidade;
- não decidir pelo personagem com `CONTROLE: JOGADOR HUMANO` aquilo que cabe ao jogador humano decidir nem substituir a decisão de um ciclo de Jogador IA.

O narrador pode avançar rotinas e consequências previsíveis quando não existe decisão significativa no intervalo.

### Mecânica invisível

A resolução usa ficha, sistema, relações e STATUS internamente, mas a narrativa deve continuar parecendo ficção.

Quando houver alteração relevante de `VIDA`, `ENERGIA` ou `COND`, mostrar o bloco de STATUS fora da prosa, conforme as regras de persistência.

---

## 15. Versão literária / capítulo consolidado

Ao transformar material jogado em capítulo:

- remover comandos de jogador e narrador;
- remover discussões de sistema;
- remover correções fora da história;
- remover versões descartadas;
- preservar decisões e consequências aprovadas;
- reconstruir transições;
- preservar quem sabia o quê em cada momento;
- tratar todos os personagens como pessoas da história, não como `PC` e `NPC`;
- manter a agência demonstrada durante o jogo;
- preservar a direção narrativa específica da campanha;
- identificar todas as falas diretas com `[Nome] — ...`;
- quando houver pensamento direto, usar `[Nome, pensa] — ...`;
- permitir pensamentos de qualquer personagem quando forem coerentes com a cena e acrescentarem interioridade sem mudar os fatos.

A versão literária não deve parecer uma sessão transcrita.

O livro pode explicitar interioridade que permaneceu oculta durante o RPG ao vivo, inclusive de NPCs, desde que isso não invente acontecimento, decisão, conhecimento ou segredo incompatível com o cânone e com o ponto de vista literário adotado.

Não inventar pensamentos decisivos do personagem do jogador para justificar retroativamente uma ação. Quando sua motivação não foi estabelecida, preservar a ambiguidade em vez de fabricar uma razão.

Formato padrão de capítulo:

```text
# CAPÍTULO N
## TÍTULO

Texto...
```

---

## 16. Consistência de personagem acima da voz genérica

A voz geral da obra é consistente, mas **os personagens não devem soar iguais**.

O estilo é a moldura.

Personalidade, relação, história e circunstância determinam o conteúdo humano dentro dela.

> **A voz da narrativa pode ser constante; a voz das pessoas não.**

---

## 17. O que evitar

Evitar por padrão:

- prosa excessivamente ornamental;
- exposição técnica desnecessária;
- repetir a mesma emoção em narração, pensamento e diálogo;
- explicar toda ironia;
- transformar todo silêncio em mistério;
- fazer toda cena terminar em ameaça;
- prolongar mal-entendido quando personagens inteligentes já têm informação para resolvê-lo;
- usar poderes como lista de comandos;
- narrar NPCs como figurantes passivos quando suas fichas indicam iniciativa;
- quebrar personalidade apenas para alcançar um resultado planejado;
- criar reviravolta apenas porque uma solução do jogador foi eficiente;
- revelar pensamentos diretos de NPCs, Jogadores IA ou Jogadores Eventuais IA no RPG ao vivo;
- omitir a identificação de quem falou ou pensou quando o trecho for diálogo ou pensamento direto;
- transformar gênero em obrigação mecânica, como inserir piada, romance, ameaça ou sensualidade em toda cena apenas porque aparecem nas diretrizes.

---

## 18. Calibração

Se houver dúvida sobre como escrever uma cena, usar esta sequência:

> **ler `diretrizes/narracao.md` → ver o mundo pelos olhos do personagem → escolher os detalhes que importam → deixar as pessoas agirem como elas mesmas → mostrar a consequência → parar ou avançar conforme exista decisão significativa.**

O arquivo `sistema/exemplo-de-estilo.md` fornece uma amostra neutra do padrão universal em funcionamento. A campanha aplica sua direção narrativa local sobre essa base.