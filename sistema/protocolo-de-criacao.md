# Protocolo de Criação de Campanha

Este documento define **como criar uma nova campanha** usando o Sistema Narrativo.

O objetivo é evitar formulários longos, não perder decisões durante a conversa e separar claramente **criação conceitual** de **revisão e conversão mecânica**.

> **Primeiro construímos a campanha conceitualmente. Depois revisamos e aplicamos as regras. Só então começamos a jogar.**

---

## 1. Entrada do protocolo

O repositório deve sempre começar perguntando:

> **Nova campanha ou continuar uma campanha existente?**

Se o jogador escolher **continuar**, este protocolo não é iniciado. O narrador deve listar as campanhas existentes em `aventuras/`, deixar o jogador escolher e carregar a aventura conforme suas fontes de continuidade.

Se o jogador escolher **nova campanha**, iniciar este protocolo.

---

## 2. Nome da campanha vem primeiro

Antes de qualquer pergunta de criação, perguntar:

> **Qual será o nome da campanha?**

Assim que o nome for definido, criar **imediatamente a estrutura completa da aventura**, já materializada por arquivos `README.md` em todas as pastas estruturais:

```text
aventuras/<nome-da-campanha>/
├── README.md
├── criacao.md
├── diretrizes/
│   └── README.md
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
│   └── README.md
└── livro/
    └── README.md
```

Git não preserva diretórios vazios. Por isso, **não esperar a primeira utilização de cada pasta**: o `README.md` estrutural deve existir desde o começo e manter a estrutura visível e compreensível para outro chat ou outra IA.

Cada `README.md` estrutural deve ser curto e explicar:

- a função daquela pasta;
- que tipo de informação pertence ali;
- o que não deve ser colocado ali quando existir risco de confusão;
- qualquer regra especial de visibilidade ou persistência daquela área.

Funções mínimas esperadas:

- `diretrizes/` — direção narrativa e regras específicas de narração e funcionamento daquela campanha;
- `personagens/` — fichas apresentáveis de personagens Centrais e Relevantes;
- `mestre/` — material persistente reservado ao narrador;
- `mestre/viloes/` — fichas ocultas de antagonistas importantes quando necessárias;
- `mundo/` — cenário, locais, organizações e fatos estáveis do mundo;
- `relacionamento/` — vínculos recorrentes ou complexos que precisem de acompanhamento próprio;
- `progressao/` — consequências duradouras ainda causalmente vivas;
- `cronologia/` — índice objetivo do que aconteceu e de mudanças relevantes de conhecimento;
- `estado/` — `inicio.md` como marco inicial aprovado e `atual.md` como savegame operacional mutável;
- `livro/` — capítulos ou outro registro narrativo canônico consolidado.

`mestre/` é uma área reservada ao narrador. Ela pode conter informações que precisam existir de forma persistente sem serem apresentadas ao jogador durante a sessão. `mestre/viloes/` é o local padrão para fichas ocultas de antagonistas importantes quando forem necessárias.

Essa área não é tecnicamente privada para o proprietário do repositório; “reservada” significa apenas que o narrador ou outra IA não deve revelar espontaneamente seu conteúdo durante o RPG.

Criar imediatamente `criacao.md` para registrar o andamento.

O `README.md` da raiz da aventura também existe desde o começo. Durante a criação ele pode ser apenas uma porta de entrada curta indicando que a campanha está em montagem e apontando para `criacao.md`; depois da aprovação final ele deve ser atualizado com a entrada completa da campanha.

Modelo inicial de `criacao.md`:

```text
# Criação da Campanha

Status geral: EM CRIAÇÃO

1. Direção narrativa e cenário: NÃO INICIADO
   - Diretrizes narrativas: NÃO INICIADO
   - Cenário: NÃO INICIADO
2. Protagonista: NÃO INICIADO
3. Personagens relevantes: NÃO INICIADO
4. Início da história: NÃO INICIADO

Revisão final: NÃO INICIADA
```

> **A estrutura nasce junto com a campanha. Pasta estrutural sem conteúdo próprio ainda mantém seu `README.md` explicando para que existe.**

---

## 3. Regra de perguntas

Durante as quatro etapas conceituais:

- fazer **uma pergunta por vez**, exceto quando um pequeno bloco puder ser respondido de forma mais eficiente;
- não pedir informação que já possa ser inferida das respostas anteriores;
- não transformar a criação em questionário enciclopédico;
- se o jogador disser `decida você`, escolher uma opção coerente e continuar;
- parar de perguntar quando já houver informação suficiente para aquela etapa;
- detalhes menores podem ser criados durante a própria campanha quando passarem a importar.

As opções apresentadas ao jogador são **exemplos, nunca uma lista fechada**. O jogador pode combinar gêneros, tons e focos livremente.

> **Perguntar apenas aquilo que o jogador realmente precisa decidir.**

---

## 4. Regra de salvamento e revisão

Cada etapa conceitual passa por este fluxo:

