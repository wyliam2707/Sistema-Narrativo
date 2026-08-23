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
3. JOGADOR IA EVENTUAL é avaliado e, se ativo, declara pelas peças necessárias
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

## JOGADORES

Cada jogador declara apenas pela própria peça.

A declaração estabelece **intenção**, não resultado.

```text
JOGADOR HUMANO
→ joga seu personagem.

JOGADOR IA
→ cada persona joga somente sua própria personagem.

JOGADOR IA EVENTUAL
→ joga as peças eventuais autorizadas quando elas realmente precisam de decisão.
```

As regras completas de autoridade e contexto estão em `../personas/`.

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

NPCs e recursos adversários podem ser delegados temporariamente a ele conforme `../personas/opositor/` e `../agencia/ganchos-do-opositor.md`.

## NARRADOR

O NARRADOR é juiz.

Sua função é somente:

```text
1. JULGAR
2. NARRAR A SENTENÇA
3. REGISTRAR
```

Consultar fichas, regras, cenário, conhecimento, meios e oportunidade faz parte do julgamento; não constitui uma etapa própria de iniciativa.

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

> **Os jogadores declaram por suas peças. O OPOSITOR apresenta o que quer movimentar. O NARRADOR julga, narra a sentença e registra. Fora de combate, o fluxo segue `janelas-e-interrupcoes.md`; em combate, segue `turnos-de-combate.md`.**