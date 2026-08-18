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

Antes de qualquer pergunta de cenário, perguntar:

> **Qual será o nome da campanha?**

Assim que o nome for definido, criar a estrutura da aventura em:

```text
aventuras/<nome-da-campanha>/
├── README.md
├── criacao.md
├── diretrizes/
├── personagens/
├── mestre/
│   └── viloes/
├── mundo/
├── relacionamento/
├── progressao/
├── cronologia/
├── estado/
└── livro/
```

`mestre/` é uma área reservada ao narrador. Ela pode conter informações que precisam existir de forma persistente sem serem apresentadas ao jogador durante a sessão. `mestre/viloes/` é o local padrão para fichas ocultas de antagonistas importantes quando forem necessárias.

Essa área não é tecnicamente privada para o proprietário do repositório; “reservada” significa apenas que o narrador ou outra IA não deve revelar espontaneamente seu conteúdo durante o RPG.

Em sistemas de armazenamento que não preservam pastas vazias, as pastas podem ser materializadas conforme seus primeiros arquivos forem criados.

Criar imediatamente `criacao.md` para registrar o andamento.

Modelo inicial:

```text
# Criação da Campanha

Status geral: EM CRIAÇÃO

1. Cenário: NÃO INICIADO
2. Protagonista: NÃO INICIADO
3. Personagens relevantes: NÃO INICIADO
4. Início da história: NÃO INICIADO

Revisão final: NÃO INICIADA
```

---

## 3. Regra de perguntas

Durante as quatro etapas conceituais:

- fazer **uma pergunta por vez**, exceto quando um pequeno bloco puder ser respondido de forma mais eficiente;
- não pedir informação que já possa ser inferida das respostas anteriores;
- não transformar a criação em questionário enciclopédico;
- se o jogador disser `decida você`, escolher uma opção coerente e continuar;
- parar de perguntar quando já houver informação suficiente para aquela etapa;
- detalhes menores podem ser criados durante a própria campanha quando passarem a importar.

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

## 5. Etapa 1 — Cenário

Objetivo: definir **o suficiente do mundo e da proposta para sustentar os personagens e a história inicial**.

Perguntar uma coisa por vez conforme necessário. Exemplos de informação que podem importar:

- universo ou tipo de cenário;
- gênero;
- foco da campanha;
- tom;
- local principal;
- época, se relevante;
- se for fanfic, grau de fidelidade ao cânone;
- adaptações gerais desejadas;
- elementos obrigatórios já declarados pelo jogador.

Não perguntar detalhes sem utilidade imediata apenas para preencher o mundo.

Se o jogador escolher um universo conhecido, o narrador pode usar seu conhecimento para preencher detalhes secundários e deve perguntar apenas quando existir uma escolha de adaptação que realmente importe.

### Fechamento da etapa

Quando houver cenário suficiente:

1. consolidar as decisões;
2. criar ou atualizar `mundo/cenario.md`;
3. marcar no arquivo:

```text
Status: PENDENTE DE REVISÃO
```

4. atualizar em `criacao.md`:

```text
1. Cenário: PENDENTE DE REVISÃO
```

5. seguir para a Etapa 2 sem iniciar ainda a revisão.

---

## 6. Etapa 2 — Protagonista

Objetivo: criar **o protagonista como pessoa e conceito**, ainda sem calibrar sua ficha numérica.

Começar pela identidade, não pela mecânica.

Perguntar uma coisa por vez conforme necessário, normalmente seguindo algo próximo de:

- nome;
- aparência física;
- imagem de referência, quando fornecida;
- idade real e aparente, quando diferentes;
- natureza/origem relevante;
- personalidade;
- comportamento social;
- história essencial;
- trajetória de vida ou ocupações importantes;
- situação e motivação atuais.

Não perguntar sobre cada detalhe biográfico se ele não for necessário para compreender o personagem.

### Imagens de referência

Quando o jogador fornecer uma imagem, ela pode ser usada para construir a descrição visual do personagem. O arquivo deve guardar a **descrição consolidada**, não depender exclusivamente da imagem para que outra IA compreenda a aparência.

### Ficha estrutural desde o começo

O arquivo do protagonista deve usar, desde esta etapa, a estrutura final de ficha sempre que ela já for conhecida.

Preencher apenas o que já foi definido conceitualmente. Campos mecânicos ainda desconhecidos permanecem **em branco**.

> **Nunca usar `[0]` para representar informação desconhecida. Zero é um valor mecânico real.**

