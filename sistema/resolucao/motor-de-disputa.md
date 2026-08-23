# Motor geral de disputa

Status: APROVADO

Este arquivo define o motor geral usado quando existe uma disputa real e o resultado pode avançar progressivamente contra uma resistência, uma exigência ou ambas.

Ele não substitui o princípio geral da resolução:

`Resultado evidente → estabelece` | `Impossibilidade evidente → estabelece` | `Incerteza real → resolve`

> **O motor existe para resolver incerteza real, não para transformar toda ação em cálculo.**

## 1. Estrutura geral

A resolução separa:

`Base → capacidade que conduz a ação`

`Suporte → outra capacidade aplicável que melhora a execução`

`Resistência → quanto o mecanismo consegue impedir por aplicação`

`Exigência → quanto precisa ser alcançado`

`Progresso → quanto avança por aplicação`

`Tempo → quanto cada aplicação representa`

`Custo → quanto recurso cada aplicação exige`

A Base pode vir de Atributo, Perícia, Poder, equipamento ou outra capacidade que realmente conduza a ação.

Quando existir uma segunda capacidade realmente aplicável apenas como apoio:

`Ação efetiva = Base + 1 + (Suporte × 0,2)`

Sem Suporte aplicável:

`Ação efetiva = Base + 1`

O progresso produzido por aplicação é:

`Progresso por aplicação = 2^(Ação efetiva − Resistência efetiva)`

A Resistência vem daquilo que realmente responde ao mecanismo usado. Ela pode ser um Atributo, Perícia, proteção, dificuldade técnica, estrutura, trava ou outro valor coerente com a cena.

> **A cena define Base, Suporte e Resistência. A ficha não é somada inteira.**

## 2. Escolha da Base

Usar a leitura definida em `leitura-da-ficha-na-resolucao.md`.

Referência rápida:

```text
algo comum que qualquer pessoa pode tentar
→ Atributo pode ser a Base

tarefa que exige conhecimento ou treinamento
→ Perícia pode ser a Base

Poder, arma ou equipamento com valor próprio
→ esse valor pode ser a Base
```

Se Atributo e Perícia puderem legitimamente conduzir a mesma ação, usar como Base o valor aplicável mais favorável e o outro como Suporte.

Isso não permite que Atributo substitua conhecimento obrigatório nem que Perícia crie capacidade inexistente.

## 3. Resistência depende do mecanismo

A mesma coisa pode possuir resistências diferentes conforme a abordagem.

Uma porta pode, por exemplo, oferecer resistência estrutural baixa contra força bruta e uma Tranca de patamar maior contra arrombamento técnico.

Não existe obrigação de condensar todas as dificuldades de um alvo em uma única Defesa universal.

Quando existir oposição ativa, usar a capacidade que realmente responde ao método empregado. Não somar automaticamente várias resistências.

## 4. Exigência

A Exigência representa quanto progresso precisa ser alcançado para cumprir o objetivo declarado.

Objetivos diferentes podem exigir profundidades diferentes mesmo usando a mesma capacidade.

O personagem não precisa alcançar mais do que sua intenção exige.

> **O objetivo define quanto precisa ser alcançado.**

Alcance, Alvos, Área/Tamanho e Duração pertencem a `consolidacao.md`.

## 5. Progresso

Se uma aplicação não alcança a Exigência e a natureza da ação permite continuidade, o progresso permanece acumulado.

`Aplicações necessárias = teto(Exigência ÷ Progresso por aplicação)`

Quando a própria natureza da ação não permite acúmulo, esta regra não cria acumulação artificial.

Uma Resistência superior não precisa significar falha imediata. Quando a ação puder continuar, ela pode significar mais aplicações, mais tempo, mais custo e mais exposição.

Uma impossibilidade estabelecida pela ficção continua impossível; o motor não cria um mecanismo que não existe.

## 6. Tempo

A unidade de tempo pertence à natureza da tarefa.

Referências usuais:

`10 segundos → aplicação imediata` | `1 minuto → aplicação curta` | `1 hora → aplicação prolongada` | `1 dia → aplicação extensa`

A natureza concreta da atividade pode justificar outra escala, inclusive `Turno` ou `Cena` quando forem as unidades adequadas.

Durante combate, uma aplicação imediata usa o mesmo relógio de `../operacao/turnos-de-combate.md`.

`Tempo efetivo = número de aplicações × tempo por aplicação`

Quando várias aplicações são necessárias, o tempo transcorrido também cria oportunidade normal para reação, interrupção ou mudança da situação quando a ficção permitir.

> **A tarefa define o tempo. A diferença entre ação e resistência define o ritmo do progresso.**

## 7. Custo

Quando a capacidade usada consome Energia, cada aplicação paga normalmente sua configuração.

`Custo = patamar efetivamente usado + Ampliação usada`

Quando existem várias aplicações:

`Custo efetivo = soma da Energia paga em cada aplicação`

As regras de Ampliação pertencem a `consolidacao.md` e as regras de Energia pertencem a `energia.md`.

## 8. Uso do motor

O mesmo motor pode ser aplicado a qualquer disputa progressiva quando Base, Resistência e Exigência forem realmente relevantes.

Regras específicas continuam prevalecendo quando um efeito possuir funcionamento próprio, como Dano em `combate-e-dano.md`.

> **Use o motor somente até o ponto necessário para decidir a cena.**

## Regra final

> **A ficção escolhe o mecanismo. O mecanismo escolhe a Base e a Resistência. O Suporte melhora uma capacidade já aplicável. A Exigência e o tempo mostram quanto custa chegar ao resultado.**
