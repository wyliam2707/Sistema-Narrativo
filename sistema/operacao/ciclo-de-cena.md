# Ciclo Operacional de Cena

Status: APROVADO

Este arquivo define **a sequência central das personas durante o jogo**.

As regras de autoridade pertencem a `../personas/`. As fórmulas pertencem a `../resolucao/`. Fora de combate, o fluxo detalhado pertence a `janelas-e-interrupcoes.md`; em combate, a `turnos-de-combate.md` e `ordem-de-resolucao-do-combate.md`.

## Ordem-base fora de combate

Em toda janela significativa fora de combate:

```text
1. JOGADOR HUMANO declara
↓
2. JOGADORES IA aplicáveis declaram
↓
3. JOGADOR IA EVENTUAL declara, quando aplicável
↓
4. OPOSITOR declara movimento, oposição, gancho ou nenhuma intervenção
↓
5. NARRADOR JULGA o conjunto apresentado
↓
6. NARRADOR resolve qualquer incerteza objetiva necessária
↓
7. NARRADOR NARRA A SENTENÇA
↓
8. NARRADOR REGISTRA o que mudou
↓
9. nova janela quando necessária
```

A ordem organiza autoridade. Ela não cria Iniciativa fora de combate e não concede conhecimento que a peça não possua legitimamente.

## Tamanho da janela

Fora de combate, a janela pode representar o intervalo coerente com a situação:

```text
uma ação
uma conversa
uma cena
minutos
uma hora
uma tarde
um dia inteiro
outro período plausível
```

Cada persona aplicável declara sua intenção dentro desse intervalo antes de o NARRADOR fechar a sentença.

O intervalo proposto pode ser interrompido antes do fim quando surgir nova decisão relevante, oposição, informação ou mudança causal.

## Declaração e sentença

Cada persona declara apenas pelas peças sob sua autoridade.

A declaração estabelece **intenção**, não resultado.

O NARRADOR não toma a decisão voluntária por outra persona; ele julga o que efetivamente acontece a partir das declarações, fatos e regras aplicáveis.

No RPG ao vivo, as declarações das personas ativas podem aparecer de forma curta antes da sentença para deixar clara a autoria das decisões. A narração literária continua pertencendo ao NARRADOR.

> **A intenção mostra quem decidiu. A sentença mostra o que aconteceu.**

## Julgamento antes da narração

O NARRADOR:

```text
RECEBE AS INTENÇÕES
→ JULGA
→ RESOLVE INCERTEZA, se houver
→ NARRA
→ REGISTRA
```

Quando o resultado for evidente, estabelece diretamente.

Quando houver impossibilidade evidente, estabelece diretamente.

Quando houver incerteza objetiva de sucesso, usa somente a regra necessária de `../resolucao/` antes de narrar a conclusão.

Quando, depois de considerar fatos e regras, ainda restarem interpretações igualmente coerentes, seguir `../resolucao/principio-de-resolucao.md`.

> **O NARRADOR não narra primeiro e testa depois. A resolução necessária vem antes da sentença conclusiva.**

## Continuidade da janela

Fora de combate, uma intenção pode continuar enquanto ainda cobrir naturalmente o fluxo. Parar quando surgir nova decisão relevante, conforme `janelas-e-interrupcoes.md`.

Em combate, abandonar esta organização ampla e usar a estrutura específica de combate:

```text
Iniciativa fixa
→ Rodada global
→ Turnos pessoais
→ uma vez por posição
→ pausa antes de prosseguir
```

A sentença não deve avançar além de um ponto em que a consequência volta a ser escolha.

## Registro

Depois da sentença, registrar somente o que realmente mudou, conforme `../persistencia/`.

Registrar preserva o resultado; não cria nova consequência.

Depois da sentença, não inventar fato anterior para alterar retroativamente o resultado. Uma nova oportunidade pertence à janela seguinte.

## Regra final

> **Fora de combate, as personas aplicáveis declaram suas intenções para a janela antes do julgamento. A janela pode cobrir desde uma ação até horas ou dias. O NARRADOR julga o conjunto, resolve qualquer dúvida objetiva necessária e só então narra e registra. Em combate, usar exclusivamente a estrutura própria de Iniciativa, Rodada, Turno e vez.**