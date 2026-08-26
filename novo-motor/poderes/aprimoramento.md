# Aprimoramento [X]

**Alcance:** Toque → Curto → Médio  
**Conjuração:** Cena → Turno → Instante  
**Alvos:** 1 → 2 → 4  
**Atributo:** +0 → +1 → +2  
**Duração:** Cena → Hora

## Efeito

Aumenta temporariamente um Atributo escolhido do alvo.

É um efeito benéfico e, por padrão, não exige Defesa nem Resistência.

Cada alvo pode manter no máximo **2 efeitos de Aprimoramento** ao mesmo tempo.

## Atributos temporários, Vida e Mana

Aumentos temporários de Atributo afetam normalmente testes e efeitos que utilizam aquele Atributo enquanto estiverem ativos.

Eles **não recalculam Vida Máxima nem Mana Máxima**.

Vida e Mana continuam sendo calculadas apenas a partir dos valores permanentes dos Atributos.

## Sobreposição no mesmo Atributo

Efeitos concorrentes de **Aprimoramento** sobre o mesmo Atributo não se somam entre si.

Quando dois efeitos da mesma fonte ou regra se sobrepõem:

- **mesmo valor:** permanece apenas o efeito de maior duração; o de menor duração é descartado;
- **valores diferentes:** apenas o efeito mais forte fica ativo;
- se o efeito mais fraco possuir duração **menor ou igual** à do efeito mais forte, ele é descartado;
- se o efeito mais fraco possuir duração **maior**, ele permanece inativo enquanto o mais forte estiver ativo e sua duração continua passando normalmente; quando o efeito mais forte terminar, o mais fraco volta a valer se ainda restar duração.

Efeitos mecanicamente parecidos provenientes de **fontes diferentes** podem permanecer ativos ao mesmo tempo, salvo quando alguma regra específica disser o contrário.

Exemplos:

- `+1 por Cena` e `+1 por Hora` da mesma fonte → permanece apenas **+1 por Hora**;
- `+2 por Cena` e `+1 por Hora` da mesma fonte → fica **+2** durante a Cena; depois, se o efeito de uma Hora ainda estiver ativo, passa a valer **+1**;
- `+1 por Cena` e `+2 por Hora` da mesma fonte → o **+1 por Cena** é descartado, pois é mais fraco e também possui duração menor.

## Custos

- **Alcance:** Toque `+0` → Curto `+1` → Médio `+2`
- **Conjuração:** Cena `+0` → Turno `+1` → Instante `+2`
- **Alvos:** 1 `+0` → 2 `+1` → 4 `+2`
- **Atributo:** +0 `+0` → +1 `+1` → +2 `+2`
- **Duração:** Cena `+0` → Hora `+1`

O custo final é a soma dos avanços escolhidos e nunca pode ultrapassar `[X]`.