> **Perguntar → Construir → Organizar → Salvar como PENDENTE DE REVISÃO → Próxima etapa**

Durante a criação conceitual, **PENDENTE DE REVISÃO não significa canônico definitivo**.

O narrador pode organizar o material em arquivos próprios, mas não deve tratá-lo como aprovado apenas porque foi escrito.

Não salvar cada tentativa, correção ou frase descartada. Ao fechar uma etapa, consolidar apenas a versão atualmente aceita.

Estados recomendados:

- `NÃO INICIADO`
- `EM ANDAMENTO`
- `PENDENTE DE REVISÃO`
- `APROVADO`

Ao final de cada etapa, atualizar também `criacao.md`.

Isso permite interromper a conversa e retomar depois sem refazer o processo.

Fichas reservadas em `mestre/viloes/` seguem uma exceção: não passam por aprovação aberta do jogador, porque isso revelaria informações que devem permanecer ocultas. A regra específica aparece adiante.

---

# AS QUATRO ETAPAS CONCEITUAIS

## 5. Etapa 1 — Direção narrativa e Cenário

Objetivo: definir **que tipo de história o jogador quer viver e em que mundo essa história acontece**.

A etapa possui duas partes relacionadas, mas salva cada uma no lugar correto:

```text
Direção narrativa → diretrizes/narracao.md
Cenário           → mundo/cenario.md
```

### 5.1. Direção narrativa — que tipo de história queremos?

Começar pela experiência desejada. Uma pergunta inicial útil é:

> **Que tipo de história você quer viver?**

Exemplos possíveis incluem aventura, drama, comédia, comédia romântica, romance, romance adulto ou erótico, terror, investigação, ação, sobrevivência, política, faroeste ou qualquer combinação descrita pelo jogador.

A lista é apenas ilustrativa. Não transformar gênero em menu fechado.

Conforme a resposta, perguntar somente o que ainda for necessário para entender a direção. Podem importar:

- gênero ou combinação de gêneros;
- tom principal e tons secundários;
- foco narrativo;
- ritmo desejado;
- presença e natureza do humor;
- romance e intimidade, quando relevantes;
- atmosfera;
- elementos que devem receber mais espaço;
- elementos que devem ser evitados ou usados com moderação;
- exceções ao modelo narrativo universal.

Nem todo campo precisa ser perguntado ou preenchido.

Exemplo: se o jogador disser `comédia romântica adulta leve`, o narrador já possui gênero, tom e parte do foco. Deve perguntar apenas o que realmente faltar para começar a campanha.

Outro exemplo:

```text
Gênero principal: romance adulto
Tom secundário: comédia romântica
Ambientação: fantasia urbana
Ritmo: cotidiano com momentos intensos
```

Essas informações pertencem a `diretrizes/narracao.md`, não a `mundo/cenario.md`.

### 5.2. Cenário — em que mundo essa história acontece?

Depois ou em conjunto com a direção narrativa, definir o suficiente do mundo para sustentar os personagens e a abertura.

Perguntar uma coisa por vez conforme necessário. Exemplos de informação que podem importar:

- universo ou tipo de cenário;
- local principal;
- época, se relevante;
- tecnologia;
- magia ou sobrenatural;
- regras específicas do mundo;
- organizações ou estruturas essenciais à premissa;
- se for fanfic, grau de fidelidade ao cânone;
- adaptações gerais desejadas;
- elementos obrigatórios já declarados pelo jogador.

Não perguntar detalhes sem utilidade imediata apenas para preencher o mundo.

Se o jogador escolher um universo conhecido, o narrador pode usar seu conhecimento para preencher detalhes secundários e deve perguntar apenas quando existir uma escolha de adaptação que realmente importe.

### Separação obrigatória entre direção e mundo

`diretrizes/narracao.md` responde principalmente:

> **Como esta campanha deve ser sentida e narrada?**

`mundo/cenario.md` responde principalmente:

> **Que mundo existe e como ele funciona?**

Não duplicar automaticamente o mesmo texto nos dois arquivos.

Uma informação pode influenciar ambos, mas deve ser registrada segundo sua função. `Magia é pública` é fato de cenário. `Magia cotidiana não deve ser narrada como espetáculo toda vez que aparece` é diretriz narrativa.

### Fechamento da etapa

Quando houver direção narrativa e cenário suficientes:

1. criar ou atualizar `diretrizes/narracao.md`;
2. criar ou atualizar `mundo/cenario.md`;
3. marcar ambos como:

```text
Status: PENDENTE DE REVISÃO
```

4. atualizar em `criacao.md`:

```text
1. Direção narrativa e cenário: PENDENTE DE REVISÃO
   - Diretrizes narrativas: PENDENTE DE REVISÃO
   - Cenário: PENDENTE DE REVISÃO
```

5. seguir para a Etapa 2 sem iniciar ainda a revisão.

