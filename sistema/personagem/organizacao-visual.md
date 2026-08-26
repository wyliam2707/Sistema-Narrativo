# Organização Visual das Fichas

Status: APROVADO

Este arquivo define o padrão visual usado pelas fichas de personagem quando renderizadas em Markdown, especialmente no GitHub.

Ele complementa `ficha.md` e `criacao.md` sem alterar o significado dos campos.

> **A ficha deve ser fácil de consultar. Informações diferentes não devem aparecer grudadas em um único bloco de texto.**

## Regra principal

Organizar a ficha por tópicos claros, usando títulos Markdown para separar grupos de informação.

Campos curtos pertencentes ao mesmo tópico podem usar lista com rótulos em negrito.

Textos descritivos maiores ficam em parágrafo próprio abaixo de seu título.

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

## Identidade visual

`Aparência` responde principalmente como a pessoa é fisicamente reconhecida.

`Estilo` responde principalmente como ela costuma se apresentar: roupas, cores, acessórios, uniforme, armadura, maquiagem, símbolos ou outros elementos visuais recorrentes.

`Descrição` pode complementar esses tópicos com presença geral, impressão visual ou outro resumo útil.

## Vida e Mana atuais

A ficha consolidada mostra normalmente apenas os valores máximos.

```text
Vida Máxima
Mana Máxima
```

Os valores atuais pertencem ao STATUS e ao HUD operacional quando necessários.

Não duplicar estado momentâneo na ficha apenas para manter a apresentação simétrica.

## Perícias

Perícias são listadas pelo nome, sem graduação antiga.

Exemplo:

```markdown
- **PERÍCIAS:** Medicina, Investigar, Ocultismo
```

Não usar `Medicina [+3]` ou sintaxe equivalente.

## Poderes

Poderes são listados pelo nome do arsenal funcional.

Exemplo:

```markdown
- **PODERES:** Teleporte, Proteção, Ilusão
```

Não usar um grau genérico `[1–5]` no nome do Poder.

Configurações de Hub pertencem às regras e só precisam aparecer na ficha quando houver uma configuração persistente realmente relevante.

## Flexibilidade

A estrutura acima é o padrão, não uma prisão.

Subtópicos adicionais podem ser criados quando melhorarem a consulta. Campos comprovadamente inúteis podem ser removidos somente no momento permitido pelas regras de revisão.

Fichas rápidas e mínimas podem omitir informação desnecessária, conforme `ficha.md` e `npcs.md`.

> **Informação omitida não significa valor zero.**

## Compatibilidade com exemplos antigos

Quando um exemplo legado mostrar:

```text
FIS / RES / MEN / VON
ENERGIA
Perícia [+X]
Poder [1–5]
```

tratar essa apresentação como material antigo que precisa ser migrado para a estrutura atual.

> **A estrutura informa o que existe. A organização visual determina como isso é apresentado de forma legível.**
