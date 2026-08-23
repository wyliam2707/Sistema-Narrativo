# Livro

Status: APROVADO

O Livro é o **registro histórico canônico da campanha**.

Ele preserva, em forma literária, aquilo que realmente aconteceu na ficção.

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
→ o que aconteceu.
```

O Livro não precisa repetir STATUS atuais, planos futuros ou fichas completas apenas para preservar informação operacional.

## O que entra

Registrar acontecimentos realmente estabelecidos, como:

- ações executadas;
- decisões;
- falas;
- deslocamentos relevantes;
- descobertas;
- conflitos e resultados;
- mudanças de situação;
- consequências;
- acontecimentos secretos que realmente ocorreram;
- ordem causal necessária para compreender a história.

## O que não entra como fato

Não registrar como acontecimento consumado:

- intenção ainda não executada;
- plano futuro;
- possibilidade;
- proposta recusada;
- versão descartada durante resolução;
- hipótese ainda não confirmada;
- correção já substituída por outra versão canônica.

> **Plano não é acontecimento. Possibilidade não é cânone histórico.**

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
- alterar resultado já julgado.

> **A prosa pode mudar. A agência exercida não.**

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

## Forma literária

A forma de escrita pertence a:

```text
../narracao/
```

Especialmente:

- `apresentacao-da-cena.md`;
- `fala-e-interioridade.md`;
- `ritmo-e-descricao.md`;
- `dramatizacao-e-resumo.md`.

O Livro não redefine ponto de vista, estilo, romance, humor, diálogo ou ritmo dentro de Persistência.

A direção narrativa local da campanha continua prevalecendo sobre o padrão geral quando explicitamente definida.

## Consolidação não é transcrição

O Livro não é cópia bruta do chat.

A consolidação pode:

- remover metaconversa;
- remover comandos administrativos;
- retirar discussão de regras;
- condensar repetição;
- melhorar transições;
- converter descrição mecânica em prosa;
- resumir passagem de tempo sem importância dramática.

Não pode:

- inventar acontecimento;
- alterar decisão;
- trocar o autor de uma ação;
- modificar consequência já estabelecida;
- criar retrospectivamente segredo, poder, recurso ou preparação;
- transformar possibilidade em fato.

> **Consolidar melhora a forma sem reescrever a realidade.**

## Relação com `estado/atual.md`

Livro e Estado Atual não competem.

```text
LIVRO
→ histórico.

ESTADO ATUAL
→ presente operacional.
```

Quando um fato deixa de importar para a retomada, ele pode sair de `estado/atual.md` sem desaparecer da história, porque permanece no Livro.

## Relação com correção de cânone

Quando uma correção for aprovada, aplicar `correcao-de-canone.md`.

O capítulo afetado deve representar apenas a versão canônica vigente.

O histórico técnico do Git pode preservar edições antigas; o Livro não funciona como changelog de erros.

## Regra final

> **O Livro responde “o que realmente aconteceu?”. `estado/atual.md` responde “como continuamos agora?”. A forma literária pertence a `narracao/`, e Persistência garante que o passado canônico não seja perdido nem reescrito silenciosamente.**