Se o jogador não desejar nenhuma exceção especial de estilo além do padrão universal, `diretrizes/narracao.md` ainda pode existir de forma mínima, registrando a direção geral escolhida e que o restante é herdado do sistema.

---

## 6. Etapa 2 — Protagonista

Objetivo: criar **o protagonista como pessoa e conceito**, ainda sem calibrar sua ficha numérica.

Começar pela identidade, não pela mecânica.

Perguntar uma coisa por vez conforme necessário, normalmente seguindo algo próximo de:

- nome;
- quem o controla;
- aparência física;
- imagem de referência, quando fornecida;
- idade real e aparente, quando diferentes;
- natureza/origem relevante;
- personalidade;
- comportamento social;
- história essencial;
- trajetória de vida ou ocupações importantes;
- situação e motivação atuais.

Para um protagonista controlado pelo usuário, registrar normalmente:

```text
CONTROLE: JOGADOR HUMANO
```

Se a campanha possuir outro arranjo de controle, o usuário pode defini-lo explicitamente.

Não perguntar sobre cada detalhe biográfico se ele não for necessário para compreender o personagem.

### Imagens de referência

Quando o jogador fornecer uma imagem, ela pode ser usada para construir a descrição visual do personagem. O arquivo deve guardar a **descrição consolidada**, não depender exclusivamente da imagem para que outra IA compreenda a aparência.

### Ficha estrutural desde o começo

O arquivo do protagonista deve usar, desde esta etapa, a estrutura final de ficha sempre que ela já for conhecida.

Preencher apenas o que já foi definido conceitualmente. Campos mecânicos ainda desconhecidos permanecem **em branco**.

> **Nunca usar `[0]` para representar informação desconhecida. Zero é um valor mecânico real.**

Campos conceituais podem incluir, quando relevantes:

- identidade;
- `CONTROLE`;
- descrição;
- `TRAÇOS` permanentes não numéricos;
- personalidade e tendências;
- história consolidada;
- desejos/objetivos atuais;
- medos/limites relevantes.

### O que NÃO fazer nesta etapa

Ainda não calibrar:

- FOR, AGI, RES, MEN ou VON;
- graus de perícia;
- graus de poderes;
- relações numéricas ainda não estabelecidas;
- ficha mecânica completa.

`CONTROLE` não é valor mecânico. Ele pode ser definido desde a criação porque determina quem possui o ciclo de decisão do personagem.

Esses elementos mecânicos pertencem à revisão posterior.

### Fechamento da etapa

Quando o conceito do protagonista estiver suficiente:

1. organizar o conceito em `personagens/<nome>.md`;
2. registrar o `CONTROLE` já definido;
3. manter a estrutura da ficha, deixando em branco o que ainda não foi definido;
4. marcar:

```text
Status: PENDENTE DE REVISÃO
```

5. atualizar `criacao.md`:

```text
2. Protagonista: PENDENTE DE REVISÃO
```

6. seguir para a Etapa 3.

---

## 7. Etapa 3 — Personagens relevantes

Objetivo: definir **qual é o elenco inicial que merece acompanhamento como Central ou Relevante e como cada personagem será controlado**.

O protocolo não precisa perguntar ao jogador por todo personagem óbvio de um cenário conhecido.

Quando o universo escolhido já indicar personagens naturalmente relevantes, o narrador pode identificá-los e propor sua inclusão.

### Controle dos personagens relevantes

Ao apresentar ou consolidar os nomes do elenco inicial, apresentar também uma proposta de `CONTROLE` ao lado de cada nome quando isso ajudar.

Exemplo:

```text
Ravena — JOGADOR IA
Robin — JOGADOR EVENTUAL IA
Estelar — NPC
Mutano — NPC
```

O usuário pode revisar e mudar essas categorias durante a criação e novamente durante a revisão da ficha.

Categorias válidas para fichas apresentáveis em `personagens/`:

```text
CONTROLE: JOGADOR HUMANO
CONTROLE: JOGADOR IA
CONTROLE: JOGADOR EVENTUAL IA
CONTROLE: NPC
```

`JOGADOR IA` significa que a IA joga permanentemente com aquele personagem, mantendo sua função de jogadora separada da função de narradora.

`JOGADOR EVENTUAL IA` significa que o usuário já autorizou a IA a assumir temporariamente aquele personagem como jogadora quando a própria campanha produzir uma situação que justifique agência operacional de jogador. Depois que essa categoria estiver aprovada, a IA decide quando ativar ou desativar o modo eventual e **não precisa pedir nova autorização a cada cena**.

Quando um Jogador Eventual IA não está ativo como jogador, funciona normalmente como NPC.

`NPC` não pode ser ativado como Jogador Eventual IA. Para isso, seu campo `CONTROLE` precisa primeiro ser alterado com aprovação do usuário.

Somente personagens com ficha em `personagens/` podem receber `JOGADOR EVENTUAL IA`. Figurantes, inimigos comuns e antagonistas reservados em `mestre/viloes/` não entram nesse mecanismo diretamente.

