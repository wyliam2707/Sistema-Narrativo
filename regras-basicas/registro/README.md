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
├── fechar-capitulo.md
├── estado-atual.md
├── livro-e-capitulos.md
├── arquivo-de-temporada.md
├── canonizacao-e-correcoes.md
└── reancoragem-operacional.md
```

### `fontes-da-campanha.md`

Explica onde cada tipo de verdade deve ser salvo.

> **Cada verdade deve ter uma fonte principal.**

### `salvar-a-historia.md`

Manual operacional para salvar sem avançar a ficção, incluindo o fechamento de temporada.

### `fechar-capitulo.md`

Define o comando **`fechar o capítulo`** como checkpoint completo:

```text
salvar
→ atualizar
→ reset operacional
→ recarregar
→ continuar
```

O reset não apaga o cânone. Ele faz regras e fontes consolidadas voltarem a ser a base principal antes do próximo capítulo.

### `estado-atual.md`

Define a fotografia operacional necessária para retomar a campanha exatamente de onde ela parou.

### `livro-e-capitulos.md`

Define o histórico canônico do que realmente aconteceu.

### `arquivo-de-temporada.md`

Define como uma temporada encerrada vira uma unidade histórica em:

```text
livro/temporada-[N]/
```

A pasta reúne capítulos, epílogo, `resumo-da-temporada.md` e `mapa-de-eventos.md`.

Capítulos e epílogo preservam o cânone detalhado. Resumo e mapa são derivados de consulta e reancoragem e nunca substituem Ficha, Estado, Narrativa, Roteiro ou capítulo quando houver divergência.

`arquivo-de-temporada.md` é a regra específica para a localização e organização de temporadas encerradas e, nesse escopo, prevalece sobre exemplos antigos que mantenham epílogos ou capítulos encerrados soltos na raiz de `livro/`.

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
    ├── README.md
    ├── temporada-1/
    ├── temporada-2/
    └── ...
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
→ o que efetivamente aconteceu, organizado por temporada quando os arcos forem encerrados.
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

Quando sua condição de encerramento é alcançada, ele deixa de dirigir a campanha atual, é arquivado em `mestre/temporadas/`, e o Narrador conclui o procedimento de arquivo da temporada antes de perguntar **“E agora?”**.

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

## Fechamento de capítulo

O comando **`fechar o capítulo`** possui função especial e segue `fechar-capitulo.md`.

Durante a fase de salvamento:

- parar no último fato estabelecido;
- não criar cena extra;
- não resolver ação pendente;
- não decidir pelo jogador;
- não fabricar fechamento dramático.

Depois que o capítulo foi consolidado e as fontes atualizadas:

```text
→ resetar o operacional
→ recarregar regras e fontes essenciais
→ continuar a partir do Estado Atual
```

Assim, o próximo capítulo não depende da inércia de uma conversa muito longa para lembrar como o sistema deve funcionar.

## Fechamento de temporada

Quando a condição de encerramento do roteiro for alcançada:

```text
→ parar no resultado real
→ fechar o último capítulo real
→ escrever o epílogo
→ consolidar fichas e Estado
→ arquivar o roteiro encerrado
→ agrupar capítulos em livro/temporada-[N]/
→ criar/atualizar README da temporada
→ criar resumo-da-temporada.md
→ criar mapa-de-eventos.md
→ atualizar referências para os novos caminhos
→ reancorar
→ perguntar “E agora?”
```

O procedimento detalhado está em `arquivo-de-temporada.md`.

O epílogo responde as perguntas relevantes para aquele tipo de campanha e registra apenas o que realmente ficou estabelecido.

```text
EPÍLOGO
→ resultado real da temporada.

RESUMO DA TEMPORADA
→ condensação derivada para reancoragem.

MAPA DE EVENTOS
→ índice cronológico e causal derivado.

PROBLEMAS ABERTOS
→ continuam verdadeiros.

PROBLEMAS ABERTOS
≠
próxima temporada obrigatória.
```

A próxima temporada só nasce depois da nova direção fornecida pelo usuário, conforme `../CRIACAO-DE-TEMPORADA.md`.

## Uso do arquivo anterior na temporada seguinte

Ao preparar uma temporada posterior, usar normalmente:

```text
mestre/narrativa.md
+ resposta a “E agora?”
+ resumo-da-temporada da temporada anterior
+ epílogo da temporada anterior
+ fichas consolidadas
+ Estado consolidado
+ processos/problemas ainda vivos pertinentes
```

Consultar `mapa-de-eventos.md` quando a cronologia ou origem de conhecimento importar e abrir capítulos completos somente quando o detalhe canônico for necessário.

Isso reduz o carregamento sem transformar resumo ou mapa em novas fontes de verdade.

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

O mesmo vale para resumo e mapa, desde que sejam tratados explicitamente como derivados e não como autoridade concorrente.

## Salvar não joga

Quando o usuário pedir apenas para **salvar** ou **registrar**:

- parar no último fato estabelecido;
- não criar uma cena extra;
- não resolver ação ainda pendente;
- não decidir pelo jogador;
- não executar automaticamente plano futuro;
- não inventar consequência para produzir fechamento.

```text
SALVAR
→ preservar.

SALVAR
≠
continuar jogando.
```

Isso é diferente do comando `fechar o capítulo`, que inclui continuação **depois** do salvamento, reset e reancoragem.

`Fechar temporada` também não continua para um novo arco: termina em **“E agora?”**.

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
- capítulos, epílogos, resumos e mapas de temporadas;
- mundo;
- processos;
- prazos;
- eventos futuros já estabelecidos;
- planos do Opositor;
- registros do Mestre.

Recursos permanentes pertencem à ficha; recursos temporários podem pertencer ao Estado Atual quando precisarem ser acompanhados.

## Regra final

> **Registro é a memória canônica da campanha. A Narrativa preserva a identidade persistente; o Roteiro preserva a temporada ativa; a ficha preserva a interpretação da personagem; o Livro preserva o passado; o Estado preserva o presente. Temporadas encerradas são agrupadas conforme `arquivo-de-temporada.md`: capítulos e epílogo preservam o cânone, enquanto resumo e mapa facilitam reancoragem sem competir com as fontes principais. `Fechar o capítulo` acrescenta um reset operacional entre capítulos; `fechar temporada` consolida também sua unidade histórica antes de perguntar “E agora?”.**
