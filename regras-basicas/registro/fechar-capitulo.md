# Fechar Capítulo — Reset Operacional

Status: REFORMULAÇÃO / NÃO IMPLEMENTADO

Este arquivo define o comportamento do comando **`fechar o capítulo`** durante uma campanha.

Variações equivalentes, como `fechar capítulo` ou sem acento, usam o mesmo protocolo.

> **Fechar o capítulo é salvar a história, atualizar as fontes, fazer um reset operacional e reancorar a IA antes de continuar.**

## Função do comando

O comando existe para impedir que uma sessão longa degrade gradualmente:

- regras de agência;
- interpretação das personagens;
- tom e foco da campanha;
- direção da temporada;
- critérios de julgamento do Narrador;
- separação entre conhecimento técnico e conhecimento das personagens.

Ele não apaga o que aconteceu.

Ele transforma o capítulo encerrado em fontes canônicas e faz essas fontes voltarem a ser a base operacional do próximo capítulo.

```text
CONVERSA DO CAPÍTULO
→ matéria que acabou de ser jogada.

LIVRO + ESTADO + FICHAS + OUTRAS FONTES ATUALIZADAS
→ memória canônica depois do fechamento.

MODELO OPERACIONAL REANCORADO
→ modo de operação do próximo capítulo.
```

## Protocolo

Ao receber `fechar o capítulo`:

```text
1. PARAR
2. CONSOLIDAR
3. ATUALIZAR
4. RESETAR O OPERACIONAL
5. RECARREGAR E REANCORAR
6. CONTINUAR
```

## 1 — Parar

Parar exatamente no último fato legitimamente estabelecido.

Antes de salvar:

- não criar despedida;
- não terminar uma conversa que ainda não terminou;
- não avançar para a manhã seguinte;
- não executar evento futuro;
- não decidir reação ainda pendente;
- não fabricar cliffhanger.

O fechamento não cria um final melhor. Ele usa o ponto em que a ficção realmente chegou.

## 2 — Consolidar

Transformar o trecho encerrado em capítulo do Livro conforme `livro-e-capitulos.md`.

O Livro preserva:

```text
o que realmente aconteceu
quem decidiu o quê
mudanças de relação
consequências
descobertas
passagem de tempo relevante
causa e efeito necessários para continuidade
```

A forma literária pode melhorar. O cânone não muda.

## 3 — Atualizar

Depois de consolidar o capítulo, atualizar somente as fontes realmente afetadas.

```text
estado/atual.md
→ ponto exato de continuação.

fichas
→ somente mudanças consolidadas de personagem, relação ou conhecimento que precisem permanecer disponíveis.

mundo/
→ somente verdade estável que mudou.

opositor/
→ planos, processos e prazos que continuem vivos ou tenham mudado.

mestre/
→ somente informação operacional que realmente mudou.
```

Seguir `salvar-a-historia.md`.

Detalhe transitório que não precisa continuar verdadeiro não precisa ser promovido a registro permanente.

## 4 — Reset operacional

Depois que o capítulo foi salvo e as fontes foram atualizadas, considerar encerrado o contexto operacional daquele capítulo.

Isso **não significa apagar literalmente a conversa**. Significa mudar a hierarquia usada para continuar.

```text
ANTES DO FECHAMENTO
→ conversa recente ainda participa diretamente da operação.

DEPOIS DO FECHAMENTO
→ fontes canônicas atualizadas passam a ser a base operacional principal.
```

Não continuar carregando como autoridade:

- interpretações provisórias;
- detalhes transitórios não consolidados;
- intenções já encerradas;
- hipóteses descartadas;
- leituras antigas substituídas por atualização de ficha ou Estado;
- hábitos narrativos que surgiram apenas por repetição durante o capítulo.

Se algo do capítulo precisa continuar importando, deve estar recuperável no Livro ou em alguma fonte operacional apropriada.

> **Reset operacional não apaga o passado. Ele impede que ruído acumulado da conversa substitua regras e fontes canônicas.**

## 5 — Recarregar e reancorar

Antes de narrar o próximo capítulo, reancorar a operação conforme:

```text
registro/reancoragem-operacional.md
```