> **O usuário decide quem a IA pode jogar. Depois de autorizado como Jogador Eventual IA, a IA decide quando usar essa função.**

### Personagens canônicos ou licenciados

Quando forem usados personagens existentes, perguntar de forma simples se o jogador quer:

- base canônica;
- base canônica flexível;
- adaptação mais livre.

Se uma adaptação específica já foi declarada — idade diferente, fase específica, relação alterada etc. — registrá-la sem exigir nova confirmação desnecessária.

Preservar identidade, personalidade, poderes e relações essenciais conforme o grau de fidelidade escolhido.

### Criação conceitual mínima de aliados

Durante esta etapa, pode ser suficiente definir apenas **a quantidade, os nomes e a categoria de controle proposta** dos aliados relevantes.

Se isso for tudo que o jogador quiser decidir naquele momento:

1. criar `personagens/<nome>.md` usando o modelo oficial de Personagem Relevante;
2. preencher nome, importância e `CONTROLE` quando já definidos;
3. preencher somente o restante que já foi realmente estabelecido;
4. deixar os demais campos em branco;
5. não inventar aparência, personalidade, história, capacidades ou recursos apenas para completar a ficha;
6. desenvolver esses elementos durante a revisão posterior.

Se o jogador disser `decida você`, `faça por mim` ou delegar de forma equivalente, o narrador pode propor esses detalhes, inclusive o `CONTROLE`, mas eles continuam sujeitos ao fluxo normal de revisão e aprovação.

> **Nome e controle podem bastar para fechar a criação conceitual de um aliado. Detalhe faltante não precisa ser inventado antes da revisão.**

### Fechar o elenco inicial

Depois de identificar os personagens óbvios, perguntar:

> **Existe mais algum personagem que você quer considerar relevante desde o começo?**

Quando o jogador disser que não, fechar o elenco.

O narrador continua livre para criar depois:

- vilões;
- aliados;
- organizações;
- figurantes;
- ameaças;
- novos personagens.

Esses personagens futuros não precisam ser previstos no protocolo.

Inimigos comuns normalmente permanecem Figurantes e **não exigem ficha persistente**. Basta usar o modelo rápido e as exceções necessárias durante a cena.

Um antagonista importante, recorrente ou poderoso pode receber ficha completa quando passar a importar. Se suas capacidades, objetivos ou segredos não devem ser revelados ao jogador, armazenar a ficha em:

```text
mestre/viloes/<nome>.md
```

Essa ficha pode ser criada pelo narrador sem ser apresentada ao jogador. Sempre que for prático, capacidades ocultas relevantes devem ser definidas antes de entrarem diretamente em conflito com o protagonista.

Depois de estabelecida, a ficha não pode ser alterada apenas para contrariar uma solução válida, restaurar dificuldade ou proteger a trama.

### Fichas estruturais nesta fase

Para cada personagem Central ou Relevante **do elenco inicial apresentável ao jogador**, criar `personagens/<nome>.md` usando a estrutura final de ficha.

Registrar `CONTROLE` junto da identidade funcional da ficha.

Preencher tudo que já for conhecido conceitualmente e deixar os campos ainda não definidos **em branco**.

Não inventar valores apenas para preencher a ficha.

> **Campo desconhecido fica em branco. `[0]` continua sendo um valor real, nunca um marcador de pendência.**

Cada arquivo permanece:

```text
Status: PENDENTE DE REVISÃO
```

A ficha conceitual pode conter identidade, `CONTROLE`, descrição, `TRAÇOS`, personalidade, história, desejos, medos e outras informações já consolidadas. A mecânica será revisada depois.

Fichas reservadas em `mestre/viloes/` usam o modelo próprio definido em `sistema/modelos.md` e não entram neste fluxo de aprovação aberta nem no mecanismo de Jogador Eventual IA.

Atualizar `criacao.md`:

```text
3. Personagens relevantes: PENDENTE DE REVISÃO
```

Depois seguir para a Etapa 4.

---

## 8. Etapa 4 — Início da história

Objetivo: definir **a situação concreta necessária para começar a primeira cena**, como o início real da história, sem planejar a campanha inteira.

A base deve responder apenas ao que importa para abrir a campanha, por exemplo:

- onde a história começa;
- como está a vida dos personagens imediatamente antes da abertura;
- por que os personagens entram em contato;
- qual necessidade, interesse ou acontecimento dispara esse contato;
- o que cada personagem sabe naquele momento;
- o que está acontecendo quando a cena abre;
- ponto exato em que o jogador recebe controle.

O narrador pode apresentar uma **base consolidada para revisão**, o jogador ajusta, e a base é reapresentada até aprovação.

Não exigir:

- vilão final;
- estrutura em três atos;
- capítulos futuros;
- resultado planejado do romance;
- solução antecipada dos conflitos;
- arcos fechados antes de jogar.