Campos conceituais podem incluir, quando relevantes:

- identidade;
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

Esses elementos pertencem à revisão posterior.

### Fechamento da etapa

Quando o conceito do protagonista estiver suficiente:

1. organizar o conceito em `personagens/<nome>.md`;
2. manter a estrutura da ficha, deixando em branco o que ainda não foi definido;
3. marcar:

```text
Status: PENDENTE DE REVISÃO
```

4. atualizar `criacao.md`:

```text
2. Protagonista: PENDENTE DE REVISÃO
```

5. seguir para a Etapa 3.

---

## 7. Etapa 3 — Personagens relevantes

Objetivo: definir **qual é o elenco inicial que merece acompanhamento como Central ou Relevante**.

O protocolo não precisa perguntar ao jogador por todo personagem óbvio de um cenário conhecido.

Quando o universo escolhido já indicar personagens naturalmente relevantes, o narrador pode identificá-los e propor sua inclusão.

### Personagens canônicos ou licenciados

Quando forem usados personagens existentes, perguntar de forma simples se o jogador quer:

- base canônica;
- base canônica flexível;
- adaptação mais livre.

Se uma adaptação específica já foi declarada — idade diferente, fase específica, relação alterada etc. — registrá-la sem exigir nova confirmação desnecessária.

Preservar identidade, personalidade, poderes e relações essenciais conforme o grau de fidelidade escolhido.

### Criação conceitual mínima de aliados

Durante esta etapa, pode ser suficiente definir apenas **a quantidade de aliados relevantes e seus nomes**.

Se isso for tudo que o jogador quiser decidir naquele momento:

1. criar `personagens/<nome>.md` usando o modelo oficial de Personagem Relevante;
2. preencher somente o que já foi realmente estabelecido;
3. deixar os demais campos em branco;
4. não inventar aparência, personalidade, história, capacidades ou recursos apenas para completar a ficha;
5. desenvolver esses elementos durante a revisão posterior.

Se o jogador disser `decida você`, `faça por mim` ou delegar de forma equivalente, o narrador pode propor esses detalhes, mas eles continuam sujeitos ao fluxo normal de revisão e aprovação.

> **Nome definido pode bastar para fechar a criação conceitual de um aliado. Detalhe faltante não precisa ser inventado antes da revisão.**

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

Preencher tudo que já for conhecido conceitualmente e deixar os campos ainda não definidos **em branco**.

Não inventar valores apenas para preencher a ficha.

> **Campo desconhecido fica em branco. `[0]` continua sendo um valor real, nunca um marcador de pendência.**

Cada arquivo permanece:

```text
Status: PENDENTE DE REVISÃO
```

A ficha conceitual pode conter identidade, descrição, `TRAÇOS`, personalidade, história, desejos, medos e outras informações já consolidadas. A mecânica será revisada depois.

Fichas reservadas em `mestre/viloes/` usam o modelo próprio definido em `sistema/modelos.md` e não entram neste fluxo de aprovação aberta.

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

Depois que Cenário, Protagonista, Personagens relevantes e Início da história estiverem organizados, iniciar a revisão.

A revisão serve para:

- corrigir conceitos;
- confirmar o que será canônico;
- aplicar atributos, perícias, poderes e demais regras;
- verificar coerência entre cenário e personagens;
- preparar o estado inicial real da campanha.

> **Conceito primeiro. Mecânica depois.**

> **Revisar não significa recriar.**

Durante toda a revisão:

- preservar exatamente o que já foi consolidado;
- não reescrever ou embelezar conteúdo aprovado sem necessidade;
- localizar apenas o que ainda está pendente;
- apresentar blocos curtos;
- explicar números brevemente quando isso ajudar;
- depois da correção, reapresentar o bloco normalizado para aprovação.

Fichas reservadas do narrador não são apresentadas nesta revisão. Elas obedecem às regras de `mestre/viloes/` e ao princípio de não revelar informação oculta.

---

## 10. Revisão do cenário

Apresentar `mundo/cenario.md` ao jogador de forma organizada.

O jogador pode:

- aprovar;
- corrigir;
- acrescentar;
- remover.

Depois da confirmação, marcar:

```text
Status: APROVADO
```

O cenário passa a ser fonte válida da aventura.

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

## 13. Método de revisão de uma ficha

Revisar **um personagem por vez**.

Fluxo padrão:

> **Abrir ficha → preservar consolidado → localizar pendências → revisar bloco por bloco → apresentar ficha completa → aprovação → salvar como APROVADO → próximo personagem.**

