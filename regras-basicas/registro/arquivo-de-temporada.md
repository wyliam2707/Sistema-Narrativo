# Arquivo de Temporada

Status: CANÔNICO / ATUAL

Esta regra define como organizar o **Livro depois que uma temporada é encerrada** e como transformar o arco concluído em uma unidade histórica reutilizável por temporadas futuras.

Ela complementa `livro-e-capitulos.md`, `salvar-a-historia.md` e `../CRIACAO-DE-TEMPORADA.md`.

> **A temporada encerrada vira uma unidade histórica. Os capítulos preservam o que aconteceu; o epílogo preserva como terminou; o resumo facilita reancoragem; o mapa de eventos facilita localizar quando e onde cada mudança ocorreu.**

## Estrutura obrigatória depois do encerramento

Quando uma temporada for encerrada, seu material literário deve ser agrupado em:

```text
campanhas/<nome>/livro/temporada-[N]/
├── README.md
├── 001.md
├── 002.md
├── ...
├── epilogo.md
├── resumo-da-temporada.md
└── mapa-de-eventos.md
```

Os nomes numéricos representam os capítulos pertencentes àquela temporada.

Uma temporada nova pode reiniciar a numeração em `001.md`, porque a pasta da temporada já fornece o escopo. Em campanhas antigas que utilizavam numeração global, a migração pode preservar os números existentes para não reescrever o cânone sem necessidade.

## Unidade histórica

Depois do arquivamento:

```text
livro/temporada-[N]/
→ unidade histórica completa da temporada encerrada.
```

O diretório raiz `livro/` deixa de acumular capítulos soltos de temporadas já encerradas.

Durante uma temporada ativa, os capítulos podem ser gravados diretamente dentro da pasta da temporada ativa quando ela já existir:

```text
livro/temporada-[N]/001.md
livro/temporada-[N]/002.md
...
```

Se uma campanha antiga ainda grava capítulos na raiz durante o arco, o encerramento deve agrupá-los antes da criação da próxima temporada.

## Autoridade dos arquivos

Os arquivos dentro da temporada possuem funções diferentes.

### Capítulos

```text
001.md, 002.md, ...
→ histórico literário canônico detalhado.
```

Continuam seguindo `livro-e-capitulos.md`.

Eles registram o que realmente aconteceu e preservam decisões, ações, descobertas, relações, consequências e causalidade.

### Epílogo

```text
epilogo.md
→ estado narrativo de encerramento da temporada.
```

O epílogo responde como o arco terminou sem decidir o próximo arco.

A partir desta regra, o destino padrão do epílogo de uma temporada arquivada é:

```text
campanhas/<nome>/livro/temporada-[N]/epilogo.md
```

Esta localização substitui, para temporadas organizadas segundo esta regra, a convenção antiga de manter `temporada-[N]-epilogo.md` solto na raiz de `livro/`.

### Resumo da temporada

```text
resumo-da-temporada.md
→ ponte operacional entre a temporada encerrada e temporadas futuras.
```

O resumo existe para permitir carregar o passado relevante sem precisar reler todos os capítulos antes de cada novo arco.

Pode consolidar:

```text
premissa e problema da temporada;
linha geral da resolução;
principais descobertas;
mudanças de mundo;
evolução das relações;
conhecimentos importantes adquiridos;
objetivos concluídos;
consequências ainda existentes;
problemas realmente abertos;
ponto final do arco.
```

O resumo não é uma nova fonte capaz de criar fatos.

```text
CAPÍTULOS + EPÍLOGO + FONTES CANÔNICAS PERTINENTES
→ determinam a verdade.

RESUMO
→ condensa essa verdade.
```

Se o resumo contradizer uma fonte canônica mais específica:

```text
→ corrigir o resumo.
→ não corrigir o cânone para fazê-lo caber no resumo.
```

O resumo não substitui:

```text
FICHA
→ quem a personagem é e o que precisa lembrar.

ESTADO ATUAL
→ como a campanha está agora.

NARRATIVA
→ identidade persistente da campanha.

ROTEIRO
→ arco ativo.

OPOSITOR
→ processos adversariais vivos.
```

### Mapa de eventos

```text
mapa-de-eventos.md
→ índice cronológico e causal da temporada.
```

O mapa permite localizar rapidamente acontecimentos sem reler toda a prosa.

Cada entrada pode registrar, quando útil:

```text
MOMENTO / DIA / PERÍODO
→ quando ocorreu.

CAPÍTULO
→ onde o acontecimento está registrado.

EVENTO
→ o que aconteceu de forma objetiva.

CONSEQUÊNCIA
→ o que mudou por causa disso.

CONHECIMENTO
→ quem passou a saber o quê, quando isso for importante.

RELAÇÕES
→ mudança relacional consolidada naquele ponto, quando houver.
```