Quando houver romance, pode existir um **tema ou tensão inicial**, mas isso não deve predeterminar sentimentos, escolhas ou resultados futuros.

> **A criação precisa definir o começo, não decidir o futuro.**

### Fechamento da etapa

Consolidar o início da história em `estado/inicio.md` e marcar:

```text
Status: PENDENTE DE REVISÃO
```

Atualizar `criacao.md`:

```text
4. Início da história: PENDENTE DE REVISÃO
Revisão final: PRONTA PARA INICIAR
```

Ainda não iniciar a primeira cena.

---

# REVISÃO E CONVERSÃO PARA O SISTEMA

## 9. Só revisar depois das quatro etapas

Depois que Direção narrativa e Cenário, Protagonista, Personagens relevantes e Início da história estiverem organizados, iniciar a revisão.

A revisão serve para:

- corrigir conceitos;
- confirmar o que será canônico;
- confirmar a direção narrativa desejada;
- confirmar `CONTROLE` dos personagens apresentáveis;
- aplicar atributos, perícias, poderes e demais regras;
- verificar coerência entre direção narrativa, cenário e personagens;
- preparar o estado inicial real da campanha.

> **Conceito primeiro. Mecânica depois.**

> **Revisar não significa recriar.**

Durante toda a revisão:

- preservar exatamente o que já foi consolidado;
- não reescrever ou embelezar conteúdo aprovado sem necessidade;
- localizar apenas o que ainda está pendente;
- apresentar somente o campo ou bloco que está sendo revisado naquele momento;
- explicar números brevemente quando isso ajudar;
- depois da correção, reapresentar o campo ou bloco normalizado para aprovação;
- só avançar ao próximo campo ou bloco depois da confirmação do jogador.

Fichas reservadas do narrador não são apresentadas nesta revisão. Elas obedecem às regras de `mestre/viloes/` e ao princípio de não revelar informação oculta.

---

## 10. Revisão da direção narrativa e do cenário

A revisão da Etapa 1 acontece em duas partes, na mesma ordem em que a campanha será interpretada.

### Diretrizes narrativas

Apresentar `diretrizes/narracao.md` ao jogador.

O jogador pode:

- aprovar;
- corrigir;
- combinar ou separar tons;
- alterar foco ou ritmo;
- acrescentar ou remover ênfases;
- alterar qualquer escolha local de narração.

Depois da confirmação, marcar:

```text
Status: APROVADO
```

### Cenário

Depois, apresentar `mundo/cenario.md` ao jogador de forma organizada.

O jogador pode:

- aprovar;
- corrigir;
- acrescentar;
- remover.

Depois da confirmação, marcar:

```text
Status: APROVADO
```

Atualizar `criacao.md`:

```text
1. Direção narrativa e cenário: APROVADO
   - Diretrizes narrativas: APROVADO
   - Cenário: APROVADO
```

A partir daí, `diretrizes/narracao.md` define a direção narrativa local e `mundo/cenario.md` define a realidade do mundo.

---

## 11. Ordem obrigatória da revisão das fichas

Na **criação conceitual**, o protagonista continua sendo criado antes do elenco relevante.

Na **revisão das fichas apresentáveis ao jogador**, a ordem é diferente:

> **Personagens relevantes/NPCs visíveis primeiro → protagonista por último.**

O protagonista fica por último para impedir que seus valores sirvam como referência inconsciente para calibrar os demais personagens.

Cada personagem deve ser avaliado por aquilo que ele próprio representa.

> **Nunca usar outra ficha como régua mecânica.**

> **Nunca aumentar ou reduzir uma capacidade para balancear um personagem com outro.**

A ficha não precisa ser justa, simétrica ou possuir quantidade semelhante de valores altos.

Nenhum personagem precisa possuir um `[5]`.

Fichas ocultas em `mestre/viloes/` ficam fora dessa ordem de revisão, porque não são exibidas ao jogador.

---

## 12. Regra de calibração mecânica

A escala do sistema deve ser aplicada de forma conservadora.

Se houver dúvida real entre dois graus adjacentes, usar o menor.

Exemplos:

```text
dúvida entre [2] e [3] → usar [2]
dúvida entre [3] e [4] → usar [3]
```

A mesma lógica vale para atributos, perícias, poderes e especializações quando aplicável.

> **Na dúvida, arredondar para baixo.**

`[5]` continua reservado para algo que realmente represente o ápice daquela escala.

Valores altos não são distribuídos por necessidade de equilíbrio de grupo, importância narrativa ou comparação com o protagonista.

A mesma calibração conservadora vale para antagonistas reservados ao narrador. Sigilo não justifica valores inflados.

---

## 13. Dois métodos de revisão de ficha

Revisar **um personagem por vez**.

Existem dois métodos diferentes conforme quem controla o personagem:

- **personagem controlado pelo jogador humano:** revisão campo por campo, com três blocos mecânicos próprios;
- **demais personagens apresentáveis ao jogador:** revisão em quatro blocos maiores.

