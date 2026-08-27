# Livro

Status: APROVADO

O Livro é o **registro histórico canônico da campanha em forma literária**.

Ele preserva, como conto ou romance, aquilo que realmente aconteceu na ficção.

> **O Livro guarda a história. Ele não é a fonte operacional padrão de retomada.**

## Destino concreto

```text
campanhas/<nome>/livro/
```

Cada capítulo consolidado registra uma unidade narrativa já ocorrida.

## Função

As fontes cumprem funções diferentes:

```text
estado/atual.md
→ como continuar agora.

personagens/
→ quem as peças com agência são.

mundo/
→ verdades estáveis do cenário.

mestre/
→ NPCs e material reservado ainda operacional.

livro/
→ a história que aconteceu, contada literariamente.
```

O Livro não precisa repetir STATUS atuais, planos futuros ou fichas completas apenas para preservar informação operacional.

## Forma obrigatória

O capítulo consolidado deve ser escrito como **história em terceira pessoa**, com fluxo de conto ou romance.

Não usar como forma principal:

- resumo técnico;
- relatório de sessão;
- lista de acontecimentos;
- log de rolagens;
- transcrição de declarações operacionais;
- seção de ficha ou estado ao fim do capítulo.

Falas diretas seguem:

```text
[Nome] — Fala.
```

Pensamentos diretos legitimamente estabelecidos seguem:

```text
[Nome, pensa] — Pensamento.
```

As regras completas de fala, pensamento e Detecção [Mentiras] pertencem a `../narracao/fala-e-interioridade.md`.

## Protagonismo compartilhado

Personagens controlados por JOGADOR HUMANO e JOGADORES IA que participam da história são tratados como **protagonistas compartilhados**.

Isso não obriga divisão matemática de páginas ou parágrafos.

Obriga a consolidação a respeitar quem realmente teve iniciativa, foco e agência em cada trecho.

O Livro não deve:

- transformar o personagem humano no motor de toda cena quando outra peça a iniciou;
- rebaixar JOGADORES IA a acompanhantes passivos;
- apagar contribuições próprias de uma protagonista;
- reescrever uma sequência coletiva como façanha individual;
- mudar o foco apenas para favorecer uma peça específica.

Pode alternar a câmera literária entre protagonistas conforme a cena.

> **Todos os jogadores relevantes são protagonistas; o foco acompanha a história, não uma hierarquia artificial de câmera.**

JOGADOR IA EVENTUAL e NPCs podem receber foco literário quando isso for importante para a cena, sem obrigação de se tornarem protagonistas permanentes.

## O que entra

Registrar acontecimentos realmente estabelecidos, como:

- ações executadas;
- decisões;
- falas relevantes;
- deslocamentos relevantes;
- descobertas;
- conflitos e resultados;
- mudanças de situação;
- consequências;
- acontecimentos secretos que realmente ocorreram;
- ordem causal necessária para compreender a história;
- interioridade legitimamente estabelecida quando fizer sentido literário.

## O que não entra como fato

Não registrar como acontecimento consumado:

- intenção ainda não executada;
- plano futuro;
- possibilidade;
- proposta recusada;
- versão descartada durante resolução;
- hipótese ainda não confirmada;
- correção já substituída por outra versão canônica;
- pensamento, emoção ou motivação inventados retrospectivamente.

> **Plano não é acontecimento. Possibilidade não é cânone histórico. Interioridade não estabelecida não vira verdade só para melhorar a prosa.**

## Agência exercida

A consolidação deve preservar toda decisão realmente exercida por personagens controlados por:

```text
JOGADOR HUMANO
JOGADOR IA
JOGADOR IA EVENTUAL
```

A forma literária pode condensar repetição ou melhorar transições, mas não pode:

- apagar decisão relevante;
- trocar quem realizou a ação;
- substituir recusa por aceitação;
- inventar motivação decisiva não estabelecida;
- alterar resultado já julgado;
- atribuir iniciativa a quem apenas reagiu.

> **A prosa pode mudar. A agência exercida não.**

## Cena e condensação

O Livro **não é transcrição integral da sessão**.

Trechos de percurso, procedimento, investigação repetitiva, deslocamento ou rotina podem ser condensados quando o processo detalhado não possui peso dramático próprio.

Ao condensar, preservar quando relevantes:

