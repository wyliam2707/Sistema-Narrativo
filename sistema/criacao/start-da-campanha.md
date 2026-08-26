# START da Campanha

Status: APROVADO

Este arquivo define a **trava final que autoriza uma campanha a sair da criação e começar a primeira cena**.

Fichas, estado inicial e cenário podem estar prontos sem que a mesa ainda esteja pronta para jogar. Antes do START, todas as personas exigidas pela campanha devem estar operacionalmente instanciadas e vinculadas.

> **A história não começa com cadeiras vazias.**

## Princípio

`CONTROLE` na ficha identifica qual autoridade decide pela peça, mas isso não substitui a preparação da persona que ocupará essa autoridade durante o jogo.

No START:

```text
personagens aprovados
→ identificar CONTROLE de cada peça inicial
→ instanciar personas necessárias
→ vincular cada persona à sua autoridade
→ conferir escopo de consulta
→ registrar Mesa operacional no README da campanha
→ executar CHECK DE START
→ somente então abrir a primeira cena
```

## Personas obrigatórias

Toda campanha iniciada precisa ter operacionais:

```text
JOGADOR HUMANO
→ vinculado à peça com CONTROLE: JOGADOR HUMANO

JOGADOR IA EVENTUAL
→ persona compartilhada da campanha

OPOSITOR
→ persona da oposição da campanha

NARRADOR
→ persona de julgamento, narração e registro da campanha
```

Além disso, para **cada** personagem cuja ficha possua:

```text
CONTROLE: JOGADOR IA
```

criar uma persona exclusiva:

```text
Personagem A → JOGADOR IA — Personagem A
Personagem B → JOGADOR IA — Personagem B
```

Dois personagens com `CONTROLE: JOGADOR IA` nunca compartilham a mesma persona dedicada.

Personagens com `CONTROLE: JOGADOR IA EVENTUAL` não exigem uma persona dedicada própria; são atendidos pela persona compartilhada conforme `../personas/`.

## Mesa operacional

O `README.md` da campanha registra a composição operacional necessária para retomada.

Formato:

```text
## Mesa operacional

JOGADOR HUMANO → <personagem>
JOGADOR IA — <personagem> → <personagem>
JOGADOR IA — <personagem> → <personagem>
JOGADOR IA EVENTUAL → ATIVO
OPOSITOR → ATIVO
NARRADOR → ATIVO
```

Só listar linhas de `JOGADOR IA — <personagem>` que realmente existirem naquela campanha.

Esse registro não duplica ficha. Ele registra **quem ocupa cada cadeira operacional**.

## Escopo antes do START

Instanciar uma persona não significa entregar a ela todo o material da campanha.

Antes do START, cada persona deve estar ligada ao escopo de consulta correto conforme:

```text
../personas/escopo-de-consulta.md
```

Em especial:

```text
JOGADOR IA
→ recebe somente a visão legítima de sua própria personagem

JOGADOR IA EVENTUAL
→ recebe somente o necessário para a peça que assumir

OPOSITOR
→ recebe oposição e material adversarial legitimamente disponível

NARRADOR
→ recebe o necessário para julgar, narrar e registrar
```

> **Persona criada não significa contexto irrestrito.**

## CHECK DE START

Antes da primeira cena, conferir obrigatoriamente:

```text
[ ] campanha materializada
[ ] direção narrativa e cenário suficientes
[ ] elenco inicial confirmado
[ ] fichas iniciais aprovadas
[ ] pareamento concluído
[ ] estado inicial definido
[ ] JOGADOR HUMANO vinculado
[ ] um JOGADOR IA exclusivo para cada CONTROLE: JOGADOR IA
[ ] JOGADOR IA EVENTUAL instanciado
[ ] OPOSITOR instanciado
[ ] NARRADOR instanciado
[ ] escopos de consulta conferidos
[ ] Mesa operacional registrada
```

Se qualquer item obrigatório estiver pendente:

```text
START BLOQUEADO
→ CRIAÇÃO continua EM ANDAMENTO
→ não abrir primeira cena
```

Se todos estiverem satisfeitos:

```text
CHECK DE START: APROVADO
→ registrar CRIAÇÃO: CONCLUÍDA
→ remover checkpoint de criação
→ registrar Mesa operacional
→ apontar para estado/atual.md
→ START
→ primeira cena
```

## START é transição operacional

`START` não é uma cena, rolagem ou acontecimento ficcional.

Ele é a transição entre:

```text
CRIAR A CAMPANHA
↓
MESA PRONTA
↓
JOGAR A CAMPANHA
```

Depois do START, a criação inicial deixa de conduzir o jogo. `operacao/`, `resolucao/`, `narracao/`, `agencia/` e `persistencia/` assumem suas funções normais.

## Continuação de campanha

Ao continuar uma campanha já iniciada, não recriar personas do zero por hábito.

Usar a `Mesa operacional` registrada para reinstanciar o mesmo arranjo de autoridades e recuperar os escopos corretos antes de retomar a cena.

Se uma mudança de `CONTROLE` tiver sido aprovada desde então, atualizar a Mesa operacional conforme a nova verdade antes de continuar.

## Regra final

> **Nenhuma campanha recebe START enquanto faltar uma persona obrigatória. A primeira cena só pode começar depois que todas as cadeiras necessárias estiverem instanciadas, vinculadas, com escopo correto e registradas na Mesa operacional da campanha.**
