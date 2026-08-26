# Aflição

Poder modular baseado na família nociva **Aflição**.

## Hub

**Aflição [X]**  
**Alcance:** Curto (~20 m) → Médio (~45 m) → Longo (~90 m)  
**Alvos:** 1 → 2 → 4 → 8  
**Área:** Toque → Próximo (~3 m) → Curto (~20 m)  
**Dano:** Nenhum → 1d6 → 2d6  
**Efeito:** Aflição: 1 de dano → 1d3 de dano → 1d6 de dano por turno  
**Defesa:** Total → Parcial  
**Efeito:** Total → Parcial → Nula  
**Duração:** Turno → Cena → Hora

`[X]` é o máximo de Mana que pode ser gasto no uso do Poder.

## Alvos ou Área

**Alvos** e **Área** são modos alternativos e nunca são somados no mesmo uso.

- **Alvos:** escolhe individualmente até a quantidade selecionada dentro do Alcance.
- **Área:** afeta todos dentro da Área escolhida, exceto o próprio conjurador.

A opção não usada não entra no custo.

## Custo

A primeira posição de cada linha custa `+0 Mana`; cada avanço posterior custa `+1 Mana`.

- **Alcance:** Curto `+0` → Médio `+1` → Longo `+2`
- **Alvos:** 1 `+0` → 2 `+1` → 4 `+2` → 8 `+3`
- **Área:** Toque `+0` → Próximo `+1` → Curto `+2`
- **Dano imediato:** Nenhum `+0` → 1d6 `+1` → 2d6 `+2`
- **Aflição:** 1 de dano `+0` → 1d3 de dano `+1` → 1d6 de dano por turno `+2`
- **Defesa:** Total `+0` → Parcial `+1`
- **Efeito:** Total `+0` → Parcial `+1` → Nula `+2`
- **Duração:** Turno `+0` → Cena `+1` → Hora `+2`

O custo final é a soma dos avanços escolhidos e nunca pode ultrapassar `[X]`.

## Uso e Resolução

O NARRADOR apresenta o Hub configurado, mostra o custo e pede **Confirmar uso por X Mana?** antes da resolução.

A sequência normal é **Defesa → Dano → Resistência → Efeito**.

Acerto e Defesa seguem a regra geral por contexto. O Atributo de Acerto é sempre o que corresponde à forma real da ação e à finalidade declarada. Se a aplicação estiver ambígua, o NARRADOR interpreta a ação; nunca se escolhe automaticamente o maior Atributo.

O **Dano** da linha geral é imediato. O dano de **Aflição** é persistente e ocorre a cada turno enquanto o Efeito permanecer ativo.

- **Efeito [Total]:** Resistência bem-sucedida anula o Efeito.
- **Efeito [Parcial]:** Resistência bem-sucedida reduz a Aflição em uma posição.
- **Efeito [Nula]:** não há Resistência.

## Progressão de Aflição

- **1 de dano:** sofre 1 de dano por turno.
- **1d3 de dano:** sofre 1d3 de dano por turno.
- **1d6 de dano:** sofre 1d6 de dano por turno.

Cada turno corresponde ao intervalo simultâneo de até 10 segundos definido em `../../operacao/turnos-de-combate.md`.