Esse fluxo se aplica às fichas apresentáveis ao jogador. Fichas reservadas em `mestre/viloes/` não passam pela apresentação final e seguem a regra específica da Seção 14.

### Conteúdo conceitual

Revisar primeiro todo o conceito:

- identidade;
- descrição;
- `TRAÇOS`, se houver;
- personalidade e tendências;
- história consolidada;
- desejos/objetivos atuais;
- medos/limites relevantes.

Se o conteúdo já existir, apresentá-lo como está para aprovação ou correção.

Se estiver em branco, perguntar ou propor conforme o tipo de personagem.

Somente depois de todo o conceito estar revisado iniciar os valores mecânicos.

### Blocos mecânicos simples

Campos simples e ordenados podem ser apresentados juntos.

Exemplo:

```text
ATR: FOR [ ] | AGI [ ] | RES [ ] | MEN [ ] | VON [ ]
```

O jogador pode responder de forma compacta, e o narrador normaliza para o formato do sistema.

Quando o narrador estiver propondo os valores, pode incluir **uma linha breve de explicação por item** para facilitar a revisão.

### Perícias

Apresentar o bloco de perícias junto.

Para personagens canônicos ou NPCs, propor apenas perícias relevantes ao personagem, sem criar uma lista enciclopédica.

Perícias não listadas continuam em `+0` quando necessárias pelas regras gerais do sistema.

### Poderes

Poderes podem exigir revisão iterativa.

O jogador pode descrever em linguagem comum ou abreviada; o narrador deve normalizar para a sintaxe do sistema e reapresentar para correção.

Quando uma lista estiver aberta, perguntar se existe mais algum poder antes de fechar o bloco.

Sempre que possível, manter **um poder completo por linha**, incluindo suas especializações.

Exemplo:

```text
Alma Astral [3] => Projeção [3] / Manifestação [3] / Contenção [3] / Telecinese [2] / Voo [2]
```

### Equipamento e recursos

Registrar apenas equipamento recorrente ou recursos persistentes que realmente importem para a personagem.

Não inventar itens para preencher o campo.

Instalações, laboratórios, oficinas ou recursos fixos podem ser registrados de forma descritiva quando fizerem parte permanente das capacidades disponíveis ao personagem.

### Relações

Revisar também `REL` antes de fechar a ficha.

Registrar apenas relações **atuais, recorrentes e estabelecidas**.

Personagens canônicos podem receber proposta baseada em suas relações conhecidas e nas adaptações da campanha.

Sentimentos, romances ou relações planejadas para acontecer no futuro **não entram antecipadamente em `REL`**.

> **A relação nasce ou muda quando isso acontece na ficção.**

### Campos irrelevantes

Se um campo não possuir importância real para aquela personagem, ele pode permanecer vazio.

Não inventar conteúdo apenas para completar visualmente uma ficha.

---

## 14. Personagens canônicos, NPCs e antagonistas ocultos na revisão

Para personagens canônicos, licenciados ou já conhecidos, o narrador pode propor o conteúdo com base em:

- identidade canônica escolhida;
- continuidade definida para a campanha;
- adaptações já aprovadas;
- conceito consolidado daquela personagem.

A revisão deve ocorrer **bloco por bloco, do topo da ficha para baixo**.

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
- só deve mudar quando acontecimentos reais da ficção justificarem a mudança.

Sempre que for prático, definir capacidades ocultas relevantes antes de usá-las diretamente contra o protagonista.

> **O narrador pode esconder a informação; não pode mudar a realidade depois de descobrir a solução do jogador.**

---

## 15. Revisão do protagonista — sempre por último entre as fichas

Somente depois de todas as fichas iniciais de personagens relevantes/NPCs **apresentáveis ao jogador** terem sido revisadas, abrir a ficha do protagonista.

O conceito já consolidado deve ser preservado.

Não perguntar novamente aquilo que já foi decidido.

A participação do jogador é direta na definição dos blocos ainda pendentes, normalmente:

1. atributos;
2. perícias;
3. poderes;
4. equipamento ou recursos recorrentes;
5. relações iniciais recorrentes;
6. qualquer outro campo realmente necessário.

O narrador pode organizar, normalizar sintaxe e apontar incoerências com as regras, mas não deve recalibrar o protagonista para aproximá-lo dos NPCs já revisados.

A mesma regra vale nos dois sentidos:

> **NPCs não são balanceados com o protagonista, e o protagonista não é balanceado com os NPCs.**

