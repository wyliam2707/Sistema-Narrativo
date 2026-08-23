# Ciclo Operacional de Cena

Status: APROVADO

Este arquivo define **a sequência central das personas durante o jogo**.

As regras de autoridade pertencem a `../personas/`. As fórmulas pertencem a `../resolucao/`. Fora de combate, o fluxo detalhado pertence a `janelas-e-interrupcoes.md`; em combate, a `turnos-de-combate.md`.

## Ordem-base

Em toda janela significativa:

```text
1. JOGADOR HUMANO declara
↓
2. JOGADORES IA aplicáveis declaram
↓
3. JOGADOR IA EVENTUAL declara, quando aplicável
↓
4. OPOSITOR declara movimento, oposição, gancho ou nenhuma intervenção
↓
5. NARRADOR JULGA
↓
6. NARRADOR NARRA A SENTENÇA
↓
7. NARRADOR REGISTRA o que mudou
↓
8. nova janela quando necessária
```

A ordem organiza autoridade. Ela não cria iniciativa automática nem concede conhecimento que a peça não possua legitimamente.

## Declaração e sentença

Cada persona declara apenas pelas peças sob sua autoridade.

A declaração estabelece **intenção**, não resultado.

O NARRADOR não toma a decisão voluntária por outra persona; ele julga o que efetivamente acontece a partir das declarações, fatos e regras aplicáveis.

No RPG ao vivo, as declarações das personas ativas aparecem de forma curta antes da sentença para deixar clara a autoria das decisões. A narração literária continua pertencendo ao NARRADOR.

> **A intenção mostra quem decidiu. A sentença mostra o que aconteceu.**

## Julgamento

O NARRADOR:

```text
JULGA
→ NARRA
→ REGISTRA
```

Quando o resultado for evidente, estabelece diretamente.

Quando houver incerteza real, usa somente a regra necessária de `../resolucao/`.

Quando, depois de considerar fatos e regras, ainda restarem interpretações igualmente coerentes, seguir `../resolucao/principio-de-resolucao.md`.

## Continuidade da janela

Fora de combate, uma intenção pode continuar enquanto ainda cobrir naturalmente o fluxo. Parar quando surgir nova decisão relevante, conforme `janelas-e-interrupcoes.md`.

Em combate, usar os turnos simultâneos definidos em `turnos-de-combate.md`.

A sentença não deve avançar além de um ponto em que a consequência volta a ser escolha.

## Registro

Depois da sentença, registrar somente o que realmente mudou, conforme `../persistencia/`.

Registrar preserva o resultado; não cria nova consequência.

Depois da sentença, não inventar fato anterior para alterar retroativamente o resultado. Uma nova oportunidade pertence à janela seguinte.

## Regra final

> **Jogadores declaram. OPOSITOR apresenta oposição. NARRADOR julga, narra e registra. A cena continua enquanto a intenção ainda cobre o fluxo e para quando surge uma nova decisão real.**
