# Combate e dano

Status: APROVADO

Este arquivo define como uma ação ofensiva é resolvida mecanicamente quando o resultado não é evidente.

A ordem operacional do combate pertence a `../operacao/ordem-de-resolucao-do-combate.md` e `../operacao/turnos-de-combate.md`.

> **Este arquivo não cria Iniciativa, Rodada ou economia universal de ações. Ele apenas resolve ataque, Defesa, Resistência e Dano durante o combate.**

---

## 1. Primeiro: a ficção

Antes de rolar, aplica-se `principio-de-resolucao.md`.

```text
resultado ofensivo evidente
→ estabelecer diretamente

ataque ou efeito impossível
→ estabelecer a impossibilidade

incerteza real
→ resolver somente as etapas necessárias
```

Combate não cria incerteza artificial apenas porque duas peças estão em conflito.

---

## 2. Defesas fixas de combate

Durante combate, a peça atacada não faz uma rolagem defensiva comum. Ela possui quatro valores fixos:

```text
DF = 14 + Controle
RF = 14 + Resistência
DM = 14 + Intelecto
RM = 14 + Vontade
```

Significados:

```text
DF — Defesa Física
→ evita ou impede que um ataque físico alcance plenamente o alvo.

RF — Resistência Física
→ suporta ou resiste a um efeito físico depois que ele alcança o alvo.

DM — Defesa Mental
→ evita ou impede que uma ação mental alcance plenamente o alvo.

RM — Resistência Mental
→ suporta ou resiste a um efeito mental depois que ele alcança o alvo.
```

Esses valores são alvos fixos. Quando uma rolagem ofensiva ou de efeito precisar vencê-los:

> **resultado igual ou maior que o valor fixo = sucesso**

Isso preserva a lógica anterior em que o empate favorecia quem iniciou a ação.

As Defesas fixas são calculadas a partir dos Atributos atuais aplicáveis. Alterações temporárias legítimas nesses Atributos alteram o valor correspondente enquanto permanecerem ativas.

Uma regra específica pode modificar, substituir ou ignorar uma dessas Defesas.

---

## 3. Ataque comum

Uma personagem não precisa possuir um Poder ofensivo para realizar uma agressão comum que seja ficcionalmente capaz de tentar.

Exemplos:

- soco;
- chute;
- empurrão ofensivo;
- golpe corporal;
- ataque mundano coerente com o equipamento disponível.

Quando houver incerteza real, o atacante rola:

> **4 dados mantidos + Atributo coerente com o ataque**

Ataques físicos comuns comparam o resultado à:

> **DF do alvo**

Exemplos de Atributo ofensivo:

```text
golpe de força
→ Potência

golpe de precisão ou técnica
→ Controle
```

Se o resultado do ataque for igual ou maior que a DF, o ataque acerta.

Quando a situação conceder vantagem ficcional óbvia e inegável, aplicar os dados adicionais ou reduzidos conforme `motor-de-disputa.md`.

---

## 4. Dano de ataque comum

Quando um ataque comum causa Dano sem usar um Poder ofensivo ou outra fonte com Dano próprio:

> **Dano = Atributo utilizado no ataque**

Não existe rolagem separada de Dano para essa forma simples de ataque.

Exemplo:

```text
ataque resolvido com Potência [3]
→ Dano 3
```

Se uma arma, equipamento, Traço ou outra capacidade possuir uma regra explícita de Dano, usa-se a regra dessa fonte em vez de inventar uma soma automática.

```text
Atributo do ataque + Dano próprio da arma
≠ soma automática
```

A fonte específica define se usa valor fixo, dados, Atributo adicional ou outra configuração.

---

## 5. Poderes ofensivos

Poderes ofensivos usam suas próprias regras de Acerto, Dano, Defesa, Resistência e Efeito.

A sequência geral é:

> **Defesa → Dano → Resistência → Efeito**

Nem todo Poder utiliza todas as etapas.

Quando o Poder exigir teste de Acerto, o usuário faz a rolagem definida pelo Poder e compara o resultado à Defesa fixa apropriada:

```text
ataque físico
→ normalmente DF

ataque mental
→ normalmente DM
```

