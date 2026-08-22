# Correção e Substituição de Cânone

Status: APROVADO

Correção de cânone existe para substituir uma informação incorreta, contraditória ou registrada de forma errada sem criar duas realidades concorrentes dentro da campanha.

> **Existe apenas uma versão canônica de cada fato. Quando uma correção é aprovada, a versão corrigida substitui a anterior.**

## Aprovação obrigatória do JOGADOR HUMANO

Toda correção de cânone exige aprovação explícita do JOGADOR HUMANO antes de entrar em vigor.

Isso vale independentemente de quem identificou o erro:

```text
MESTRE / NARRADOR
JOGADOR IA
JOGADOR IA EVENTUAL
OPOSITOR
ou qualquer outra fonte de revisão
```

Todos podem apontar inconsistências, erros ou possíveis correções.

Nenhum deles pode substituir unilateralmente um fato já estabelecido.

> **Sem aprovação do JOGADOR HUMANO, não existe correção de cânone.**

O fluxo é:

```text
1. Alguém identifica uma inconsistência ou erro.
2. O MESTRE / NARRADOR apresenta claramente o fato atual e a correção proposta.
3. O JOGADOR HUMANO aprova, recusa ou ajusta.
4. Somente após aprovação a correção substitui a versão anterior.
5. A PERSISTÊNCIA atualiza todos os registros realmente afetados.
```

## Correção não é acontecimento ficcional

Uma correção feita fora da ficção altera a realidade canônica; ela não cria uma nova cena nem um novo acontecimento dentro da história.

Exemplo:

```text
Versão registrada por engano:
Corvin entrou pela porta.

Correção aprovada:
Corvin entrou pela janela.
```

Depois da correção, o cânone é simplesmente:

```text
Corvin entrou pela janela.
```

Não significa que Corvin entrou pela porta e depois voltou no tempo ou mudou de entrada.

A versão anterior deixa de ser canônica.

## Uma única versão válida

Não manter duas versões contraditórias como igualmente verdadeiras.

O histórico técnico do repositório pode preservar versões antigas por meio do Git, mas os arquivos atuais da campanha devem representar apenas o cânone vigente.

O Livro definitivo não deve funcionar como changelog de erros.

Evitar:

```text
Corvin entrou pela porta.

[Nota: depois foi corrigido; na verdade entrou pela janela.]
```

Preferir simplesmente corrigir o capítulo para:

```text
Corvin entrou pela janela.
```

> **O Git pode preservar o histórico da edição. A campanha preserva apenas a realidade canônica vigente.**

## Quem pode propor

### MESTRE / NARRADOR

Pode identificar erro, contradição ou problema de continuidade e propor uma correção.

Deve explicar de forma suficiente:

- qual fato está registrado atualmente;
- onde está a inconsistência;
- qual correção propõe;
- quais consequências conhecidas podem ser afetadas.

Não pode aplicar silenciosamente a correção.

### JOGADOR IA e JOGADOR IA EVENTUAL

Podem apontar inconsistências ou sugerir correções quando perceberem conflito com fatos já estabelecidos.

Não podem alterar unilateralmente o cânone.

### OPOSITOR

Pode apontar contradições relevantes para uma resolução ou para a coerência da campanha.

Não pode usar correção como forma de introduzir retroativamente obstáculo, recurso, preparação, capacidade ou vantagem.

### JOGADOR HUMANO

Possui autoridade final sobre toda correção de cânone.

Pode:

```text
APROVAR
→ a correção substitui a versão anterior.

RECUSAR
→ o cânone permanece como estava.

AJUSTAR
→ a proposta é modificada até existir uma versão aceita.
```

## Propagação da correção

Depois de aprovada, a correção deve ser aplicada a todos os registros cuja validade realmente dependa daquele fato.

Pode ser necessário revisar:

```text
LIVRO
STATUS
PROGRESSÃO
FICHA
mestre/
MUNDO
NPCs
outros registros da campanha
```