Em ambos os casos, `CONTROLE` deve ser confirmado antes da mecânica.

A regra é:

> **Apresentar → corrigir se necessário → reapresentar normalizado → obter aprovação → só então avançar.**

A ficha completa só é apresentada depois que todos os campos ou blocos tiverem sido revisados.

Fichas reservadas em `mestre/viloes/` não entram nesses métodos de aprovação aberta.

### 13.1. Personagem controlado pelo jogador humano — campo por campo

A ficha do personagem do jogador humano deve ser revisada com controle fino.

Campos simples são apresentados **individualmente**, um de cada vez. O narrador não deve misturar o próximo campo antes da aprovação do atual.

A ordem recomendada segue a própria ficha:

1. nome/identidade, quando ainda houver algo a revisar;
2. `CONTROLE`;
3. idade;
4. conceito;
5. descrição;
6. `TRAÇOS`;
7. **ATRIBUTOS** — bloco único com `FOR`, `AGI`, `RES`, `MEN` e `VON`;
8. **PERÍCIAS** — bloco único com todas as perícias relevantes;
9. **PODERES** — bloco único com todos os poderes e especializações;
10. `EQP`;
11. `REL`;
12. personalidade e tendências;
13. desejos/objetivos atuais;
14. medos/limites relevantes;
15. história consolidada relevante.

Se um campo já estiver plenamente definido, apresentá-lo como está para confirmação; não reabrir sua criação sem necessidade.

Nos blocos de ATRIBUTOS, PERÍCIAS e PODERES, o jogador pode responder de forma compacta. O narrador normaliza a sintaxe e reapresenta o **bloco inteiro** antes de pedir aprovação.

Para PODERES, manter sempre que possível um poder completo por linha, incluindo suas especializações.

Exemplo:

```text
Alma Astral [3] => Projeção [3] / Manifestação [3] / Contenção [3] / Telecinese [2] / Voo [2]
```

> **No personagem do jogador humano, campo simples é uma revisão; ATRIBUTOS, PERÍCIAS e PODERES são três blocos próprios.**

### 13.2. Demais personagens apresentáveis — quatro blocos

Personagens relevantes, NPCs originais, canônicos ou licenciados que serão apresentados ao jogador usam uma revisão mais compacta em **quatro blocos**:

**Bloco 1 — Identidade e conceito**
- nome;
- importância;
- `CONTROLE`;
- idade;
- conceito;
- descrição;
- `TRAÇOS`.

**Bloco 2 — Capacidades**
- atributos;
- perícias;
- poderes e especializações.

**Bloco 3 — Recursos**
- `EQP` e recursos recorrentes;
- `REL` atual e recorrente.

**Bloco 4 — Interpretação**
- personalidade e tendências;
- desejos/objetivos atuais;
- medos/limites relevantes;
- história consolidada relevante.

O narrador pode propor uma base para qualquer bloco, inclusive quando o jogador delegou a criação, mas deve apresentar, ajustar e obter aprovação do jogador **antes de avançar ao bloco seguinte**.

No Bloco 1, o usuário pode alterar livremente a proposta de `CONTROLE`. Essa escolha define quem terá o ciclo de decisão daquele personagem durante a campanha.

Se algum campo dentro do bloco não possuir importância real, ele pode permanecer vazio. Não inventar conteúdo apenas para completar visualmente a ficha.

> **Outros personagens são revisados em quatro blocos; o personagem do jogador humano recebe revisão mais fina.**

---

## 14. Personagens canônicos, NPCs e antagonistas ocultos na revisão

Para personagens canônicos, licenciados ou já conhecidos, o narrador pode propor o conteúdo com base em:

- identidade canônica escolhida;
- continuidade definida para a campanha;
- adaptações já aprovadas;
- conceito consolidado daquela personagem;
- função de controle desejada na campanha.

A proposta deve respeitar os **quatro blocos** da Seção 13.2.

O narrador não deve transformar a revisão em uma recriação espontânea do personagem.

Para NPCs originais criados pelo narrador e apresentáveis ao jogador, aplicar o mesmo método com base no conceito já estabelecido.

Cada proposta continua apenas:

```text
Status: PENDENTE DE REVISÃO
```

até a ficha completa ser aprovada.

> **Ficha proposta não é ficha aprovada.**

### Inimigos comuns

Inimigos comuns normalmente são Figurantes.

Eles não precisam receber arquivo individual nem entrar na revisão de fichas. O narrador usa apenas o modelo rápido e as exceções necessárias para a cena.

Se um inimigo sobreviver, reaparecer ou ganhar importância real, ele pode então receber ficha adequada.

### Antagonistas reservados ao narrador

Um antagonista importante, recorrente ou poderoso pode receber ficha completa em:

```text
mestre/viloes/<nome>.md
```

Usar o modelo `Ficha reservada — antagonista importante` de `sistema/modelos.md`.

Essa ficha:

