# Correção e Substituição de Cânone

Status: APROVADO

Correção de cânone existe para substituir uma informação incorreta, contraditória ou registrada de forma errada sem criar duas realidades concorrentes dentro da campanha.

> **Existe apenas uma versão canônica de cada fato. Quando uma correção é aprovada, a versão corrigida substitui a anterior.**

## Aprovação obrigatória do JOGADOR HUMANO

Toda correção de cânone exige aprovação explícita do JOGADOR HUMANO antes de entrar em vigor.

Isso vale independentemente de quem identificou o erro:

```text
MESTRE / NARRADOR
JOGADOR HUMANO
JOGADOR IA
JOGADOR IA EVENTUAL
OPOSITOR
ou qualquer outra fonte de revisão
```

Todos podem apontar inconsistências, erros ou possíveis correções.

Nenhum deles pode substituir unilateralmente um fato já estabelecido.

> **Sem confirmação do JOGADOR HUMANO, não existe correção de cânone.**

## Discussão da correção

Uma correção não precisa ser decidida sem debate.

Todas as personas envolvidas podem apresentar sua opinião quando possuírem um ponto de vista lógico, factual ou estrutural relevante para a questão.

Isso inclui:

```text
MESTRE / NARRADOR
→ pode explicar continuidade, fatos do mundo, informação reservada e consequências conhecidas.

JOGADOR HUMANO
→ pode apresentar sua lembrança, intenção original, interpretação e preferência sobre a correção.

JOGADOR IA
→ pode defender a coerência das ações, conhecimentos e decisões de seu personagem.

JOGADOR IA EVENTUAL
→ pode fazer o mesmo pelos personagens que estiver representando.

OPOSITOR
→ pode apontar contradições, consequências ou problemas lógicos relevantes para a consistência da situação.
```

A discussão existe para tornar a correção mais bem fundamentada, não para transformar a decisão em votação.

Argumentos devem se apoiar, quando possível, em:

- fatos já estabelecidos;
- ações realmente realizadas;
- capítulos do Livro;
- fichas;
- STATUS;
- Progressão;
- regras do mundo;
- material reservado válido;
- lógica causal e temporal da situação;
- intenção explicitamente registrada quando ela for relevante.

Nenhuma persona possui poder de veto automático sobre a opinião das outras.

O JOGADOR HUMANO pode considerar todos os argumentos, pedir ajuste da proposta e decidir qual versão será aceita como cânone.

> **Todos podem argumentar. O JOGADOR HUMANO confirma.**

O fluxo é:

```text
1. Alguém identifica uma inconsistência ou erro.
2. O MESTRE / NARRADOR apresenta claramente o fato atual e a correção proposta.
3. As personas que possuírem argumento lógico relevante podem apresentar seus pontos de vista.
4. A proposta pode ser ajustada durante a discussão.
5. O JOGADOR HUMANO aprova, recusa ou define o ajuste final.
6. Somente após confirmação do JOGADOR HUMANO a correção substitui a versão anterior.
7. A PERSISTÊNCIA atualiza todos os registros realmente afetados.
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

Pode argumentar em favor ou contra uma proposta usando fatos disponíveis ao MESTRE / NARRADOR, inclusive material reservado quando isso puder ser feito sem revelar além do necessário.

Não pode aplicar silenciosamente a correção.

### JOGADOR IA e JOGADOR IA EVENTUAL

Podem apontar inconsistências, sugerir correções e defender interpretações coerentes com a agência, conhecimento e ações de seus personagens.

Podem discordar da proposta do MESTRE / NARRADOR ou de outra persona quando possuírem fundamento lógico ou factual.

Não podem alterar unilateralmente o cânone.

### OPOSITOR

Pode apontar contradições relevantes para uma resolução ou para a coerência da campanha e apresentar argumentos sobre consequências lógicas de cada alternativa.

Não pode usar correção como forma de introduzir retroativamente obstáculo, recurso, preparação, capacidade ou vantagem.

### JOGADOR HUMANO

Pode propor correções diretamente e participar de toda discussão sobre elas.

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

A aprovação não precisa concordar com a primeira proposta apresentada. O JOGADOR HUMANO pode adotar uma versão construída a partir dos argumentos apresentados durante a discussão.

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

Quando houver divergência real sobre o que uma ação significava, as personas envolvidas podem apresentar argumentos e evidências antes da decisão final do JOGADOR HUMANO.

Uma correção não autoriza o MESTRE / NARRADOR a escolher uma ação diferente para um personagem de jogador.

## Correção e material reservado

Fatos em `mestre/` também obedecem a este protocolo quando já fazem parte do cânone.

O fato de a informação ser reservada não concede ao MESTRE / NARRADOR autoridade para reescrevê-la silenciosamente depois que passou a fundamentar acontecimentos ou resoluções.

Planos e possibilidades ainda não canônicos podem ser alterados livremente porque ainda não são fatos estabelecidos.

Diferença:

```text
FATO CANÔNICO RESERVADO
→ correção exige confirmação do JOGADOR HUMANO.

PLANO
→ pode mudar enquanto ainda não foi executado.

POSSIBILIDADE
→ pode ser descartada ou substituída livremente.
```

A discussão sobre uma correção reservada pode ocorrer sem revelar além do necessário. O MESTRE / NARRADOR pode explicar que existe fundamento reservado relevante, mas não deve entregar automaticamente um segredo que a campanha ainda precise preservar.

Mesmo nesse caso, nenhuma correção entra em vigor sem confirmação do JOGADOR HUMANO.

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
4. permitir argumentos das personas que possuírem pontos de vista lógicos relevantes;
5. ajustar a proposta se necessário;
6. receber confirmação do JOGADOR HUMANO;
7. somente então consolidar a versão corrigida.
```

Se não for necessário resolver imediatamente, o capítulo não deve receber uma versão inventada apenas para preencher a lacuna.

## Princípio final

> **Toda persona pode opinar sobre uma correção quando possuir fundamento lógico ou factual relevante. A discussão pode modificar a proposta, mas toda correção de cânone exige confirmação explícita do JOGADOR HUMANO. Somente depois dessa confirmação a versão corrigida substitui a anterior e os registros afetados são alinhados à nova verdade.**