- contribuição distinta de cada protagonista;
- pistas necessárias;
- uma ou algumas falas marcantes;
- humor, tensão ou dinâmica de relação;
- a descoberta ou mudança que encerra a sequência.

Exemplo de princípio:

```text
investigação com várias etapas
→ pode virar poucos parágrafos de prosa
→ mantém as contribuições de Corvin, Ravena e Estelar
→ preserva uma ou duas falas importantes
→ desacelera novamente quando surge o portal ou outra descoberta decisiva.
```

> **Condensar percurso, procedimento e repetição. Expandir descoberta, conflito, relação, decisão e revelação.**

A regra completa pertence a `../narracao/dramatizacao-e-resumo.md`.

## Falas

O Livro não precisa reproduzir cada fala funcional ocorrida durante a mesa.

Preservar especialmente falas que:

- definem decisão;
- alteram relação;
- revelam personalidade;
- produzem humor relevante;
- contêm informação importante;
- marcam uma descoberta;
- são necessárias para compreender causa e consequência.

Diálogo repetitivo ou meramente operacional pode ser resumido em prosa, desde que seu efeito canônico permaneça correto.

## Pensamentos

O Livro pode usar `[Nome, pensa] —` para diferentes protagonistas, respeitando `../narracao/fala-e-interioridade.md`.

Pensamento direto precisa ser legitimamente sustentado pela agência ou interioridade estabelecida daquela peça.

O Livro não inventa a mente de uma personagem para justificar retrospectivamente o que ela fez.

## Mecânica não é prosa obrigatória

Declarações como:

```text
JOGADOR IA — Ravena
OPOSITOR
NARRADOR — JULGAMENTO
resultado 23
Dificuldade 18
+1d
```

não aparecem no Livro como estrutura operacional.

O acontecimento produzido por essas regras é convertido em ficção.

Quando uma mecânica for diegética e realmente conhecida pelas personagens, ela pode aparecer naturalmente pela própria ficção.

## Detecção [Mentiras]

Quando uma mentira conscientemente falsa foi percebida por uma personagem com Detecção [Mentiras] ou capacidade equivalente, o Livro preserva a convenção visual definida em `../narracao/fala-e-interioridade.md`:

> **somente o menor fragmento reconhecido como falso fica em negrito.**

Não acrescentar explicação dizendo qual é a verdade ou que a habilidade “reagiu”, salvo se isso também tiver sido expressamente narrado por outro motivo.

## OPOSITOR

O OPOSITOR não aparece como personagem do Livro.

Quando uma ação proposta por ele realmente acontece, registrar a peça ficcional responsável.

```text
OPOSITOR
→ propõe uma ação de Trigon.

NARRADOR
→ julga a situação.

SE A AÇÃO ACONTECE
→ Livro registra Trigon realizando a ação.
```

Uma proposta que não aconteceu não entra no Livro.

## Acontecimentos secretos

O Livro pode preservar acontecimentos que nenhuma personagem protagonista presenciou, desde que eles realmente tenham ocorrido.

Isso não concede automaticamente conhecimento às personagens.

```text
CONHECIMENTO DO LEITOR
≠
CONHECIMENTO DA PERSONAGEM
```

Se uma campanha preferir não revelar determinado acontecimento reservado ao leitor naquele momento, ele pode continuar operacionalmente em `mestre/` até o ponto adequado de consolidação, desde que o cânone não seja perdido.

## Relação com `estado/atual.md`

Livro e Estado Atual não competem.

```text
LIVRO
→ histórico literário.

ESTADO ATUAL
→ presente operacional.
```

Quando um fato deixa de importar para a retomada, ele pode sair de `estado/atual.md` sem desaparecer da história, porque permanece no Livro.

## Relação com correção de cânone

Quando uma correção for aprovada, aplicar `correcao-de-canone.md`.

O capítulo afetado deve representar apenas a versão canônica vigente.

O histórico técnico do Git pode preservar edições antigas; o Livro não funciona como changelog de erros.

## Regra final

> **O Livro responde “o que realmente aconteceu?” em forma de conto ou romance em terceira pessoa. Preserva protagonismo compartilhado, falas e pensamentos identificados, condensa o que não precisa ocupar cena e expande o que merece ser vivido. `estado/atual.md` continua respondendo “como continuamos agora?”.**
