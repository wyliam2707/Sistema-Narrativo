# Estado Atual

Status: APROVADO

Este arquivo define a função de:

```text
campanhas/<nome>/estado/atual.md
```

`estado/atual.md` é a **fonte concreta de retomada da campanha**.

Ele responde:

> **Se a campanha continuar agora, o que precisa estar imediatamente verdadeiro e disponível para que a próxima cena comece corretamente?**

## Princípio

`estado/atual.md` não é histórico, não é ficha, não é mundo e não é material reservado completo.

Ele guarda somente o retrato operacional do presente.

```text
LIVRO
→ o que aconteceu

FICHA
→ quem a peça é

MUNDO
→ o que é verdade de forma estável no cenário

MESTRE
→ fatos, NPCs, planos e informações reservadas

ESTADO ATUAL
→ como a campanha precisa ser retomada agora
```

## O que pode entrar

Registrar somente o que ainda é necessário para continuar corretamente, por exemplo:

- momento e local atuais;
- quem está presente ou diretamente envolvido;
- STATUS relevantes;
- Vida atual/máxima quando precisar persistir;
- Mana atual/máxima quando precisar persistir;
- Trama atual da personagem humana quando precisar persistir;
- Status, condições e Efeitos Ativos;
- Barreiras atuais;
- alterações temporárias de Atributo;
- ações ou situações ainda em andamento;
- posição operacional que continue importante;
- compromissos, promessas, dívidas, investigações ou outras consequências causalmente vivas quando forem necessárias à retomada;
- fatos recentes que ainda alteram diretamente as opções disponíveis;
- referência a material reservado necessário para o próximo julgamento, sem copiar seu conteúdo inteiro.

Nem todos esses elementos precisam existir em toda campanha ou cena.

> **Entrar no estado atual exige utilidade para a retomada, não apenas ter acontecido.**

## STATUS dentro do estado atual

`status.md` define o conceito de STATUS.

Na campanha, seus valores persistentes são registrados dentro de `estado/atual.md` quando ainda forem relevantes.

Exemplo:

```text
## Personagens

### Protagonista
Local: corredor norte
Vida: 18/29
Mana: 9/24
Trama: 27
Status: Envenenado
Barreira: 7/15
Efeitos Ativos: Proteção — Cena
```

Isso não cria um arquivo `status.md` dentro da campanha.

`ENERGIA` e `Bateria [1–5]` não são campos universais do motor atual.

## Consequências causalmente vivas

`progressao.md` define o conceito de consequência ainda viva.

Na estrutura atual, essas consequências ficam em `estado/atual.md` quando precisam permanecer disponíveis para a retomada.

Exemplo:

```text
## Fios atuais

- Corvin ainda deve retornar o grimório a Helena.
- A investigação da Guarda continua aberta.
- O credor pode voltar entre 18 e 30 dias para cobrar a dívida.
```

Quando um fio for reservado ou pertencer especificamente ao OPOSITOR, seu detalhe pode ficar em `mestre/` conforme as regras correspondentes.

Não duplicar automaticamente o mesmo conteúdo em todas as fontes.

## O que não entra

Não usar `estado/atual.md` como depósito geral para:

- tudo que aconteceu no capítulo;
- biografia completa de personagens;
- regras do mundo já estáveis;
- fichas inteiras;
- capítulos do Livro;
- segredos que não precisam ser consultados na retomada;
- planos futuros ainda sem efeito sobre o presente;
- ganchos já encerrados;
- consequências que deixaram de ser causalmente vivas.

## Entrada, mudança e saída

O estado atual é sobrescrito pela realidade presente.

```text
ENTRA
→ quando algo passa a ser necessário para continuar corretamente

MUDA
→ quando o fato presente muda

SAI
→ quando deixa de existir ou de ser necessário para a retomada
```

O que sai não é apagado da história: permanece no Livro quando tiver acontecido.

## Relação com material reservado

Informação reservada continua em:

```text
campanhas/<nome>/mestre/
```

Se o NARRADOR precisar saber apenas que existe uma fonte reservada relevante para retomar a situação, `estado/atual.md` pode apontar para ela sem revelar ou duplicar seu conteúdo.

## Relação com fechamento

`SALVAR ESTADO` atualiza `estado/atual.md` sem consolidar novo capítulo.

`SALVAR CAPÍTULO` consolida o Livro e também atualiza `estado/atual.md` para o ponto exato em que a ficção parou.

## Relação com retomada

Ao continuar uma campanha:

```text
campanhas/<nome>/README.md
→ roteia a campanha

estado/atual.md
→ informa o presente necessário para retomar
```

Outras fontes são consultadas somente quando forem necessárias para a próxima decisão, julgamento ou interpretação.

## Regra final

> **`estado/atual.md` é uma fotografia operacional, não um arquivo histórico. Ele guarda somente o que precisa continuar verdadeiro e acessível agora.**
