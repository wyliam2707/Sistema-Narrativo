# Manual de Registro da Campanha

Status: REFORMULAÇÃO / NÃO IMPLEMENTADO

Esta pasta é o **manual de persistência da história**.

Ela explica como transformar acontecimentos já julgados e narrados em arquivos permanentes dentro de:

```text
campanhas/<nome>/
```

`regras-basicas/registro/` contém somente regras e modelos.

Nenhum fato vivo de uma campanha deve ser salvo aqui.

> **O jogo acontece na mesa. O Registro preserva o que precisa continuar verdadeiro depois da resposta.**

## Função do Registro

O Registro responde:

```text
SOBRE O QUE A CAMPANHA É AO LONGO DAS TEMPORADAS?
→ mestre/narrativa.md.

QUAL É O ARCO ATIVO AGORA?
→ mestre/roteiro.md.

QUEM É A PERSONAGEM E O QUE ELA PRECISA LEMBRAR PARA SER INTERPRETADA?
→ ficha da personagem.

O QUE ACONTECEU?
→ Livro / histórico canônico.

COMO A CAMPANHA ESTÁ AGORA?
→ Estado Atual.

O QUE É VERDADE EXTERNA À PERSONAGEM?
→ mundo, livros e demais fontes apropriadas.

O QUE CONTINUA EXISTINDO FORA DA CENA?
→ processos, prazos, planos e outras fontes apropriadas.
```

Registrar não cria ficção.

```text
DECLARAÇÃO
→ intenção.

JULGAMENTO / RESOLUÇÃO
→ estabelece realidade.

NARRAÇÃO
→ apresenta a realidade.

REGISTRO
→ preserva a realidade que precisa sobreviver.
```

## Arquitetura deste manual

```text
registro/
├── README.md
├── fontes-da-campanha.md
├── salvar-a-historia.md
├── estado-atual.md
└── livro-e-capitulos.md
```

### `fontes-da-campanha.md`

Explica onde cada tipo de verdade deve ser salvo.

> **Cada verdade deve ter uma fonte principal.**

### `salvar-a-historia.md`

Manual operacional para salvar sem avançar a ficção, incluindo o fechamento de temporada.

### `estado-atual.md`

Define a fotografia operacional necessária para retomar a campanha exatamente de onde ela parou.

### `livro-e-capitulos.md`

Define o histórico canônico do que realmente aconteceu.

## Estrutura recomendada de uma campanha

```text
campanhas/<nome>/
├── README.md
├── personagens/
├── estado/
│   └── atual.md
├── mundo/
├── mestre/
│   ├── narrativa.md
│   ├── roteiro.md
│   └── temporadas/
├── opositor/
└── livro/
```

Função de cada área:

```text
README
→ identidade, estado geral e roteamento da campanha.

PERSONAGENS
→ fichas reais; principal fonte de interpretação de cada personagem.

ESTADO
→ como a campanha precisa ser retomada agora.

MUNDO
→ verdades estáveis do cenário.

MESTRE / NARRATIVA
→ identidade persistente da campanha.

MESTRE / ROTEIRO
→ temporada ativa.

MESTRE / TEMPORADAS
→ roteiros já encerrados e arquivados.

OPOSITOR
→ planos, processos e informações do outro lado da trama.

LIVRO
→ o que efetivamente aconteceu, incluindo epílogos de temporada.
```

## Narrativa e roteiro

A direção da história possui duas camadas.

### `mestre/narrativa.md`

Preserva o que não deve ser redescoberto ou reinventado a cada temporada:

```text
foco principal
gênero e tom
experiência desejada
temas e conflitos recorrentes
o que não deve dominar
premissas gerais
```

Ela é a identidade persistente da campanha.

### `mestre/roteiro.md`

Preserva somente o arco atual:

```text
situação inicial
foco aplicado
trama de fundo
prazo ou processo
miniquests ou variações
direção da temporada
condição de encerramento
```

O roteiro não é histórico nem Estado Atual. Ele não registra cada cena e não determina resultados.

Quando sua condição de encerramento é alcançada, ele deixa de dirigir a campanha atual, é arquivado em `mestre/temporadas/`, e o Narrador escreve o epílogo antes de perguntar **“E agora?”**.

Uma miniquest pode terminar, surgir outra e o Estado pode mudar sem que a Narrativa da Campanha seja reescrita.

Mudança real da identidade da campanha deve ser deliberada; não acontece automaticamente porque uma trama secundária ficou interessante.

## Ficha e memória da personagem

A ficha é a principal fonte de interpretação da personagem.

Quando um fato adquirido passa a ser importante para decisões futuras, relações, evolução emocional ou leitura recorrente de situações, ele deve ser consolidado em `Conhecimento relevante` ou no bloco apropriado da própria ficha.

