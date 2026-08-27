# Estado Atual

Status: REFORMULAÇÃO / NÃO IMPLEMENTADO

Este arquivo define a função de:

```text
campanhas/<nome>/estado/atual.md
```

`estado/atual.md` é a **fotografia operacional do presente**.

Ele responde:

> **Se a campanha continuar agora, o que precisa estar imediatamente disponível para retomar corretamente?**

## O que entra

Registrar somente o que ainda é útil para a continuação imediata, por exemplo:

- data ou momento atual;
- local atual;
- quem está presente;
- posição relevante;
- Vida e Mana atuais quando aplicáveis;
- condições e efeitos ativos;
- recursos temporários importantes;
- intenção persistente ainda em curso;
- ação interrompida;
- processo imediato;
- prazo prestes a interferir;
- fato recente que ainda altera diretamente as opções disponíveis.

Nem todos esses campos precisam existir sempre.

> **Entrar no Estado Atual exige utilidade para a retomada, não apenas ter acontecido.**

## O que não entra

Não usar `estado/atual.md` como depósito de:

- tudo que aconteceu no capítulo;
- biografia completa;
- ficha inteira;
- mundo inteiro;
- todos os conhecimentos da personagem;
- todos os planos do Opositor;
- capítulos do Livro;
- fatos antigos sem efeito atual.

## Exemplo simples

```text
# Estado Atual

Momento: noite, após o jantar
Local: biblioteca da mansão

## Presentes
- Corvin
- Ravena

## Corvin
Vida: 18/24
Mana: 10/16
Condição: Envenenado
Efeito do veneno: próximo dano em 1 hora

## Ravena
Estado: presente na biblioteca

## Situação
Corvin havia declarado que estudaria durante a noite.
O veneno interrompe o avanço da sentença em 1 hora.
```

O exemplo mostra somente o necessário para continuar.

## Entrar, mudar e sair

```text
ENTRA
→ quando algo passa a ser necessário para a retomada.

MUDA
→ quando a realidade presente muda.

SAI
→ quando deixa de existir ou de ser útil para continuar.
```

Se a condição `Envenenado` termina, ela sai do Estado Atual.

O histórico de que a personagem foi envenenada continua no Livro quando relevante.

## Estado não é histórico

```text
LIVRO
→ Corvin foi envenenado durante o jantar.

ESTADO ATUAL
→ Corvin continua Envenenado agora.
```

Depois da cura:

```text
LIVRO
→ continua registrando o acontecimento.

ESTADO ATUAL
→ remove Envenenado.
```

## Processos longos

Nem todo processo fora de cena precisa ser copiado integralmente para o Estado Atual.

Se existir em outra fonte apropriada, o Estado pode guardar somente uma referência quando isso for necessário para a retomada.

Exemplo:

```text
## Processos relevantes
- investigação de Dick continua; consultar registro correspondente se o prazo se tornar relevante.
```

## Planos do Opositor

Detalhes reservados ficam em `campanhas/<nome>/opositor/`.

O Estado Atual não deve revelar nem duplicar o plano inteiro.

Quando necessário, pode registrar apenas que existe um prazo operacional relevante para o Narrador consultar.

## Salvar no meio de uma decisão

Se a campanha for interrompida exatamente antes de uma nova escolha, registrar o ponto sem decidir por ninguém.

Exemplo:

```text
A porta foi aberta.
Ravena está do outro lado.
Nenhuma nova decisão de Corvin foi declarada ainda.
```

Isso é suficiente.

Não completar:

```text
Corvin entra e começa a conversar.
```

se isso ainda não aconteceu.

## Regra final

> **`estado/atual.md` é uma fotografia do presente, não um diário. Guarde somente aquilo que precisa estar imediatamente correto para a próxima janela começar sem reconstruir a campanha inteira.**