Exemplo:

```text
Dia 6 | Cap. 013
Evento: Corvin completa o Ciclo da Vida diante de Ravena e Estelar.
Consequência: ambas passam a conhecer a morte e renovação natural de Corvin.
Conhecimento: Ravena e Estelar sabem que o ciclo existe; ainda não significa conhecer toda possível exceção não revelada.
```

O mapa também é derivado.

Ele não pode:

- criar cena que não aconteceu;
- transformar hipótese em fato;
- entregar conhecimento a quem não o possuía;
- decidir motivação ambígua;
- substituir o capítulo como autoridade quando detalhes importarem.

## README da temporada

`README.md` funciona como índice curto da unidade histórica.

Deve apontar para:

```text
intervalo de capítulos;
epilogo.md;
resumo-da-temporada.md;
mapa-de-eventos.md;
roteiro arquivado correspondente em mestre/temporadas/.
```

Pode informar título ou identificação da temporada e status `ENCERRADA`.

Não precisa repetir o resumo inteiro.

## Fechamento atualizado da temporada

Quando a condição de encerramento for alcançada, o procedimento completo passa a ser:

```text
1. concluir somente a situação em resolução;
2. fechar o último capítulo real;
3. escrever o epílogo;
4. consolidar fichas, Estado, mundo e processos afetados;
5. arquivar o roteiro em mestre/temporadas/temporada-[N].md;
6. agrupar os capítulos em livro/temporada-[N]/;
7. criar/atualizar README.md da temporada;
8. criar resumo-da-temporada.md;
9. criar mapa-de-eventos.md;
10. atualizar referências que apontavam para caminhos antigos;
11. reancorar o sistema;
12. perguntar “E agora?”.
```

Nenhuma dessas etapas autoriza avançar a ficção.

```text
ORGANIZAR A TEMPORADA
≠
JOGAR A PRÓXIMA TEMPORADA
```

## Uso na criação da temporada seguinte

Para uma temporada que não é a primeira, a entrada recomendada passa a ser:

```text
mestre/narrativa.md
+ resposta a “E agora?”
+ livro/temporada-[N-1]/resumo-da-temporada.md
+ livro/temporada-[N-1]/epilogo.md
+ fichas consolidadas
+ estado consolidado
+ problemas/processos ainda vivos pertinentes
```

`mapa-de-eventos.md` é consultado quando cronologia, origem de conhecimento, sequência de relação ou localização de um acontecimento anterior realmente importar.

Os capítulos completos são consultados quando for necessário recuperar detalhes específicos, fala, causalidade fina ou contexto que o resumo/mapa não preserve suficientemente.

```text
RESUMO
→ contexto rápido.

MAPA
→ localização cronológica.

CAPÍTULO
→ detalhe canônico completo.
```

## Conhecimento continua compartimentado

O resumo e o mapa podem registrar fatos conhecidos pelo responsável da campanha sem transformar isso em conhecimento de todas as personagens.

```text
ARQUIVO SABE
≠
PERSONAGEM SABE
```

Quando a origem do conhecimento for importante, o mapa deve indicar quem descobriu ou presenciou o fato.

As fichas continuam sendo a fonte operacional principal do conhecimento que uma personagem precisa levar para decisões recorrentes.

## Migração de campanhas existentes

Ao aplicar esta regra a uma campanha já em andamento:

```text
1. identificar quais capítulos pertencem a cada temporada encerrada;
2. mover os arquivos sem alterar seu conteúdo literário;
3. mover/renomear o epílogo para `epilogo.md`;
4. gerar resumo e mapa somente a partir do cânone existente;
5. atualizar referências em README, Estado, roteiro e outros arquivos afetados;
6. não promover a reorganização de arquivos a mudança ficcional.
```

Mover arquivo não cria uma nova versão da história.

```text
CAMINHO MUDOU
→ organização mudou.

CONTEÚDO CANÔNICO
→ permanece o mesmo.
```

## Regra final

> **Cada temporada encerrada deve tornar-se uma unidade histórica em `livro/temporada-[N]/`. Capítulos e epílogo continuam preservando o cânone; `resumo-da-temporada.md` condensa o arco para reancoragem e `mapa-de-eventos.md` indexa sua cronologia e causalidade. Resumo e mapa são derivados e nunca substituem Ficha, Estado, Narrativa, Roteiro ou os capítulos quando houver divergência. A reorganização ocorre antes de “E agora?” virar uma nova temporada e nunca avança a ficção por si mesma.**
