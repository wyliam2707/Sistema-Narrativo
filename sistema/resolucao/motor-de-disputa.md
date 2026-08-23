# Motor geral de disputa

Status: APROVADO

Este arquivo define o motor geral usado quando existe uma disputa real e o resultado pode avançar progressivamente contra uma resistência, uma exigência ou ambas.

Ele não substitui o princípio geral da resolução:

`Resultado evidente → estabelece` | `Impossibilidade evidente → estabelece` | `Incerteza real → resolve`

> **O motor existe para resolver incerteza real, não para transformar toda ação em cálculo.**

## 1. Estrutura geral

A resolução separa:

`Potência → quanto consegue produzir`

`Resistência → quanto consegue impedir por aplicação`

`Exigência → quanto precisa ser alcançado`

`Progresso → quanto avança por aplicação`

`Tempo → quanto cada aplicação representa`

`Custo → quanto recurso cada aplicação exige`

Quando houver Perícias realmente aplicáveis dos dois lados:

`Perícia efetiva = Perícia de aplicação − Perícia de oposição`

Quando não houver oposição técnica real, considera-se apenas a Perícia aplicável de quem executa.

O efeito efetivo é:

`Efeito efetivo = Potência usada + 1 + (Perícia efetiva × 0,2)`

O progresso produzido por aplicação é:

`Progresso por aplicação = 2^(Efeito efetivo − Resistência efetiva)`

A Potência pode vir de Poder, Atributo, equipamento ou outra capacidade que realmente produza o efeito.

A Resistência vem daquilo que realmente se opõe ao mecanismo usado.

> **A cena decide quais capacidades entram. Valores não são somados apenas por existirem na ficha.**

## 2. Exigência

A Exigência representa quanto progresso precisa ser alcançado para cumprir o objetivo declarado.

Objetivos diferentes podem exigir profundidades diferentes mesmo usando a mesma capacidade.

O personagem não precisa alcançar mais do que sua intenção exige.

> **O objetivo define quanto precisa ser alcançado.**

Alcance, Alvos, Área/Tamanho e Duração pertencem a `consolidacao.md`.

## 3. Progresso

Se uma aplicação não alcança a Exigência e a natureza da ação permite continuidade, o progresso pode permanecer acumulado.

`Aplicações necessárias = teto(Exigência ÷ Progresso por aplicação)`

Quando a própria natureza da ação não permite acúmulo, esta regra não cria acumulação artificial.

Uma capacidade inferior pode alcançar um objetivo maior quando a ficção permitir continuidade, pagando por isso em tempo, custo e exposição.

## 4. Tempo

A unidade de tempo pertence à natureza da tarefa.

Referências usuais:

`10 segundos → aplicação imediata` | `1 minuto → aplicação curta` | `1 hora → aplicação prolongada` | `1 dia → aplicação extensa`

A natureza concreta da atividade pode justificar outra escala.

Durante combate, uma aplicação imediata usa o mesmo relógio de `../operacao/turnos-de-combate.md`.

`Tempo efetivo = número de aplicações × tempo por aplicação`

Quando várias aplicações são necessárias, o tempo transcorrido também cria oportunidade normal para reação, interrupção ou mudança da situação quando a ficção permitir.

> **A tarefa define o tempo. A disputa define quantas aplicações são necessárias.**

## 5. Custo

Quando a capacidade usada consome Energia, cada aplicação paga normalmente sua configuração.

`Custo = patamar efetivamente usado + Ampliação usada`

Quando existem várias aplicações:

`Custo efetivo = soma da Energia paga em cada aplicação`

As regras de Ampliação pertencem a `consolidacao.md` e as regras de Energia pertencem a `energia.md`.

> **Resistência pode transformar dificuldade em mais tempo, mais custo e mais exposição.**

## 6. Uso do motor

O mesmo motor pode ser aplicado a qualquer disputa quando Potência, Resistência e Exigência forem realmente relevantes.

A natureza da cena determina o que cada uma dessas grandezas representa.

Regras específicas continuam prevalecendo quando um efeito possuir funcionamento próprio.

> **Use o motor somente até o ponto necessário para decidir a cena.**

## Regra final

> **Potência determina quanto consegue produzir. Resistência determina quanto atravessa. Exigência determina quanto precisa ser alcançado. Progresso, Tempo e Custo mostram o preço de chegar lá.**