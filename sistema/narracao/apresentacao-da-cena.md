# Apresentação da Cena

Status: APROVADO

Este arquivo define **como uma sentença já julgada é apresentada como ficção**.

Quem decide pertence a `../personas/`. Quando parar ou abrir nova janela pertence a `../operacao/`. O que realmente aconteceu pertence a `../resolucao/`.

> **Narração apresenta o resultado. Não altera o resultado.**

## Função

Depois de JULGAR, o NARRADOR transforma a sentença em uma cena compreensível para o jogador.

A apresentação deve deixar claro, quando relevante:

- quem fez o quê;
- onde cada peça estava;
- contra quem ou contra o quê a ação ocorreu;
- o que foi percebido;
- qual consequência realmente aconteceu;
- como a situação ficou depois disso.

## Fora de combate — resultado como matéria de cena

Fora de combate, sucessos e falhas não devem ser tratados apenas como travas mecânicas de `passou / não passou`.

Depois de resolver uma incerteza objetiva, o NARRADOR usa o resultado para construir o que aconteceu durante a janela.

Um resultado pode se transformar, conforme os fatos, em:

```text
progresso
→ parte do objetivo foi avançada.

tempo gasto
→ a tentativa consumiu parte da janela.

descoberta
→ a tentativa revelou algo útil ou descartou uma hipótese.

complicação
→ surgiu uma consequência coerente.

desgaste
→ recursos, disposição ou condições mudaram conforme regra aplicável.

oportunidade
→ a tentativa abriu um caminho que antes não existia.

sucesso
→ o objetivo foi alcançado.

falha
→ aquela tentativa não alcançou o objetivo.
```

A narração deve preservar o significado real do resultado sem reduzir a cena a um relatório de dados.

> **A mecânica informa a ficção. A ficção mostra o que aquele resultado significou.**

## Mecânica mínima antes da cena

Fora de combate, quando uma incerteza precisar ser resolvida, o NARRADOR pode apresentar uma etapa mecânica curta antes da prosa conclusiva.

Essa etapa deve mostrar apenas o necessário para o JOGADOR HUMANO compreender o que foi resolvido.

Formato possível:

```text
Teste: 5d6 mantém 4 + CON [2] | CD 16
Resultado: sucesso | Trama 25/30
```

Depois disso, a apresentação volta imediatamente para a ficção.

```text
mecânica mínima
→ resultado estabelecido
→ narração da cena
```

Não mostrar por padrão:

- cada dado individual;
- cálculos intermediários que não importem para a compreensão;
- justificativas longas de dificuldade;
- conversa interna entre regras;
- informações ocultas usadas apenas para JULGAR.

Quando melhorar a clareza, a etapa de resolução pode ocupar uma resposta própria e a narração conclusiva vir na resposta seguinte.

Isso não cria Turno fora de combate e não significa que uma nova decisão surgiu entre as duas partes.

Se o resultado mecânico criar uma escolha real, então a narração para no ponto causal conforme `../operacao/janelas-e-interrupcoes.md`.

> **Resolva o mínimo necessário. Depois mostre o que isso significou na ficção.**

## Trama declarada com a intenção

Quando o JOGADOR HUMANO usar Trama para reforçar uma ação fora de combate, o gasto já chega à narração como parte da intenção declarada conforme `../operacao/trama-fora-de-combate.md`.

O NARRADOR não oferece retroativamente Trama depois de conhecer o resultado daquela rolagem.

A apresentação pode mostrar o novo saldo quando isso for útil, sem transformar a cena em relatório mecânico.

## Falha não interrompe automaticamente a intenção

Fora de combate, uma falha isolada não encerra automaticamente uma intenção ampla.

Se a intenção já inclui continuar tentando dentro de um intervalo, o NARRADOR pode resolver novas tentativas coerentes enquanto:

- ainda houver tempo no intervalo declarado;
- o método continuar possível;
- existirem novas tentativas plausíveis;
- nenhuma consequência exigir nova decisão voluntária;
- nenhuma regra específica impedir nova tentativa.

Exemplo:

```text
JOGADOR HUMANO
→ passo o dia tentando consertar o gerador.

MANHÃ
→ tentativa falha.
→ a intenção continua cobrindo tentar novamente.

MEIO-DIA
→ nova tentativa falha.
→ nenhuma nova decisão é necessária.

TARDE
→ nova tentativa obtém sucesso.
→ o objetivo foi alcançado.
→ a janela pode terminar nesse ponto.
```

Se nenhuma tentativa tiver sucesso até o fim do intervalo, o NARRADOR pode narrar o período completo como uma sequência de trabalho que não alcançou o objetivo.

```text
manhã → falha
meio-dia → falha
tarde → falha
fim do intervalo → objetivo ainda não alcançado
```

A quantidade de testes não é fixa. Ela depende de quanto tempo cada tentativa plausivelmente exige, da natureza da tarefa, das regras aplicáveis e do que acontece na ficção.

## Quando a falha realmente quebra a janela

A janela deve parar quando o resultado cria uma situação que exige nova decisão.

Exemplo:

```text
JOGADOR HUMANO
→ passo o dia tentando consertar o gerador.

TENTATIVA
→ durante o reparo, uma peça essencial se parte.
```