```text
se esquecer provavelmente faria a personagem agir de forma incoerente nesta história
→ consolidar na ficha.

se importa apenas para o momento atual
→ Estado Atual.

se é contexto externo já bem guardado em livro, mundo ou outra fonte
→ não duplicar integralmente na ficha.
```

O que merece consolidação depende da Narrativa da Campanha e da Temporada. Romance, terror, investigação e ação podem tornar informações diferentes importantes para interpretação.

Conhecimento consolidado não deve ser tratado novamente como descoberta apenas porque a campanha foi retomada depois.

## Verdade estabelecida x informação disponível

Um fato pode ser verdadeiro na campanha sem ser conhecido por todas as personagens.

```text
CAMPANHA SABE
≠
PERSONAGEM SABE
```

Arquivos podem permanecer visíveis no repositório, mas informação reservada não pode ser usada por uma personagem que ainda não a descobriu.

Relações registradas na ficha representam o ponto de vista do dono daquela ficha. A percepção de outra personagem só entra como conhecimento quando for legitimamente conhecida.

## Registrar somente fatos concluídos

Nunca salvar como acontecimento algo que ainda é somente intenção, hipótese ou plano.

```text
JOGADOR
→ vou procurar Ravena amanhã.

NÃO SALVAR COMO HISTÓRIA
→ encontrou Ravena amanhã.
```

Pode ser preservado, quando relevante:

```text
INTENÇÃO ATUAL
→ pretende procurar Ravena amanhã.
```

Da mesma forma, um plano futuro do Opositor permanece plano até realmente acontecer.

## Processos e prazos

Um resultado pode continuar vivo mesmo fora da cena.

Exemplo:

```text
Dick inicia investigação.
NARRADOR estabelece: primeiras pistas em 10 dias.
```

Salvar:

```text
Processo: investigação de Dick
Estado: em andamento
Prazo: primeiras pistas em 10 dias
```

O processo não precisa ser redeclarado em toda janela distante.

## Fechamento de temporada

Quando a condição de encerramento do roteiro for alcançada:

```text
→ parar no resultado real
→ escrever epílogo
→ consolidar fichas e Estado
→ arquivar o roteiro encerrado
→ perguntar “E agora?”
```

O epílogo responde as perguntas relevantes para aquele tipo de campanha e registra apenas o que realmente ficou estabelecido.

```text
EPÍLOGO
→ resultado real da temporada.

PROBLEMAS ABERTOS
→ continuam verdadeiros.

PROBLEMAS ABERTOS
≠
próxima temporada obrigatória.
```

A próxima temporada só nasce depois da nova direção fornecida pelo usuário, conforme `../CRIACAO-DE-TEMPORADA.md`.

## Duplicação legítima

Uma mesma realidade pode aparecer em duas fontes quando cada uma possui função diferente.

```text
LIVRO
→ registra que a personagem descobriu um fato.

FICHA / CONHECIMENTO RELEVANTE
→ preserva o fato que ela precisa continuar sabendo.
```

Outro exemplo:

```text
LIVRO
→ registra que houve um ferimento.

ESTADO ATUAL
→ preserva as marcas de Vida que ainda estão presentes.
```

Isso não é duplicação ruim porque cada fonte responde a uma pergunta diferente.

## Salvamento não joga

Quando o usuário pedir para salvar, registrar, fechar capítulo ou fechar temporada:

- parar no último fato estabelecido;
- não criar uma cena extra;
- não resolver ação ainda pendente;
- não decidir pelo jogador;
- não executar automaticamente plano futuro;
- não inventar consequência para produzir fechamento;
- não criar a próxima temporada durante o epílogo.

```text
SALVAR
→ preservar.

SALVAR
≠
continuar jogando.
```

## Dados vivos ficam somente em `campanhas/`

Isso inclui:

- narrativa da campanha;
- roteiro da temporada ativa;
- roteiros arquivados;
- fichas reais;
- relações consolidadas;
- conhecimento relevante;
- Estado Atual;
- Vida, Mente, Mana e condições atuais;
- acontecimentos;
- capítulos e epílogos;
- mundo;
- processos;
- prazos;
- eventos futuros já estabelecidos;
- planos do Opositor;
- registros do Mestre.

Recursos permanentes pertencem à ficha; recursos temporários podem pertencer ao Estado Atual quando precisarem ser acompanhados.

## Regra final

> **Registro é a memória canônica da campanha. A Narrativa preserva a identidade persistente; o Roteiro preserva a temporada ativa; a ficha preserva a interpretação da personagem; o Livro preserva o passado; o Estado preserva o presente. Quando a temporada termina, o epílogo consolida o resultado e a próxima só nasce depois de “E agora?”.**