Quando o Poder exigir Resistência de Efeito, a resolução compara a rolagem ou resultado aplicável à Resistência fixa apropriada:

```text
efeito físico
→ normalmente RF

efeito mental
→ normalmente RM
```

A natureza real da ação e a regra específica do Poder determinam qual valor se aplica. Não escolher automaticamente o menor valor apenas para favorecer o atacante.

O Dano do Poder vem de seu próprio arquivo e Hub. Não se substitui automaticamente pelo Dano de ataque comum.

---

## 6. Tipos de Defesa de Poder

Quando um Poder indicar um tipo de Defesa, primeiro resolve-se o Acerto contra a Defesa fixa apropriada.

Se o ataque alcançar ou superar a Defesa fixa, a ação venceu a etapa de Defesa e segue normalmente.

Se ficar abaixo da Defesa fixa, aplicar o tipo de Defesa configurado pelo Poder:

### Defesa [Absoluta]

Se a Defesa impedir o ataque:

- não há Dano;
- o Efeito é anulado antes de qualquer Resistência de Efeito.

### Defesa [Total]

Se a Defesa impedir o ataque:

- não há Dano;
- o Efeito ainda pode seguir para sua Resistência, se existir.

### Defesa [Parcial]

Se a Defesa impedir o ataque:

- o alvo sofre metade do Dano;
- arredonde para baixo;
- o Efeito ainda pode seguir para sua Resistência, se existir.

### Defesa [Nula]

Não existe etapa de Defesa.

Isso nunca transforma uma ação ficcionalmente impossível em possível.

---

## 7. Resistência de Efeito

Quando um Efeito permitir Resistência, usar a Resistência fixa coerente com sua natureza:

```text
efeito físico
→ RF

efeito mental
→ RM
```

A regra específica do Poder define qual resultado é comparado à Resistência e o que acontece quando ela é alcançada ou não.

Quando o Efeito for `[Nula]`, não existe etapa de Resistência.

---

## 8. Redução de Dano — RD

Quando uma ou mais Reduções de Dano forem aplicáveis ao mesmo dano:

> **use somente a maior RD aplicável**

Reduções de Dano não se somam.

Exemplo:

```text
RD 2 contra fogo
RD 3 geral
ataque de fogo

→ usar apenas RD 3
```

A RD é aplicada depois de qualquer redução causada pela Defesa.

---

## 9. Escudo / Barreira

Escudos ou Barreiras que possuam reserva própria absorvem Dano conforme a regra que os criou.

O Dano restante atinge essa reserva antes da Vida.

```text
Escudo possui valor suficiente
→ absorve todo o Dano
→ Vida não é reduzida

Dano supera o valor restante do Escudo
→ Escudo chega a 0
→ excedente continua para as etapas seguintes
```

Fontes diferentes só existem e interagem conforme suas regras específicas.

---

## 10. Trama e Dano

Somente a personagem sob `CONTROLE: JOGADOR HUMANO` possui Trama por regra geral.

Depois de Defesa, RD e Escudo determinarem quanto Dano realmente alcançaria a personagem, o jogador pode usar `../personagem/trama.md`:

> **1 Trama = reduz 1 ponto do Dano restante**

Esse gasto acontece depois que o valor é conhecido e antes de reduzir a Vida.

Trama pode reduzir o Dano restante até `0`.

Essa é uma redução própria e posterior ao mínimo final da etapa de Dano; portanto, não se reaplica o mínimo de `1` depois do gasto de Trama.

---

## 11. Ordem de aplicação do Dano

A ordem universal é:

> **Defesa → redução causada pela Defesa → RD → mínimo final → Escudo → Trama, quando aplicável → Vida**

Quando uma regra produzir fração:

> **arredonde para baixo**

Quando um Dano tiver chegado à etapa final de aplicação, ele causa no mínimo:

> **1 ponto de Dano**

Assim, se a maior RD reduzir o valor a `0` ou menos, o Dano final ainda será `1`, desde que o ataque tenha realmente chegado à etapa de Dano.

Esse mínimo não se aplica quando uma etapa anterior anulou completamente o Dano, como uma Defesa que impede o ataque antes da aplicação.

