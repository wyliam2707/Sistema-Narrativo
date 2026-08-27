# Janelas de Ação

Status: APROVADO

Este arquivo define **quem pode iniciar uma nova ação e quando o NARRADOR recebe autoridade para resolver uma janela**.

A regra existe para impedir dois problemas:

- transformar o JOGADOR HUMANO no gatilho obrigatório de toda cena;
- permitir que o NARRADOR resolva antes que todas as peças com agência tenham declarado sua intenção.

## Princípio central

> **Iniciativa abre a janela. Declarações completam a janela. O NARRADOR somente resolve a janela completa.**

Uma declaração iniciadora **não é uma resolução**.

Nenhuma consequência incerta, oposição, reação voluntária ou resultado pode ser decidido antes de todas as declarações obrigatórias daquela janela terem sido apresentadas.

## Quando uma nova janela abre

Uma nova janela de ação abre:

```text
APÓS O NARRADOR TERMINAR UMA SENTENÇA
→ a situação resultante fica disponível para nova iniciativa.

NO INÍCIO DE UMA CENA
→ depois que a situação inicial foi estabelecida.

QUANDO UMA CONSEQUÊNCIA JÁ RESOLVIDA CRIA NOVA ESCOLHA
→ a sentença termina e uma nova janela começa.
```

O NARRADOR não escolhe uma ação voluntária para abrir a janela. Ele apenas estabelece a situação resultante da sentença anterior.

## Quem pode iniciar

Não existe prioridade fixa pertencente ao protagonista.

A primeira declaração legítima apresentada depois da abertura torna-se a **declaração iniciadora** daquela janela.

Podem iniciar:

```text
JOGADOR HUMANO
→ pela própria peça.

JOGADOR IA
→ pela personagem dedicada que controla.

JOGADOR IA EVENTUAL
→ por uma peça eventual operacionalmente ativa ou NPC ad hoc legitimamente assumido.

OPOSITOR
→ por um movimento, gancho ou peça adversarial legitimamente disponível.
```

O NARRADOR **não inicia ações voluntárias**.

> **Iniciativa narrativa não pertence ao JOGADOR HUMANO. Pertence a qualquer cadeira com autoridade legítima sobre uma peça ou movimento disponível.**

## Iniciativa não concede prioridade de resolução

Iniciar significa somente declarar primeiro.

Exemplo:

```text
JOGADOR IA — Ravena [INICIADORA]
→ decide examinar a passagem antes de sair do quarto.
```

Isso não autoriza o NARRADOR a narrar imediatamente o que ela encontra.

A janela permanece aberta até receber todas as demais declarações obrigatórias.

## Declarações obrigatórias

Antes do julgamento, toda peça operacionalmente ativa cuja decisão intersecte a janela deve declarar.

Isso inclui:

```text
JOGADOR HUMANO
→ declara pela própria peça quando ela estiver envolvida ou puder agir na janela.

CADA JOGADOR IA ATIVO
→ declara ação, intenção ou inação explicitamente.

JOGADOR IA EVENTUAL
→ declara por cada peça eventual/NPC ad hoc que realmente precise decidir.
→ se nenhuma peça eventual precisar decidir, declara isso explicitamente.

OPOSITOR
→ declara o movimento aplicável ou declara explicitamente que não fará movimento adicional.
```

A ausência de ação também é uma declaração válida:

```text
JOGADOR IA — permanece observando e não interfere.

JOGADOR IA EVENTUAL — nenhuma peça eventual precisa de decisão nesta janela.

OPOSITOR — nenhum movimento adicional nesta janela.
```

> **Silêncio operacional não substitui declaração obrigatória.**

## A declaração do iniciador já conta

A peça que abriu a janela não precisa repetir sua intenção.

Sua declaração iniciadora já ocupa sua posição no conjunto de declarações daquela janela.

Exemplo:

```text
JOGADOR HUMANO
→ abre a janela declarando que tenta mover o guarda-roupa.

essa declaração já conta como a declaração do JOGADOR HUMANO
→ faltam as declarações dos demais participantes obrigatórios.
```

## Ordem das declarações

A ordem serve apenas para coleta operacional.

Ela não concede vantagem automática, conhecimento impossível ou direito de reescrever uma intenção depois de conhecer informação privada de outra cadeira.

