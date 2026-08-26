# Disparo

Poder ofensivo de ataque projetado, com base física.

## Hub

**Disparo [X]**  
**Alcance:** Curto (~20 m) → Médio (~45 m) → Longo (~90 m)  
**Alvos:** 1 → 2 → 4 → 8  
**Área:** Toque → Próximo (~3 m) → Curto (~20 m)  
**Dano:** 1d8 → 2d8 → 3d8 → 4d8 **[+Potência]**  
**Efeito:** Nenhum  
**Defesa:** Total → Parcial  
**Efeito [Nula]**

`[X]` é o máximo de **Mana** que pode ser gasto no uso do Poder.

As distâncias são referências narrativas. Os valores em metros servem como média para interpretar a cena, não como limites rígidos.

## Alvos ou Área

**Alvos** e **Área** são modos alternativos de aplicação e nunca são somados no mesmo uso.

Ao usar Disparo, escolha **Alvos** ou **Área**.

- **Alvos:** permite escolher individualmente até a quantidade selecionada de alvos dentro do Alcance do Poder.
- **Área:** afeta todos que estiverem dentro da Área escolhida, exceto o próprio usuário.

A linha que não for escolhida naquele uso não entra no custo nem na aplicação do Poder.

## Custo

Cada linha é uma progressão própria.

A primeira posição custa `+0 Mana`. Cada avanço posterior custa `+1 Mana`.

- **Alcance:** Curto (~20 m) `+0` → Médio (~45 m) `+1` → Longo (~90 m) `+2`
- **Alvos:** 1 `+0` → 2 `+1` → 4 `+2` → 8 `+3`
- **Área:** Toque `+0` → Próximo (~3 m) `+1` → Curto (~20 m) `+2`
- **Dano:** 1d8 `+0` → 2d8 `+1` → 3d8 `+2` → 4d8 `+3`
- **Defesa:** Total `+0` → Parcial `+1`

O custo final é a soma de todos os avanços escolhidos e nunca pode ultrapassar `[X]`.

Como **Alvos** e **Área** são alternativos, apenas a opção usada é somada ao custo.

Se nenhuma alteração for declarada, Disparo usa as posições iniciais das linhas escolhidas e custa **0 Mana**.

## Uso

Ao declarar Disparo, o JOGADOR HUMANO escolhe apenas os avanços desejados. A operação de combate segue `../../operacao/ordem-de-resolucao-do-combate.md`; não criar confirmação mecânica adicional quando configuração, alvo e custo já estiverem inequívocos.

## Resolução

Disparo não possui Efeito adicional. Portanto, sua resolução usa apenas:

> **Defesa → Dano**

### Acerto e Defesa

Disparo representa um ataque projetado fisicamente: tiro, flecha, projétil, arremesso ou manifestação equivalente.

O Acerto usa:

> `4d6 + Controle`

Como é um ataque físico, o resultado é comparado à:

> **DF do alvo = 14 + Controle do alvo**

```text
Acerto ≥ DF
→ ataque acerta

Acerto < DF
→ a Defesa impede o Acerto pleno conforme a configuração do Hub
```

O alvo não faz rolagem defensiva comum.

Se o Acerto alcançar ou superar a DF, o Dano é aplicado normalmente.

Se ficar abaixo da DF:

- **Defesa [Total]:** o alvo não sofre Dano;
- **Defesa [Parcial]:** o alvo sofre metade do Dano.

### Dano

Role a quantidade de `d8` escolhida no Hub e some **Potência uma única vez ao total dos dados**.

Exemplo:

`3d8 [+Potência]`

Se os dados resultarem em `14` e a Potência for `3`, o Dano final é `17`.

Em **Defesa [Parcial]** que impeça o Acerto pleno, reduza esse Dano final pela metade.

## Efeito

Disparo possui **Efeito: Nenhum** e **Efeito [Nula]**. Não existe etapa de Resistência nem outro Efeito a ser aplicado além do Dano.