A reancoragem não significa apenas abrir arquivos. Ela reconstrói uma representação funcional e integrada do Motor, das personagens e do presente.

### Sempre recarregar

```text
regras-basicas/nucleo/1.0-tribunal.md
regras-basicas/nucleo/1.3-jogador-ia.md
regras-basicas/mestre/README.md
regras-basicas/mestre/julgamento.md
regras-basicas/mestre/perspectiva-e-fala.md
regras-basicas/mestre/ritmo-e-descricao.md

campanhas/<nome>/mestre/narrativa.md
campanhas/<nome>/mestre/roteiro.md
campanhas/<nome>/estado/atual.md
fichas das personagens relevantes
```

Se houver `JOGADOR IA EVENTUAL` ativo ou provável na abertura, recarregar também:

```text
regras-basicas/nucleo/1.4-jogador-ia-eventual.md
```

Depois de carregar essas fontes, formar o modelo operacional descrito em `reancoragem-operacional.md` antes de continuar a ficção.

### Recarregar sob demanda

Consultar somente quando o próximo trecho realmente precisar:

```text
romance / intimidade
→ mestre/intimidade-e-romance.md

criação de cenário ou histórico menor
→ nucleo/1.7-criacao-emergente.md

combate, dano, Mana, movimento ou outra resolução específica
→ regra mecânica pertinente

registro adicional
→ arquivo pertinente de registro/
```

Se o foco persistente da campanha depender fortemente de uma regra específica — por exemplo romance — essa regra pode fazer parte da reancoragem normal daquela campanha.

Uma consulta específica deve detalhar ou corrigir o modelo já carregado; não deve substituir o restante do Motor por uma regra isolada.

Não reler `regras-basicas/` inteiro sem necessidade.

> **Recarregar o núcleo operacional, formar a imagem integrada e consultar especialidades sob demanda.**

## 6 — Continuar

Depois da reancoragem, continuar a campanha a partir de `estado/atual.md`.

Não presumir passagem de tempo nem uma nova decisão humana apenas porque começou outro capítulo.

```text
ESTADO DIZ QUE A CENA CONTINUA
→ novo capítulo pode abrir exatamente dali.

ESTADO TERMINOU NUMA NOVA ESCOLHA HUMANA
→ apresentar a situação e devolver a decisão.

ESTADO PERMITE AVANÇO SEM NOVA ESCOLHA
→ continuar normalmente.
```

O novo capítulo usa as fontes reancoradas como base, não a inércia narrativa do capítulo anterior.

## Se o capítulo também encerrou a temporada

Se a condição de encerramento de `mestre/roteiro.md` foi alcançada, o fechamento de temporada tem precedência sobre a abertura automática de outro capítulo.

```text
FECHAR CAPÍTULO
→ consolidar e atualizar
→ reset operacional
→ recarregar e reancorar
→ reconhecer que a temporada terminou
→ escrever epílogo
→ arquivar roteiro
→ perguntar “E agora?”
```

Não abrir uma nova temporada ou novo arco antes da resposta a **“E agora?”**.

## Checklist

```text
[ ] parei no último fato real?
[ ] capítulo foi consolidado no Livro?
[ ] Estado Atual representa exatamente a continuação?
[ ] fichas só receberam mudanças realmente consolidadas?
[ ] processos, prazos e Opositor foram atualizados quando necessário?
[ ] deixei de tratar ruído transitório da conversa como fonte principal?
[ ] recarreguei o núcleo operacional?
[ ] recarreguei narrativa, roteiro, estado e fichas relevantes?
[ ] formei o modelo integrado conforme reancoragem-operacional.md?
[ ] consultei regras específicas somente se necessárias?
[ ] continuei sem inventar passagem de tempo ou decisão humana?
[ ] se a temporada terminou, parei em “E agora?”?
```

## Regra final

> **`Fechar o capítulo` significa: consolidar o passado, atualizar o presente, resetar o contexto operacional, recarregar as regras e fontes essenciais, reancorá-las como um modelo integrado e só então continuar. O Livro preserva o que aconteceu; o Estado mostra de onde continuar; as fichas preservam quem as personagens são; e a reancoragem impede que uma sessão longa substitua o sistema por hábitos narrativos acumulados.**