Não corrigir arquivos por associação superficial. Atualizar apenas aquilo que realmente ficou incorreto ou contraditório.

## Consequências dependentes

Uma correção remove ou altera consequências que dependiam exclusivamente do fato substituído.

Exemplo:

```text
Correção aprovada:
Trigon não matou o guarda.
```

Se existia:

```text
PROGRESSÃO:
- A polícia procura Trigon exclusivamente pelo assassinato do guarda.
```

essa entrada precisa ser removida ou corrigida.

Mas se a polícia também procura Trigon por crimes independentes já estabelecidos, a investigação pode continuar por esses outros fundamentos.

> **A correção invalida o que dependia do fato corrigido. O que possui fundamento independente continua válido.**

## Correção de fala, ação ou agência

Ações de JOGADOR HUMANO, JOGADOR IA e JOGADOR IA EVENTUAL não podem ser alteradas retroativamente por conveniência narrativa.

Se uma ação foi registrada incorretamente no Livro, a correção deve restaurar aquilo que realmente foi declarado e estabelecido durante o jogo.

Uma correção não autoriza o MESTRE / NARRADOR a escolher uma ação diferente para um personagem de jogador.

## Correção e material reservado

Fatos em `mestre/` também obedecem a este protocolo quando já fazem parte do cânone.

O fato de a informação ser reservada não concede ao MESTRE / NARRADOR autoridade para reescrevê-la silenciosamente depois que passou a fundamentar acontecimentos ou resoluções.

Planos e possibilidades ainda não canônicos podem ser alterados livremente porque ainda não são fatos estabelecidos.

Diferença:

```text
FATO CANÔNICO RESERVADO
→ correção exige aprovação do JOGADOR HUMANO.

PLANO
→ pode mudar enquanto ainda não foi executado.

POSSIBILIDADE
→ pode ser descartada ou substituída livremente.
```

A aprovação de uma correção reservada deve ser apresentada sem revelar além do necessário quando houver segredo que ainda precise permanecer protegido durante a campanha.

## Correção não serve para recuperar dificuldade

Não é permitido usar correção de cânone para responder retroativamente a uma solução eficaz dos jogadores.

Exemplo inválido:

```text
JOGADOR:
Encontra uma entrada pelo telhado que contorna os guardas.

MESTRE:
"Correção: sempre existiu uma barreira invisível no telhado."
```

Se a barreira não estava previamente estabelecida como fato ou preparação válida, isso não é correção. É criação retroativa.

O mesmo vale para:

- poderes;
- imunidades;
- recursos;
- guardas;
- armadilhas;
- conhecimento de NPC;
- alianças;
- preparações;
- regras locais;
- qualquer outro elemento criado apenas depois de conhecer a ação do jogador.

> **Correção resolve erro de continuidade. Não corrige o sucesso dos jogadores.**

## Relação com o Livro

Quando uma correção aprovada afeta um capítulo já salvo, corrigir o próprio capítulo afetado.

Não criar automaticamente um novo capítulo para registrar a correção.

O Livro deve continuar apresentando a história como ela canonicamente aconteceu, sem notas administrativas sobre versões descartadas, salvo se a campanha exigir explicitamente outro formato.

## Relação com o fechamento de capítulo

Durante o salvamento, uma inconsistência descoberta não deve ser corrigida silenciosamente.

Se a correção for necessária para consolidar corretamente o capítulo:

```text
1. interromper a correção automática;
2. informar o JOGADOR HUMANO;
3. apresentar a proposta;
4. aguardar aprovação, recusa ou ajuste;
5. somente então consolidar a versão corrigida.
```

Se não for necessário resolver imediatamente, o capítulo não deve receber uma versão inventada apenas para preencher a lacuna.

## Princípio final

> **Toda correção de cânone exige aprovação explícita do JOGADOR HUMANO. Depois de aprovada, a versão corrigida substitui a anterior e todos os registros realmente afetados são alinhados à nova verdade, sem manter versões contraditórias e sem usar correção como criação retroativa.**
