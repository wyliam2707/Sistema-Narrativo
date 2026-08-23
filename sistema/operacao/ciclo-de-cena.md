# Ciclo Operacional de Cena

Status: APROVADO

Este arquivo define **a sequência central das personas durante o jogo**.

Detalhes de fluxo pertencem aos arquivos especializados:

```text
janelas-e-interrupcoes.md
→ intenção ampla, passagem de tempo, interrupção e nova decisão fora de combate.

turnos-de-combate.md
→ turnos simultâneos de até 10 segundos durante combate.
```

As fórmulas e cálculos continuam em `../resolucao/`.

## Imagem mental

> **Os jogadores são a defesa de suas peças. O OPOSITOR é a promotoria. O NARRADOR é o juiz.**

```text
JOGADORES
→ declaram pelas próprias peças.

OPOSITOR
→ apresenta movimento, pressão, gancho, oportunidade ou oposição.

NARRADOR
→ julga.
→ narra a sentença.
→ registra.
```

## Ordem-base

Em toda janela significativa:

```text
1. JOGADOR HUMANO declara
↓
2. JOGADORES IA aplicáveis declaram, cada um por sua peça
↓
3. JOGADOR IA EVENTUAL é avaliado e, se ativo, declara pelas peças eventuais ou NPCs ad hoc necessários
↓
4. OPOSITOR declara movimento, oposição, gancho ou nenhuma intervenção
↓
5. NARRADOR JULGA
↓
6. NARRADOR NARRA A SENTENÇA
↓
7. NARRADOR REGISTRA o que passou a ser verdade
↓
8. nova janela quando necessária
```

A ordem organiza autoridade. Ela não concede conhecimento automático das declarações anteriores a personagens que não as perceberam legitimamente.

### Visibilidade das cadeiras no RPG ao vivo

Durante o RPG ao vivo, as declarações operacionais das personas ativas devem aparecer **explicitamente antes da sentença do NARRADOR**, com identificação da cadeira e da peça quando aplicável.

Exemplo:

```text
[JOGADOR IA — Ravena]
→ continua dormindo; não possui motivo percebido para agir.

[JOGADOR IA — Wanda]
→ permanece deitada; nenhuma nova decisão.

[OPOSITOR]
→ nenhuma intervenção nesta janela.

[NARRADOR]
→ julga e narra a sentença.
```

Se uma cadeira aplicável escolher não agir, isso também deve ser mostrado como declaração de inação. Não esconder a etapa e fazer o NARRADOR parecer autor da decisão da peça.

`JOGADOR IA EVENTUAL` só precisa aparecer quando houver alguma peça eventual ou NPC comum exigindo decisão voluntária naquela janela.

> **No jogo ao vivo, a mesa deve conseguir ver quem declarou e quem apenas julgou.**

## JOGADORES

Cada jogador declara apenas pelas peças sob sua autoridade naquela janela.

A declaração estabelece **intenção**, não resultado.

```text
JOGADOR HUMANO
→ joga seu personagem.

JOGADOR IA
→ cada persona joga somente sua própria personagem.

JOGADOR IA EVENTUAL
→ joga personagens eventuais autorizados e pode assumir NPCs comuns ad hoc quando uma decisão voluntária relevante precisa ser tomada.
```

As regras completas de autoridade estão em `../personas/` e, para NPCs, em `../personas/npcs-e-delegacao.md`.

### NPC comum dentro do ciclo

Nem todo gesto de NPC abre a terceira cadeira.

```text
ROTINA EVIDENTE
→ pode ser narrada como consequência já determinada.

DECISÃO VOLUNTÁRIA RELEVANTE, NÃO ADVERSARIAL
→ JOGADOR IA EVENTUAL assume o NPC naquela janela.

OPOSIÇÃO ATIVA
→ a peça pode ser delegada ao OPOSITOR se o NARRADOR julgar que ela está legitimamente disponível.
```

Assumir um NPC ad hoc não muda seu `CONTROLE` permanente.

## OPOSITOR

O OPOSITOR atua antes do julgamento.

Pode:

- puxar um gancho;
- apresentar oposição;
- avançar plano adversário;
- usar oportunidade;
- movimentar peça ou recurso legitimamente disponibilizado;
- declarar nenhuma intervenção.

O OPOSITOR não determina o resultado.

NPCs e recursos adversários podem ser delegados temporariamente a ele conforme `../personas/npcs-e-delegacao.md` e `../personas/opositor/`.

## NARRADOR

O NARRADOR é juiz.

Sua função é somente:

```text
1. JULGAR
2. NARRAR A SENTENÇA
3. REGISTRAR
```

Consultar fichas, regras, cenário, conhecimento, meios e oportunidade faz parte do julgamento; não constitui uma etapa própria de iniciativa.

O NARRADOR não escolhe decisões voluntárias por NPCs. Quando algo é apenas rotina evidente e já determinada pelos fatos, pode narrar isso como parte da sentença sem criar uma nova decisão.

Quando existir incerteza mecânica real, usar `../resolucao/`.

Quando fatos ou regras já determinarem claramente o resultado, não fabricar dúvida.

## In dubio pro reo

A ordem é:

```text
FATO CLARO
→ aplicar.

REGRA CLARA
→ aplicar.

INCERTEZA QUE EXIGE RESOLUÇÃO
→ usar a mecânica.

DÚVIDA REAL RESTANTE ENTRE INTERPRETAÇÕES IGUALMENTE PLAUSÍVEIS
→ favorecer a defesa.
```

> **In dubio pro reo — na dúvida genuína, favoreça os jogadores.**

## Fora de combate

O fluxo normal segue:

```text
janelas-e-interrupcoes.md
```

Uma intenção pode continuar cobrindo o fluxo enquanto não surgir nova decisão real.

## Em combate

O fluxo passa a seguir:

```text
turnos-de-combate.md
```

Cada turno representa até 10 segundos compartilhados por todas as peças envolvidas.

O turno organiza o tempo; as mecânicas continuam em `../resolucao/`.

## Narração da sentença

O NARRADOR apresenta somente aquilo que o julgamento estabeleceu e aquilo que é legitimamente perceptível.

Fora de combate, a sentença termina quando consequência volta a ser escolha.

Em combate, o limite adicional pertence a `turnos-de-combate.md`.

## Registro

Depois da sentença, registrar somente o que realmente mudou.

```text
estado/atual.md
→ situação operacional presente.

mestre/ganchos-do-opositor.md
→ pontas e oportunidades ainda vivas.

mundo/
→ verdades estáveis quando apropriado.

ficha
→ mudanças estáveis conforme regras de aprovação.

livro/
→ história efetivamente ocorrida quando consolidada.
```

A estrutura concreta segue `../persistencia/`.

Registrar não cria nova consequência.

## Regra contra correção retroativa

Depois da sentença, nenhuma persona inventa fato anterior para alterar o resultado.

Uma nova oportunidade legítima pertence à janela seguinte.

## Regra final

> **Os jogadores declaram por suas peças e essas declarações ficam visíveis no RPG ao vivo. O EVENTUAL cobre também NPCs comuns quando há vontade relevante; o OPOSITOR joga a oposição legitimamente disponível; o NARRADOR julga, narra a sentença e registra. Rotina evidente não exige uma nova cadeira.**
