# Correção e Substituição de Cânone

Status: APROVADO

Correção de cânone existe para substituir uma informação incorreta, contraditória ou registrada de forma errada sem criar duas realidades concorrentes.

> **Existe uma única versão canônica de cada fato. Quando uma correção é aprovada, a versão corrigida substitui a anterior.**

## Aprovação obrigatória

Toda correção de cânone exige aprovação explícita do JOGADOR HUMANO antes de entrar em vigor.

Podem apontar inconsistências ou propor correções:

```text
JOGADOR HUMANO
JOGADOR IA
JOGADOR IA EVENTUAL
OPOSITOR
NARRADOR
```

Nenhuma dessas funções pode substituir unilateralmente um fato já estabelecido.

> **Sem confirmação do JOGADOR HUMANO, não existe correção de cânone.**

## Discussão

Uma correção pode ser debatida antes da decisão final.

Cada persona pode apresentar argumento quando possuir fundamento relevante.

```text
JOGADOR HUMANO
→ lembrança, intenção original, interpretação e preferência.

JOGADOR IA
→ coerência das ações, conhecimentos e decisões da própria peça.

JOGADOR IA EVENTUAL
→ o mesmo pelas peças eventuais que estiver representando.

OPOSITOR
→ contradições, consequências e problemas lógicos relevantes.

NARRADOR
→ fatos canônicos, continuidade, regras, conhecimento reservado necessário e consequências dependentes.
```

O NARRADOR não decide a correção por autoridade narrativa. Ele apresenta os fatos disponíveis e os efeitos da alteração.

A decisão final pertence ao JOGADOR HUMANO.

## Fluxo

```text
1. Identificar erro ou inconsistência.
2. Expor o fato atual e a correção proposta.
3. Consultar somente as fontes relevantes.
4. Permitir argumentos das personas pertinentes.
5. Ajustar a proposta quando necessário.
6. JOGADOR HUMANO aprova, recusa ou define ajuste final.
7. Somente após aprovação a correção entra em vigor.
8. PERSISTÊNCIA alinha todas as fontes realmente afetadas.
```

## Correção não é acontecimento ficcional

Uma correção altera o cânone fora da ficção. Ela não cria uma nova cena.

```text
Versão errada:
Corvin entrou pela porta.

Correção aprovada:
Corvin entrou pela janela.
```

Depois da correção, o cânone é simplesmente:

```text
Corvin entrou pela janela.
```

A versão anterior deixa de ser válida.

## Uma única versão vigente

O Git pode preservar o histórico técnico das edições, mas os arquivos atuais da campanha devem representar somente o cânone vigente.

Não usar o Livro como changelog de erros.

## Propagação

Depois da aprovação, revisar apenas as fontes cuja validade realmente depende do fato corrigido.

Podem ser afetados:

```text
livro/
estado/atual.md
personagens/
mundo/
mestre/
```

Não alterar arquivos por associação superficial.

## Consequências dependentes

Se uma consequência existia apenas por causa do fato corrigido, ela também precisa ser removida ou ajustada.

Se possuía fundamento independente, continua válida.

Exemplo:

```text
Correção:
Trigon não matou o guarda.
```

Se a polícia o procurava exclusivamente por esse assassinato, esse fio deve ser corrigido.

Se também o procura por crimes independentes já estabelecidos, a investigação pode continuar por esses outros fundamentos.

> **A correção altera o que dependia do fato substituído. Fundamentos independentes permanecem.**

## Agência não pode ser reescrita por conveniência

Ações de peças controladas por JOGADOR HUMANO, JOGADOR IA ou JOGADOR IA EVENTUAL não podem ser trocadas retroativamente apenas para melhorar a história.

Se o Livro registrou uma ação incorretamente, a correção deve restaurar aquilo que realmente foi declarado e estabelecido.

Quando houver divergência genuína de interpretação, as personas pertinentes podem argumentar antes da decisão final do JOGADOR HUMANO.

## Material reservado

Fatos canônicos em `mestre/` também obedecem a este protocolo.

```text
FATO CANÔNICO RESERVADO
→ correção exige aprovação.

PLANO ainda não executado
→ pode mudar sem correção de cânone.

POSSIBILIDADE
→ pode ser descartada ou substituída livremente.
```

A discussão pode preservar o segredo mostrando apenas o fundamento necessário para avaliar a correção.

## Correção não cria dificuldade retroativa

Não usar correção para responder a uma solução eficaz dos jogadores.

Exemplo inválido:

```text
JOGADOR
→ encontra uma entrada pelo telhado.

DEPOIS DA SOLUÇÃO
→ “Correção: sempre existiu uma barreira invisível no telhado.”
```

Se a barreira não era fato ou preparação válida antes, isso é criação retroativa, não correção.

O mesmo vale para poder, imunidade, recurso, guarda, armadilha, conhecimento, aliança, preparação ou regra local inventados depois para alterar o resultado.

> **Correção resolve erro de continuidade. Não corrige o sucesso dos jogadores.**

## Livro

Se uma correção aprovada afeta capítulo já salvo, corrigir o próprio capítulo afetado.

Não criar novo capítulo apenas para registrar a correção.

## Fechamento de capítulo

Se uma inconsistência for descoberta durante o fechamento, não corrigi-la silenciosamente.

Quando a correção for necessária para consolidar corretamente:

```text
parar
→ apresentar a inconsistência
→ discutir se necessário
→ obter aprovação do JOGADOR HUMANO
→ aplicar correção
→ continuar o fechamento
```

Se não for necessário resolver naquele momento, não inventar uma versão para preencher a lacuna.

## Regra final

> **Todos podem apontar e argumentar. O JOGADOR HUMANO confirma. Depois da confirmação, a versão corrigida substitui a anterior e somente as fontes realmente afetadas são alinhadas à nova verdade.**