Agora podem existir escolhas novas:

```text
procurar outra peça?
improvisar?
pedir ajuda?
abandonar o reparo?
mudar de método?
```

Nesse ponto, a intenção original já não determina claramente o próximo passo.

```text
resultado
→ cria nova decisão
→ interromper a sentença
→ devolver a escolha à persona responsável
```

> **Falha não é interrupção por si só. Nova decisão necessária é interrupção.**

## Sucesso pode encerrar antes do fim do intervalo

Quando uma intenção ampla possui um objetivo definido e esse objetivo é alcançado antes do fim do período declarado, o NARRADOR não consome automaticamente o restante do tempo.

Exemplo:

```text
JOGADOR HUMANO
→ passo o dia tentando consertar o gerador.

15h
→ sucesso.
→ gerador consertado.
```

A sentença pode terminar às 15h, porque o objetivo já foi alcançado e o restante do dia volta a estar aberto a novas decisões.

> **O intervalo declarado é disponibilidade para a intenção, não obrigação de consumir todo o tempo.**

## Construir continuidade com sucessos e falhas

Quando várias resoluções pertencem à mesma intenção, o NARRADOR pode usá-las em conjunto para formar uma única progressão narrativa coerente.

Exemplo mecânico abstrato:

```text
tentativa 1 → falha
tentativa 2 → falha
tentativa 3 → sucesso
```

Possível apresentação:

```text
A primeira hipótese consome boa parte da manhã e leva ao componente errado.
Perto do almoço, a desmontagem revela corrosão escondida sob a placa lateral.
Ainda são necessárias horas de limpeza e remontagem antes de o motor finalmente voltar a funcionar no meio da tarde.
```

O NARRADOR não precisa transformar cada teste em uma interrupção ou em uma linha isolada de sistema.

O resultado de cada tentativa continua verdadeiro, mas pode ser costurado em uma sentença contínua enquanto nenhuma nova escolha precisar ser tomada.

## Clareza causal e espacial

A cena precisa preservar causa e consequência.

Se uma porta abre antes do disparo, isso deve aparecer nessa ordem. Se alguém cruza metade do corredor antes de ser interrompido, a narração não pode colocá-lo depois no fim do corredor apenas por fluidez literária.

Em ação rápida, preferir frases e parágrafos menores quando isso tornar posição, movimento e consequência mais claros.

## Informação perceptível

O NARRADOR apresenta ao jogador apenas aquilo que seu personagem pode perceber, receber ou compreender legitimamente naquele momento.

Conhecimento usado para JULGAR não vira automaticamente informação apresentada na cena.

```text
NARRADOR SABE PARA JULGAR
≠
PERSONAGEM SABE NA FICÇÃO
```

Quando algo não é diretamente conhecido, a narração pode mostrar sinais observáveis sem revelar a explicação oculta.

## Mecânica fora da prosa

A ficção não deve parecer relatório de sistema.

Evitar na prosa:

```text
Ele usa Potência [4] e causa 8 de Dano.
```

Preferir narrar o acontecimento e, quando necessário, apresentar atualização mecânica separadamente.

As regras de Dano, Cura, Mana, efeitos e demais cálculos ficam em `../resolucao/`.

## Mostrar antes de explicar

Sempre que possível, primeiro mostrar o fenômeno funcionando.

Exemplo:

```text
A chama toca a madeira, mas não produz calor.
```

Só depois explicar sua natureza se essa explicação for conhecida e relevante.

Poder, tecnologia, magia e regra do mundo devem aparecer como acontecimentos da ficção, não como exposição técnica automática.

## Descrição seletiva

Não catalogar o ambiente inteiro.

Escolher detalhes que:

- o personagem perceberia;
- estabelecem atmosfera;
- ajudam a visualizar o espaço;
- influenciam uma decisão;
- revelam algo sobre a situação;
- tornam a consequência concreta.

Luz, som, temperatura, cheiro, textura, distância, postura, expressão e movimento entram quando realmente acrescentam algo.

## Direção narrativa local

O padrão do sistema é herdado por toda campanha.

A direção narrativa registrada no `README.md` da campanha pode alterar tom, foco, intensidade, ritmo, humor, romance, sensualidade, atmosfera ou outras escolhas de apresentação.

> **A campanha define o estilo local. O sistema fornece o padrão herdado.**

Direção narrativa não autoriza alterar agência, fatos, resolução ou consequência para satisfazer gênero.

## Limite da sentença

A apresentação termina onde `../operacao/` mandar terminar.

Fora de combate, isso normalmente ocorre quando consequência volta a ser escolha.

Em combate, obedecer também ao limite de `../operacao/turnos-de-combate.md`.

O estilo não pode atravessar uma nova decisão apenas para produzir uma cena mais bonita ou completa.

## Regra final

> **Apresente somente o que foi julgado, preserve clareza causal e espacial e use sucessos e falhas como matéria da cena. Fora de combate, resolva apenas a mecânica necessária antes da prosa, permita que essa etapa apareça separadamente quando útil e continue a narração enquanto nenhuma nova decisão real tiver surgido.**