Cada persona declara usando somente o conhecimento legítimo de sua peça.

Quando uma declaração anterior produz um gesto, fala ou intenção que seria perceptível apenas depois da resolução, as outras peças não podem tratá-la como fato consumado antes do julgamento.

> **Ordem de declaração não é ordem ficcional automática.**

## Quando o JOGADOR HUMANO ainda não declarou

Se uma IA ou o OPOSITOR iniciar a janela e a peça humana precisar decidir, a IA deve apresentar as declarações que lhe pertencem e **parar antes da resolução**.

Exemplo:

```text
JOGADOR IA — Ravena [INICIADORA]
→ propõe atravessar a passagem.

JOGADOR IA — Estelar
→ decide acompanhá-la.

JOGADOR IA EVENTUAL
→ Stancy decide permanecer no quarto.

OPOSITOR
→ nenhum movimento adicional.

JOGADOR HUMANO
→ ainda não declarou.
```

Resultado obrigatório:

```text
NARRADOR
→ NÃO JULGA
→ NÃO RESOLVE
→ NÃO NARRA A CONSEQUÊNCIA
→ aguarda a declaração do JOGADOR HUMANO.
```

Depois que o humano declarar, a janela estará completa e poderá seguir para julgamento.

## Quando o JOGADOR HUMANO inicia

Se o JOGADOR HUMANO abrir a janela, sua declaração já está coletada.

A IA executa então as demais cadeiras obrigatórias:

```text
JOGADOR IA — personagem A
JOGADOR IA — personagem B
JOGADOR IA EVENTUAL
OPOSITOR
```

Somente depois dessas declarações o NARRADOR pode julgar e narrar a sentença.

## Fechamento da janela

A janela somente fica pronta para o NARRADOR quando o conjunto obrigatório estiver completo.

```text
INICIATIVA
→ abre a janela.

TODAS AS DECLARAÇÕES OBRIGATÓRIAS
→ completam a janela.

NARRADOR
→ JULGA.
→ aplica RESOLUÇÃO, se necessária.
→ NARRA A SENTENÇA.
→ REGISTRA, quando aplicável.
```

Se faltar uma declaração obrigatória:

> **não existe resolução ainda.**

## Nova iniciativa depois da sentença

Quando o NARRADOR termina a sentença, a janela anterior está encerrada.

A situação resultante abre imediatamente a possibilidade de uma nova janela.

Qualquer cadeira legítima pode ser a próxima iniciadora.

Isso permite que personagens controlados por IA:

- iniciem conversas sem esperar o protagonista falar;
- proponham planos;
- investiguem por iniciativa própria;
- abandonem ou mudem de atividade;
- puxem assuntos pessoais;
- cumpram compromissos próprios;
- reajam a objetivos que não dependem do personagem humano.

Também permite que o OPOSITOR tome a iniciativa quando um gancho ou plano realmente possuir oportunidade.

A existência dessa possibilidade **não obriga** uma IA ou o OPOSITOR a iniciar toda janela. Se nenhuma cadeira artificial tiver motivo próprio para fazê-lo, a situação pode permanecer aberta para iniciativa do JOGADOR HUMANO.

## Sem encadeamento clandestino

O NARRADOR não pode terminar uma sentença e, dentro da mesma autoridade de NARRADOR, escolher que uma personagem faça voluntariamente a próxima coisa.

Se uma personagem controlada por IA vai iniciar a nova janela, a autoridade deve voltar explicitamente à cadeira correspondente:

```text
NARRADOR
→ termina a sentença.

JOGADOR IA — Ravena [INICIADORA]
→ abre a nova janela com uma decisão própria.
```

Não:

```text
NARRADOR
→ termina a sentença e decide que Ravena vai investigar outra sala.
```

## Regra final

> **Qualquer cadeira com autoridade legítima pode iniciar uma nova janela. A iniciativa apenas abre essa janela. Toda peça operacionalmente ativa que precise decidir deve declarar ação ou inação, e o OPOSITOR deve declarar movimento ou ausência dele. Somente quando todas as declarações obrigatórias estiverem presentes o NARRADOR recebe autoridade para julgar, resolver, narrar a sentença e registrar. Se faltar uma declaração obrigatória, não existe resolução.**