O Escudo ainda pode absorver integralmente esse Dano mínimo.

Depois do Escudo, Trama pode reduzir o Dano restante a `0` conforme sua regra específica.

---

## 12. Exemplo completo

Um Poder causa `9` de Dano.

O ataque fica abaixo da Defesa em uma configuração de Defesa [Parcial], o alvo possui RD `2` e Escudo `1`.

```text
9 ÷ 2
→ 4,5
→ arredonda para 4

4 - RD 2
→ 2

Escudo absorve 1
→ Escudo 0

1 excedente
→ chega à etapa de Trama, se aplicável
→ sem gasto de Trama, Vida perde 1
```

Se essa personagem for o protagonista humano e gastar `1 Trama`, o Dano restante cai para `0` e a Vida não é reduzida.

---

## 13. Vida e incapacidade

O Dano que ultrapassa as proteções e qualquer gasto de Trama reduz a Vida atual.

A Vida Máxima pertence a `vida.md`.

Quando a Vida chega a:

> **0**

A personagem fica:

> **Incapacitada**

0 Vida não significa morte automática.

Uma consequência evidentemente letal continua podendo ser estabelecida pela ficção quando não existir mecanismo real de sobrevivência.

---

## 14. Perícias em combate

Não existe Perícia genérica obrigatória de combate.

Perícias não são somadas ofensiva contra defensiva e não geram `Perícia efetiva`.

Uma Perícia só concede `+1d` durante combate quando seu campo realmente for relevante para aquela resolução específica, conforme `../personagem/pericias.md`.

Exemplos:

```text
Esportes durante uma luta dentro de correnteza
→ pode ser relevante

Condução durante perseguição de veículos
→ pode ser relevante

"Combate" genérico apenas porque existe uma luta
→ não existe como bônus automático
```

---

## 15. Menor número possível de rolagens

Uma ação ofensiva usa o menor número de rolagens necessário.

Como DF, RF, DM e RM são valores fixos, o defensor não faz rolagem apenas para ser atacado ou resistir a uma etapa que possa ser resolvida por esses valores.

Quando um Poder atingir vários alvos e sua regra permitir compartilhar o mesmo Acerto ou Dano:

- fazer uma rolagem de Acerto quando ela puder representar todos os alvos;
- comparar o mesmo resultado às Defesas fixas individuais;
- fazer uma única rolagem de Dano quando o Poder usar Dano rolado compartilhável;
- comparar o resultado de Efeito às Resistências fixas individuais quando aplicável.

Regras específicas de Poder podem estabelecer outra necessidade.

---

## 16. Regras antigas removidas

Não fazem parte do combate:

```text
Perícia efetiva = ofensiva − defensiva
Ataque efetivo = Dano + 1 + (Perícia × 0,2)
Dano = 2^(Ataque − Defesa)
Dano mínimo acumulável 0,25
rolagem defensiva comum contra cada ataque
FIS / RES como estrutura universal antiga
```

Não reutilizar essas fórmulas em novas resoluções.

---

## Fluxo rápido

```text
ficção permite e há incerteza?
→ sim

ataque comum ou Poder?
→ identificar regra aplicável

ataque físico?
→ rolagem ofensiva × DF

ataque mental?
→ rolagem ofensiva × DM

efeito resistível físico?
→ resultado aplicável × RF

efeito resistível mental?
→ resultado aplicável × RM

ataque chegou ao Dano?
→ determinar Dano da fonte
→ aplicar redução da Defesa
→ aplicar maior RD
→ mínimo final 1, se a etapa de Dano foi alcançada
→ Escudo
→ Trama, quando aplicável
→ Vida
→ interpretar consequência
```

## Regra final

> **No combate, DF, RF, DM e RM são valores fixos: DF = 14 + Controle, RF = 14 + Resistência, DM = 14 + Intelecto e RM = 14 + Vontade. Quem age faz a rolagem necessária e compara o resultado à Defesa ou Resistência correspondente. Ataques comuns causam Dano igual ao Atributo usado; Poderes e fontes específicas usam suas próprias regras de Dano e Efeito.**