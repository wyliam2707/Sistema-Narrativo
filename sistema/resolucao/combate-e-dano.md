# Combate e dano

Status: APROVADO

Este arquivo define como uma ação ofensiva é resolvida mecanicamente quando o resultado não é evidente.

A ordem operacional do combate pertence a `ordem-de-resolucao-do-combate.md` e `../operacao/turnos-de-combate.md`.

> **Este arquivo não cria iniciativa, fila fixa ou economia universal de ações. Ele apenas resolve ataque, Defesa e Dano dentro do turno simultâneo.**

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

## 2. Ataque comum

Uma personagem não precisa possuir um Poder ofensivo para realizar uma agressão comum que seja ficcionalmente capaz de tentar.

Exemplos:

- soco;
- chute;
- empurrão ofensivo;
- golpe corporal;
- ataque mundano coerente com o equipamento disponível.

Quando houver oposição ativa, o ataque usa o motor universal:

```text
4 dados mantidos + Atributo do ataque
×
4 dados mantidos + Atributo da defesa
```

Cada lado usa o Atributo coerente com sua própria ação ou reação.

Exemplos possíveis:

```text
golpe de força
→ Potência

golpe de precisão ou técnica
→ Controle

esquiva
→ Controle

suportar ou resistir fisicamente ao mecanismo
→ Resistência
```

Os dois lados não precisam usar o mesmo Atributo.

Em empate, vence quem iniciou a ação. A defesa precisa superar o ataque para impedi-lo.

Quando a situação conceder vantagem ficcional óbvia e inegável a um dos lados, aplica-se `+1d` ao lado favorecido conforme `motor-de-disputa.md`.

---

## 3. Dano de ataque comum

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

## 4. Poderes ofensivos

Poderes ofensivos usam suas próprias regras de Acerto, Dano, Defesa, Resistência e Efeito.

A sequência geral é:

> **Defesa → Dano → Resistência → Efeito**

Nem todo Poder utiliza todas as etapas.

Quando o Poder exigir teste de Acerto, ele usa o motor universal de oposição salvo regra específica.

O Dano do Poder vem de seu próprio arquivo e Hub. Não se substitui automaticamente pelo Dano de ataque comum.

---

## 5. Tipos de Defesa de Poder

Quando um Poder indicar um tipo de Defesa, aplicar exatamente o efeito correspondente.

### Defesa [Absoluta]

Se a Defesa vencer:

- não há Dano;
- o Efeito é anulado antes de qualquer Resistência de Efeito.

### Defesa [Total]

Se a Defesa vencer:

- não há Dano;
- o Efeito ainda pode seguir para sua Resistência, se existir.

### Defesa [Parcial]

Se a Defesa vencer:

- o alvo sofre metade do Dano;
- arredonde para baixo;
- o Efeito ainda pode seguir para sua Resistência, se existir.

### Defesa [Nula]

Não existe etapa de Defesa.

Isso nunca transforma uma ação ficcionalmente impossível em possível.

---

## 6. Redução de Dano — RD

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

## 7. Barreira

Barreiras possuem sua própria reserva de PV conforme a regra que as criou.

O Dano restante atinge a Barreira antes da Vida.

```text
Barreira possui PV suficiente
→ absorve todo o Dano
→ Vida não é reduzida

Dano supera os PV restantes da Barreira
→ Barreira chega a 0
→ excedente passa para Vida
```

Barreiras diferentes só existem e interagem conforme as regras específicas que as criaram.

---

## 8. Ordem de aplicação do Dano

A ordem universal é:

> **Defesa → redução causada pela Defesa → RD → mínimo final → Barreira → Vida**

Quando uma regra produzir fração:

> **arredonde para baixo**

Quando um Dano tiver chegado à etapa final de aplicação, ele causa no mínimo:

> **1 ponto de Dano**

Assim, se a maior RD reduzir o valor a `0` ou menos, o Dano final ainda será `1`, desde que o ataque tenha realmente chegado à etapa de Dano.

Esse mínimo não se aplica quando uma etapa anterior anulou completamente o Dano, como uma Defesa que impede o ataque antes da aplicação.

A Barreira ainda pode absorver integralmente esse Dano mínimo antes que ele alcance a Vida.

---

## 9. Exemplo completo

Um Poder causa `9` de Dano.

O alvo vence uma Defesa [Parcial], possui RD `2` e uma Barreira com `1 PV`.

```text
9 ÷ 2
→ 4,5
→ arredonda para 4

4 - RD 2
→ 2

Barreira absorve 1
→ Barreira 0

1 excedente
→ Vida perde 1
```

---

## 10. Vida e incapacidade

O Dano que ultrapassa as proteções reduz a Vida atual.

A Vida Máxima pertence a `vida.md`.

Quando a Vida chega a:

> **0**

A personagem fica:

> **Incapacitada**

0 Vida não significa morte automática.

Uma consequência evidentemente letal continua podendo ser estabelecida pela ficção quando não existir mecanismo real de sobrevivência.

---

## 11. Perícias em combate

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

## 12. Menor número possível de rolagens

Uma ação ofensiva usa o menor número de rolagens necessário.

Quando um Poder atingir vários alvos e sua regra permitir compartilhar o mesmo Acerto ou Dano:

- fazer uma rolagem de Acerto quando ela puder representar todos os alvos;
- comparar o mesmo resultado às Defesas individuais;
- fazer uma única rolagem de Dano quando o Poder usar Dano rolado compartilhável;
- fazer Resistências individuais apenas quando os resultados realmente precisarem ser diferentes.

Regras específicas de Poder podem estabelecer outra necessidade.

---

## 13. Regras antigas removidas

Não fazem mais parte do combate:

```text
Perícia efetiva = ofensiva − defensiva
Ataque efetivo = Dano + 1 + (Perícia × 0,2)
Dano = 2^(Ataque − Defesa)
Dano mínimo acumulável 0,25
FIS / RES como estrutura antiga universal
```

Não reutilizar essas fórmulas em novas resoluções.

---

## Fluxo rápido

```text
ficção permite e há incerteza?
→ sim

ataque comum ou Poder?
→ identificar regra aplicável

oposição ativa, se houver
→ Acerto × Defesa

ataque chegou ao Dano?
→ determinar Dano da fonte
→ aplicar redução da Defesa
→ aplicar maior RD
→ mínimo final 1, se a etapa de Dano foi alcançada
→ Barreira
→ Vida
→ interpretar consequência
```

## Regra final

> **Combate usa o mesmo motor universal do restante do sistema. Ataques comuns causam Dano igual ao Atributo usado; Poderes e fontes específicas usam seu próprio Dano. Defesa, RD, Barreira e Vida são aplicadas apenas quando realmente pertencem ao mecanismo da ação.**
