# Janelas e Interrupções

Status: APROVADO

Este arquivo define **até onde uma intenção pode avançar antes de ser necessária uma nova decisão** fora de combate.

Durante combate, usar `turnos-de-combate.md`.

## Regra central

Fora de combate, o jogo funciona por **janelas narrativas**, não por Rodadas, Turnos ou Iniciativa.

Uma janela pode representar o intervalo que fizer sentido para a situação:

```text
uma ação breve
uma conversa
uma cena
alguns minutos
uma hora
uma tarde
um dia inteiro
outro intervalo coerente
```

O tamanho da janela não determina sucesso automático e não obriga a narrar todo o período até o fim.

> **A janela define quanto tempo está sendo proposto. As intenções dizem o que cada peça tenta fazer dentro desse tempo. O NARRADOR decide o que realmente acontece.**

## Declarações antes da sentença

Antes de fechar uma janela significativa, considerar as intenções das personas aplicáveis ao intervalo:

```text
JOGADOR HUMANO
→ declara o que sua peça pretende fazer

JOGADORES IA aplicáveis
→ declaram o que suas próprias peças pretendem fazer

JOGADOR IA EVENTUAL
→ declara quando houver peça sob sua autoridade naquela janela

OPOSITOR
→ declara movimento, oposição, gancho ou nenhuma intervenção

NARRADOR
→ somente depois julga o conjunto apresentado
```

As declarações podem coexistir dentro do mesmo intervalo, desde que sejam compatíveis com tempo, posição, conhecimento, meios e oportunidade.

O NARRADOR não escolhe por uma persona que ainda possui decisão voluntária relevante.

> **Primeiro vêm as intenções aplicáveis. Depois vem o julgamento.**

## Declaração é intenção

O jogador não precisa dizer `tento` antes de toda ação.

```text
“Eu abro a porta.”
→ intenção de abrir a porta.

“Eu convenço ela a ficar.”
→ intenção de convencê-la.
```

A declaração informa o objetivo e o método escolhido. O resultado pertence ao julgamento do NARRADOR.

## Intenção ampla

Uma intenção pode cobrir várias ações coerentes sem exigir nova declaração para cada detalhe.

Exemplo:

```text
“Vou até a cozinha, pego o livro e volto para o quarto.”
```

A intenção continua enquanto:

- nada relevante mudar;
- o método declarado continuar possível;
- nenhuma nova informação exigir escolha;
- nenhuma oposição produzir um novo ponto real de decisão;
- a ação seguinte continuar claramente coberta pela intenção original.

> **Não parar por hábito. Parar quando consequência voltar a ser escolha.**

## Janela longa

Uma declaração pode abranger um período extenso quando isso fizer sentido.

Exemplo:

```text
JOGADOR HUMANO
→ passo o dia pesquisando os registros da mansão.

JOGADOR IA — RAVENA
→ durante esse dia, fica na biblioteca estudando o grimório e evita sair da propriedade.

OPOSITOR
→ nenhuma intervenção durante esse intervalo.
```

O NARRADOR recebe essas intenções antes de fechar o período.

Se nada relevante interromper o intervalo, pode narrar o resultado do dia como uma única sentença.

Se algo importante acontecer às 15h, a sentença para às 15h. O restante do dia ainda não aconteceu.

## Dúvida objetiva antes de narrar

Depois de receber as intenções aplicáveis e antes de narrar a sentença, o NARRADOR verifica cada ponto relevante.

```text
resultado evidente
→ estabelece diretamente

impossibilidade evidente
→ estabelece diretamente

incerteza objetiva de sucesso
→ usa somente a resolução necessária

resultado obtido
→ integra esse resultado à sentença da janela
```

O teste acontece **antes da narração conclusiva**, porque a narração deve descrever o resultado que realmente foi estabelecido.

Exemplo:

```text
JOGADOR HUMANO
→ passo a manhã tentando decifrar o código.

NARRADOR
→ existe dúvida objetiva de sucesso
→ resolve Intelecto + Perícia relevante contra a Dificuldade aplicável
→ obtém o resultado
→ só então narra o que a manhã produziu
```

Não é necessário expor toda a conta mecânica quando ela não for útil para a decisão do JOGADOR HUMANO.

## Reação não é interrupção automática

Outra peça pode falar, reagir ou realizar um detalhe coerente sem necessariamente encerrar a intenção em andamento.

A janela só precisa parar quando a nova situação puder plausivelmente mudar a próxima decisão voluntária de alguma peça controlada por jogador.

Exemplo:

```text
JOGADOR
→ vou até a porta e abro.
```

Se a porta está destrancada:

```text
→ abrir faz parte da intenção.
```

Se a porta está trancada e o personagem possui a chave:

```text
→ usar a chave pode continuar dentro da mesma intenção.
```

Se a porta está trancada e não existe método já escolhido:

```text
→ surgiu nova decisão.
→ parar.
```

## Interrupção acontece no ponto causal

Quando algo relevante interfere no meio de uma intenção ampla, o NARRADOR não conclui artificialmente o restante da sequência.

Exemplo:

```text
JOGADOR
→ entro, atravesso o salão, pego o artefato e saio pela janela.
```

Se uma oposição legítima surge quando ele entra:

```text
→ a sentença para nesse momento.
→ o restante da intenção ainda não aconteceu.
```

> **A ficção é interrompida no momento em que a situação muda, não depois de completar o plano original.**

## Passagem de tempo

Fora de combate, uma declaração pode cobrir minutos, horas ou período maior quando não existir decisão intermediária importante.

Antes de narrar todo o intervalo como concluído, considerar se durante ele:

- outra peça com agência possui ação que intersecta esse período;
- um compromisso ou retorno chega ao momento relevante;
- um gancho do OPOSITOR amadurece;
- uma oposição válida entra em cena;
- surge informação que mudaria a decisão;
- uma condição existente muda de forma relevante.

Se nada disso acontecer, o tempo pode avançar normalmente.

Se algo acontecer no meio, a sentença para no momento causal da mudança.

## Competência evidente

O jogador não precisa lembrar o NARRADOR de cada capacidade óbvia da ficha.

Se algo seria automaticamente perceptível ou executável diante da competência estabelecida, isso entra no julgamento sem pedido especial.

Competência não cria informação inexistente e não concede onisciência.

> **A ficha funciona mesmo quando o jogador não recita seus valores.**

## Resultado evidente

Quando fatos, capacidades e situação tornam o resultado claro, não criar incerteza artificial.

```text
resultado evidente
→ julgar diretamente.

incerteza real
→ usar `../resolucao/`.
```

## Quando abrir nova janela

Abrir nova janela quando ocorrer pelo menos uma das situações abaixo:

- uma peça precisa tomar nova decisão;
- surgiu informação capaz de mudar uma escolha;
- apareceu obstáculo ou oportunidade relevante;
- outra peça tomou iniciativa que exige resposta;
- o OPOSITOR puxou um gancho que entra efetivamente na situação;
- o resultado anterior mudou as opções disponíveis;
- a intenção original deixou de cobrir o próximo passo.

## Relação com combate

Quando a disputa passa a exigir acompanhamento concorrente em intervalos curtos, entra `turnos-de-combate.md`.

Enquanto o combate estiver ativo, usar Iniciativa, Rodadas, Turnos pessoais e vezes conforme as regras próprias de combate.

Quando o combate termina, volta a valer este arquivo.

## Regra final

> **Fora de combate, uma janela pode abranger de uma ação breve a horas ou dias. As personas aplicáveis declaram suas intenções dentro desse intervalo antes de o NARRADOR fechar a sentença. O NARRADOR julga o conjunto, resolve qualquer incerteza objetiva necessária e só então narra o que realmente aconteceu. Se surgir uma nova decisão relevante no meio do intervalo, a sentença para exatamente nesse ponto.**