- não é apresentada ao jogador para aprovação;
- pode conter capacidades, objetivos, limites e segredos ainda desconhecidos;
- deve respeitar a mesma calibração mecânica do restante do sistema;
- deve ser consultada pelo narrador quando o antagonista agir;
- não pode ser reescrita retroativamente apenas para neutralizar o protagonista, recuperar dificuldade ou proteger o roteiro;
- só deve mudar quando acontecimentos reais da ficção justificarem a mudança;
- não participa do mecanismo de Jogador Eventual IA enquanto permanecer em `mestre/viloes/`.

Sempre que for prático, definir capacidades ocultas relevantes antes de usá-las diretamente contra o protagonista.

> **O narrador pode esconder a informação; não pode mudar a realidade depois de descobrir a solução do jogador.**

---

## 15. Revisão do protagonista — sempre por último entre as fichas

Somente depois de todas as fichas iniciais de personagens relevantes/NPCs **apresentáveis ao jogador** terem sido revisadas, abrir a ficha do protagonista.

O conceito já consolidado deve ser preservado.

Não perguntar novamente aquilo que já foi decidido sem necessidade. Em vez disso, apresentar cada campo já consolidado para confirmação conforme o método da Seção 13.1.

A revisão do protagonista segue obrigatoriamente:

> **campos simples um por vez → ATRIBUTOS como bloco → PERÍCIAS como bloco → PODERES como bloco → demais campos simples um por vez → ficha completa.**

`CONTROLE` é um dos primeiros campos simples e normalmente será `JOGADOR HUMANO` quando o protagonista pertence ao usuário.

O narrador pode organizar, normalizar sintaxe e apontar incoerências com as regras, mas não deve recalibrar o protagonista para aproximá-lo dos NPCs já revisados.

A mesma regra vale nos dois sentidos:

> **NPCs não são balanceados com o protagonista, e o protagonista não é balanceado com os NPCs.**

Fichas ocultas de antagonistas não servem como régua para o protagonista e não são comparadas a ele durante a revisão.

---

## 16. Aprovação final de cada ficha

Quando todos os campos ou blocos de uma personagem **apresentável ao jogador** estiverem revisados, apresentar **a ficha completa consolidada** ao jogador.

Enquanto essa leitura final não for aprovada, manter:

```text
Status: PENDENTE DE REVISÃO
```

Depois da aprovação explícita:

1. consolidar somente a versão aceita;
2. salvar o arquivo;
3. mudar para:

```text
Status: APROVADO
```

4. considerar também aprovado o `CONTROLE` registrado na ficha;
5. seguir para a próxima ficha.

Para `JOGADOR EVENTUAL IA`, essa aprovação já autoriza a IA a decidir futuras ativações e desativações sem pedir permissão novamente para cada cena. Mudar depois a categoria de `CONTROLE` continua exigindo decisão explícita do usuário.

Não carregar correções descartadas, explicações de conversa ou versões intermediárias para a ficha final.

Fichas reservadas em `mestre/viloes/` são a exceção. Elas usam:

```text
Status: CANÔNICO DO MESTRE
Visibilidade: MESTRE
```

e não são exibidas ao jogador para aprovação.

---

## 17. Revisão do início da história

Depois que direção narrativa, cenário e fichas estiverem aprovados, revisar `estado/inicio.md` como **o começo concreto da história**.

Apresentar a base consolidada, ajustar com o jogador e reapresentar até aprovação.

Verificar se o início é coerente com:

- direção narrativa e tom escolhidos;
- capacidades reais dos personagens;
- categorias de `CONTROLE` definidas;
- relações estabelecidas;
- cenário;
- localização;
- informação disponível;
- motivações atuais.

O início pode estabelecer:

- motivo do primeiro encontro;
- vantagem ou problema inicial;
- interesse ou curiosidade;
- tema de um romance;
- tensão dramática inicial.

Mas não deve determinar antecipadamente:

- sentimentos futuros;
- escolhas dos personagens;
- resultado do romance;
- solução da campanha.

Depois da aprovação:

1. marcar `estado/inicio.md` como `APROVADO`;
2. criar `estado/atual.md` com o ponto operacional exato em que a campanha começa;
3. atualizar o `README.md` da raiz da aventura para apontar para `diretrizes/narracao.md`, `mundo/cenario.md`, estado e demais fontes necessárias.

---

## 18. Encerramento da criação

Quando tudo estiver aprovado, `criacao.md` deve ficar aproximadamente assim:

```text
# Criação da Campanha

Status geral: CONCLUÍDA

1. Direção narrativa e cenário: APROVADO
   - Diretrizes narrativas: APROVADO
   - Cenário: APROVADO
2. Protagonista: APROVADO
3. Personagens relevantes: APROVADOS
4. Início da história: APROVADO

Revisão final: CONCLUÍDA
```

`criacao.md` pode permanecer como histórico do processo, mas não substitui os arquivos canônicos aprovados.

