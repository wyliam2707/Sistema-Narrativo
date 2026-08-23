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
Ele usa FIS [4] e causa 8 de Dano.
```

Preferir narrar o acontecimento e, quando necessário, apresentar atualização mecânica separadamente.

As regras de Dano, Cura, Energia, efeitos e demais cálculos ficam em `../resolucao/`.

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

> **Apresente somente o que foi julgado, preserve clareza causal e espacial, mostre o que a peça pode perceber e pare exatamente onde a próxima decisão volta a pertencer à mesa.**