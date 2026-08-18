# Protocolo de Criação de Campanha

Este documento define **como criar uma nova campanha** usando o Sistema Narrativo.

O objetivo é evitar formulários longos, não perder decisões durante a conversa e separar claramente **criação conceitual** de **revisão mecânica**.

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
├── mundo/
├── relacionamento/
├── progressao/
├── cronologia/
├── estado/
└── livro/
```

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

- fazer **uma pergunta por vez**;
- não pedir informação que já possa ser inferida das respostas anteriores;
- não transformar a criação em questionário enciclopédico;
- se o jogador disser `decida você`, escolher uma opção coerente e continuar;
- parar de perguntar quando já houver informação suficiente para aquela etapa;
- detalhes menores podem ser criados durante a própria campanha quando passarem a importar.

> **Perguntar apenas aquilo que o jogador realmente precisa decidir.**

---

## 4. Regra de salvamento e revisão

Cada etapa passa por este fluxo:

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

5. seguir para a Etapa 2 sem iniciar ainda a revisão mecânica.

---

## 6. Etapa 2 — Protagonista

Objetivo: criar **o protagonista como pessoa e conceito**, ainda sem convertê-lo para números.

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

### O que NÃO fazer nesta etapa

Ainda não definir:

- FOR, AGI, RES, MEN ou VON;
- graus de perícia;
- graus de poderes;
- custos ou economia mecânica;
- ficha numérica completa.

Esses elementos pertencem à revisão posterior.

### Fechamento da etapa

Quando o conceito do protagonista estiver suficiente:

1. organizar o conceito em `personagens/<nome>.md`;
2. marcar:

```text
Status: PENDENTE DE REVISÃO
```

3. manter apenas o conceito narrativo nesta fase;
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

Esses personagens futuros não precisam ser previstos no protocolo. Se ganharem importância durante a campanha, podem ser promovidos para Relevantes ou Centrais e receber ficha apropriada.

### Arquivos nesta fase

Para cada personagem do elenco inicial, criar `personagens/<nome>.md` com o conceito disponível e:

```text
Status: PENDENTE DE REVISÃO
```

Nesta fase, uma ficha de personagem canônico pode ser mínima, por exemplo:

```text
# Ravena
Status: PENDENTE DE REVISÃO
Importância: Central
Base: canônica flexível
Adaptações:
- 26 anos
```

Não é obrigatório aplicar ainda os valores numéricos do sistema.

Atualizar `criacao.md`:

```text
3. Personagens relevantes: PENDENTE DE REVISÃO
```

Depois seguir para a Etapa 4.

---

## 8. Etapa 4 — Início da história

Objetivo: definir **a situação necessária para começar a primeira cena**, não planejar a campanha inteira.

Perguntar uma coisa por vez apenas sobre o que for necessário, por exemplo:

- onde a história começa;
- situação imediata do protagonista;
- por que os personagens entram em contato;
- acontecimento imediatamente anterior relevante;
- o que está acontecendo quando a cena abre;
- ponto exato em que o jogador recebe controle.

Não exigir:

- vilão final;
- estrutura em três atos;
- capítulos futuros;
- resultado planejado do romance;
- solução antecipada dos conflitos;
- arcos fechados antes de jogar.

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

## 11. Revisão do protagonista

Para o protagonista do jogador, a aplicação mecânica deve ser feita com participação direta dele.

Perguntar uma categoria por vez, por exemplo:

1. definir atributos;
2. definir perícias;
3. definir poderes;
4. definir equipamento recorrente, se houver;
5. definir relações iniciais recorrentes, se houver.

A ordem pode ser adaptada se o conceito exigir.

Depois, montar a ficha completa no formato do sistema e apresentá-la ao jogador.

A ficha continua:

```text
Status: PENDENTE DE REVISÃO
```

até o jogador aprovar o conjunto.

Só então marcar:

```text
Status: APROVADO
```

---

## 12. Revisão dos personagens relevantes

Para personagens canônicos ou conhecidos, o narrador pode **propor a ficha mecânica completa** com base no conceito e no grau de fidelidade escolhido.

Apresentar para revisão do jogador.

O jogador pode corrigir antes da aprovação.

Para NPCs originais criados pelo narrador, o narrador também pode propor a ficha quando ela for necessária para agência e resolução.

Nenhuma proposta automática se torna definitiva apenas porque foi escrita.

> **Ficha proposta não é ficha aprovada.**

Quando aprovada, marcar cada arquivo como:

```text
Status: APROVADO
```

---

## 13. Revisão do início da história

Depois que cenário e fichas estiverem aprovados, revisar `estado/inicio.md` para garantir que o começo é coerente com:

- capacidades reais dos personagens;
- relações estabelecidas;
- cenário;
- localização;
- informação disponível;
- tom da campanha.

Depois da aprovação:

1. marcar `estado/inicio.md` como `APROVADO`;
2. criar `estado/atual.md` com o ponto operacional exato em que a campanha começa;
3. preparar o `README.md` da aventura como porta de entrada da campanha.

---

## 14. Encerramento da criação

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

A partir daqui a aventura está pronta para jogar.

> **Só começar a primeira cena depois que a revisão estiver concluída.**

---

## 15. Retomar uma criação interrompida

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

> **Não perguntar ao jogador onde parou quando o próprio arquivo de criação consegue responder.**

---

## 16. Resumo operacional

```text
NOVA CAMPANHA
↓
Perguntar nome
↓
Criar pasta + criacao.md
↓
1. CENÁRIO
perguntas uma a uma → organizar → PENDENTE DE REVISÃO
↓
2. PROTAGONISTA
conceito apenas → organizar → PENDENTE DE REVISÃO
↓
3. PERSONAGENS RELEVANTES
definir elenco → criar arquivos conceituais → PENDENTE DE REVISÃO
↓
4. INÍCIO DA HISTÓRIA
definir apenas o começo → organizar → PENDENTE DE REVISÃO
↓
REVISÃO
cenário → protagonista + mecânica → NPCs + mecânica → início
↓
APROVAR ARQUIVOS
↓
criar estado/atual.md
↓
COMEÇAR A CAMPANHA
```

## Regra final

> **Criar uma campanha não é preencher uma ficha gigante antes de jogar. É fazer poucas perguntas úteis, preservar cada etapa, organizar o conceito, revisar com o jogador, aplicar a mecânica e começar assim que houver uma base sólida.**