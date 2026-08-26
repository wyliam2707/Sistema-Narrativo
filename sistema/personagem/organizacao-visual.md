# Organização Visual das Fichas

Status: APROVADO

Este arquivo define **como apresentar uma ficha de personagem de forma legível**, especialmente em Markdown.

Ele complementa `ficha.md`. O procedimento de preenchimento e revisão pertence a `../criacao/personagem.md`.

> **`ficha.md` define o conteúdo; este arquivo define sua organização visual.**

## Estrutura visual padrão

```markdown
# Nome

## Metadados
- **Status:** PENDENTE DE REVISÃO
- **Importância:** ...
- **CONTROLE:** ...
- **Patamar:** [ ]

## Identidade
- **Nome real:**
- **Idade:**

## Aparência

## Estilo

## Conceito

## Descrição

## Capacidades
- **TRAÇOS:**
- **Corpo:** Potência [ ] | Controle [ ] | Resistência [ ]
- **Mente:** Intelecto [ ] | Presença [ ] | Vontade [ ]
- **Vida Máxima:** [ ]
- **Mana Máxima:** [ ]
- **PERÍCIAS:**
- **PODERES:**
- **RECURSOS:**
- **REL:**

## Personalidade e tendências

## Desejos / objetivos atuais

## Medos / limites relevantes

## Conhecimento atual relevante

## História consolidada relevante
```

Campos curtos do mesmo tópico podem compartilhar uma linha ou lista. Textos maiores ficam em seção própria.

## Identidade visual

```text
Aparência → como a pessoa é fisicamente reconhecida
Estilo    → como costuma se apresentar
Conceito  → síntese do que ela é
Descrição → presença e impressão geral útil
```

A ficha não precisa virar catálogo de medidas; precisa permitir reconhecimento e consistência.

## Valores atuais

A ficha consolidada mostra normalmente:

```text
Vida Máxima
Mana Máxima
```

Vida/Mana/Trama atuais, Status, Barreiras e outras condições momentâneas pertencem a `../persistencia/` e ao HUD quando necessário.

Não duplicar estado atual apenas por simetria visual.

## Perícias

Listar pelo nome, sem graduação:

```markdown
- **PERÍCIAS:** Medicina, Investigar, Ocultismo
```

Não usar `Medicina [+3]`.

## Poderes

Listar os Poderes possuídos:

```markdown
- **PODERES:** Teleporte, Proteção, Ilusão
```

Não usar grau genérico `[1–5]`.

Configurações de Hub só entram na ficha quando alguma configuração persistente realmente precisar ser registrada.

## Flexibilidade

O modelo é padrão de leitura, não prisão.

Fichas rápidas ou mínimas podem omitir campos desnecessários conforme `npcs.md`.

> **Informação omitida não significa valor zero.**

O critério para remover campos ou persistir informação pertence a `../persistencia/relevancia-da-ficha.md`.

## Compatibilidade

Exemplos legados com:

```text
FIS / RES / MEN / VON
ENERGIA
Perícia [+X]
Poder [1–5]
```

não definem o formato atual.

## Regra final

> **A organização visual serve à consulta. Ela não cria campos, mecânicas, autoridade nem estado que não estejam definidos nas áreas responsáveis.**