Fichas ocultas de antagonistas não servem como régua para o protagonista e não são comparadas a ele durante a revisão.

---

## 16. Aprovação final de cada ficha

Quando todos os blocos de uma personagem **apresentável ao jogador** estiverem revisados, apresentar **a ficha completa** ao jogador.

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

4. seguir para a próxima ficha.

Não carregar correções descartadas, explicações de conversa ou versões intermediárias para a ficha final.

Fichas reservadas em `mestre/viloes/` são a exceção. Elas usam:

```text
Status: CANÔNICO DO MESTRE
Visibilidade: MESTRE
```

e não são exibidas ao jogador para aprovação.

---

## 17. Revisão do início da história

Depois que cenário e fichas estiverem aprovados, revisar `estado/inicio.md` como **o começo concreto da história**.

Apresentar a base consolidada, ajustar com o jogador e reapresentar até aprovação.

Verificar se o início é coerente com:

- capacidades reais dos personagens;
- relações estabelecidas;
- cenário;
- localização;
- informação disponível;
- motivações atuais;
- tom da campanha.

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
3. preparar o `README.md` da aventura como porta de entrada da campanha.

---

## 18. Encerramento da criação

Quando tudo estiver aprovado, `criacao.md` deve ficar aproximadamente assim:

```text
# Criação da Campanha

Status geral: CONCLUÍDA

1. Cenário: APROVADO
2. Protagonista: APROVADO
3. Personagens relevantes: APROVADOS
4. Início da história: APROVADO

Revisão final: CONCLUÍDA
```

`criacao.md` pode permanecer como histórico do processo, mas não substitui os arquivos canônicos aprovados.

Fichas reservadas de antagonistas não impedem o encerramento da criação e não precisam existir antecipadamente. O narrador pode criá-las depois, quando algum antagonista realmente passar a exigir continuidade própria.

A partir daqui a aventura está pronta para jogar.

> **Só começar a primeira cena depois que a revisão estiver concluída.**

---

## 19. Retomar uma criação interrompida

Se uma campanha já possui `criacao.md` com `Status geral: EM CRIAÇÃO`, não iniciar outra criação e não presumir que a aventura já está pronta para jogar.

Ler `criacao.md`, localizar a primeira etapa ainda não concluída ou a revisão pendente e continuar daquele ponto.

Exemplo:

```text
1. Cenário: PENDENTE DE REVISÃO
2. Protagonista: PENDENTE DE REVISÃO
3. Personagens relevantes: EM ANDAMENTO
4. Início da história: NÃO INICIADO
```

Nesse caso, retomar pela Etapa 3.

Se a criação conceitual já terminou e a revisão foi interrompida, localizar qual ficha ou bloco ainda está pendente e continuar dali, sem recomeçar as fichas já aprovadas.

> **Não perguntar ao jogador onde parou quando o próprio arquivo de criação consegue responder.**

---

## 20. Resumo operacional

```text
NOVA CAMPANHA
↓
Perguntar nome
↓
Criar pasta + criacao.md
↓
1. CENÁRIO
perguntas úteis → organizar → PENDENTE DE REVISÃO
↓
2. PROTAGONISTA
conceito + ficha estrutural → PENDENTE DE REVISÃO
↓
3. PERSONAGENS RELEVANTES
elenco; aliados podem começar só com nomes + fichas estruturais vazias → PENDENTE DE REVISÃO
↓
4. INÍCIO DA HISTÓRIA
situação inicial concreta → PENDENTE DE REVISÃO
↓
REVISÃO
cenário
↓
fichas dos personagens relevantes/NPCs visíveis, uma por vez
↓
ficha do protagonista POR ÚLTIMO
↓
início da história
↓
APROVAR ARQUIVOS
↓
criar estado/atual.md
↓
COMEÇAR A CAMPANHA

DURANTE A CAMPANHA
inimigo comum → modelo rápido, sem arquivo obrigatório
antagonista importante/recorrente/poderoso → ficha opcional em mestre/viloes/, reservada ao narrador
```

---

## Regra final

> **Criar uma campanha não é preencher uma ficha gigante antes de jogar. É fazer poucas perguntas úteis, preservar cada etapa, organizar o conceito, revisar sem recriar, calibrar cada personagem por si mesmo e começar assim que houver uma base sólida aprovada. Inimigos comuns não exigem burocracia; antagonistas ocultos podem ter continuidade própria sem entregar seus segredos ao jogador.**