Os `README.md` estruturais permanecem em suas respectivas pastas durante toda a campanha. Eles descrevem a função da pasta e não devem ser apagados apenas porque outros arquivos passaram a existir ali.

Fichas reservadas de antagonistas não impedem o encerramento da criação e não precisam existir antecipadamente. O narrador pode criá-las depois, quando algum antagonista realmente passar a exigir continuidade própria.

A partir daqui a aventura está pronta para jogar.

> **Só começar a primeira cena depois que a revisão estiver concluída.**

---

## 19. Retomar uma criação interrompida

Se uma campanha já possui `criacao.md` com `Status geral: EM CRIAÇÃO`, não iniciar outra criação e não presumir que a aventura já está pronta para jogar.

Ler `criacao.md`, localizar a primeira etapa ainda não concluída ou a revisão pendente e continuar daquele ponto.

Exemplo:

```text
1. Direção narrativa e cenário: PENDENTE DE REVISÃO
   - Diretrizes narrativas: APROVADO
   - Cenário: PENDENTE DE REVISÃO
2. Protagonista: PENDENTE DE REVISÃO
3. Personagens relevantes: EM ANDAMENTO
4. Início da história: NÃO INICIADO
```

Nesse caso, a parte conceitual já avançou até a Etapa 3, mas a revisão futura ainda deverá resolver o cenário pendente sem reabrir as diretrizes já aprovadas.

Se a criação conceitual já terminou e a revisão foi interrompida, localizar qual arquivo, personagem e qual **campo ou bloco** ainda estão pendentes e continuar dali, sem recomeçar partes já aprovadas.

> **Não perguntar ao jogador onde parou quando o próprio arquivo de criação consegue responder.**

---

## 20. Resumo operacional

```text
NOVA CAMPANHA
↓
Perguntar nome
↓
Criar estrutura completa + README.md em cada pasta estrutural + criacao.md
↓
1. DIREÇÃO NARRATIVA E CENÁRIO
que tipo de história? → diretrizes/narracao.md
em que mundo? → mundo/cenario.md
ambos → PENDENTE DE REVISÃO
↓
2. PROTAGONISTA
conceito + CONTROLE + ficha estrutural → PENDENTE DE REVISÃO
↓
3. PERSONAGENS RELEVANTES
elenco + proposta de CONTROLE; aliados podem começar só com nomes/controle + fichas estruturais vazias → PENDENTE DE REVISÃO
↓
4. INÍCIO DA HISTÓRIA
situação inicial concreta → PENDENTE DE REVISÃO
↓
REVISÃO
diretrizes/narracao.md
↓
mundo/cenario.md
↓
personagens relevantes/NPCs visíveis → 4 blocos por personagem; CONTROLE no Bloco 1
↓
protagonista POR ÚLTIMO → CONTROLE e campos simples individualmente; ATRIBUTOS, PERÍCIAS e PODERES como blocos
↓
ficha completa → aprovação final
↓
início da história
↓
APROVAR ARQUIVOS
↓
criar estado/atual.md + atualizar README.md da raiz da aventura
↓
COMEÇAR A CAMPANHA

DURANTE A CAMPANHA
JOGADOR IA → IA joga permanentemente conforme ficha, conhecimento, diretrizes e situação
JOGADOR EVENTUAL IA → IA decide quando ativar/desativar; sem nova autorização por cena após aprovação da ficha
NPC → permanece sob narrador; só vira eventual se CONTROLE for alterado com aprovação do usuário
inimigo comum → modelo rápido, sem arquivo obrigatório
antagonista importante/recorrente/poderoso → ficha opcional em mestre/viloes/, reservada ao narrador
README.md estrutural → permanece explicando a função da pasta
```

---

## Regra final

> **Criar uma campanha não é preencher uma ficha gigante antes de jogar. É primeiro descobrir que tipo de história o jogador quer viver e em que mundo ela acontece, fazer poucas perguntas úteis, preservar cada etapa, organizar o conceito, revisar sem recriar, calibrar cada personagem por si mesmo e começar assim que houver uma base sólida aprovada. A direção narrativa fica em `diretrizes/narracao.md`; a realidade do mundo fica em `mundo/cenario.md`. A estrutura completa da campanha, com um `README.md` explicativo em cada pasta estrutural, nasce assim que o nome é definido. As fichas em `personagens/` também registram `CONTROLE`, permitindo distinguir Jogador Humano, Jogador IA, Jogador Eventual IA e NPC. O usuário decide essa categoria; depois de um personagem ser aprovado como Jogador Eventual IA, a IA decide quando ativar ou desativar seu ciclo próprio de jogador. O personagem do jogador humano recebe revisão campo por campo, com ATRIBUTOS, PERÍCIAS e PODERES como blocos próprios; os demais personagens apresentáveis são revisados em quatro blocos. Inimigos comuns não exigem burocracia; antagonistas ocultos podem ter continuidade própria sem entregar seus segredos ao jogador.**