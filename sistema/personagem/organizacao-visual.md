# Organização Visual das Fichas

Status: APROVADO

Este arquivo define o padrão visual usado pelas fichas de personagem quando renderizadas em Markdown, especialmente no GitHub.

Ele complementa `ficha.md` e `criacao.md` sem alterar o significado dos campos.

> **A ficha deve ser fácil de ler visualmente. Informações diferentes não devem aparecer grudadas em um único bloco de texto.**

## Regra principal

Organizar a ficha por **tópicos claros**, usando títulos Markdown para separar grupos de informação.

Campos curtos pertencentes ao mesmo tópico podem usar lista com rótulos em negrito.

Textos descritivos maiores devem ficar em parágrafo próprio abaixo de seu título.

Evitar uma sequência como:

```text
Status: ... Importância: ... CONTROLE: ... Nome real: ... Idade: ... Aparência: ... Estilo: ...
```

Mesmo que esses campos estejam em linhas diferentes no arquivo-fonte, alguns renderizadores podem apresentá-los como um único parágrafo visual.

## Estrutura visual padrão

```markdown
# Nome

## Metadados
- **Status:** PENDENTE DE REVISÃO
- **Importância:** ...
- **CONTROLE:** ...

## Identidade
- **Nome real:**
- **Idade:**

## Aparência

## Estilo

## Conceito

## Descrição

## Capacidades
- **TRAÇOS:**
- **ATR:** FIS [ ] | RES [ ] | MEN [ ] | VON [ ]
- **PER:**
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

`Aparência` responde principalmente **como a pessoa é fisicamente reconhecida**.

`Estilo` responde principalmente **como ela costuma se apresentar**: roupas, cores, acessórios, uniforme, armadura, maquiagem, símbolos ou outros elementos visuais recorrentes.

`Descrição` pode complementar esses tópicos com presença geral, impressão visual ou outro resumo útil, mas não substitui Aparência e Estilo quando ambos forem relevantes.

## Flexibilidade

A estrutura acima é o padrão, não uma prisão.

Subtópicos adicionais podem ser criados quando melhorarem a consulta. Campos comprovadamente inúteis podem ser removidos somente no momento permitido pelas regras de revisão.

O conteúdo e o momento em que cada campo pode ser preenchido continuam definidos por `ficha.md` e `criacao.md`.

## Compatibilidade com exemplos antigos

Quando um exemplo anterior do sistema mostrar os mesmos campos em linhas simples, interpretar aquilo como **estrutura de dados**, não como obrigação de apresentação visual.

Para a apresentação renderizada da ficha, este padrão por tópicos prevalece.

> **A estrutura informa o que existe. A organização visual determina como isso é apresentado de forma legível.**
