# Persistência

Esta pasta reúne as regras que respondem à pergunta:

> **O que precisa permanecer verdadeiro depois que a cena, sessão ou capítulo termina?**

## Estado da migração

A estrutura nova está sendo construída sem apagar os arquivos antigos.

Enquanto uma regra ainda não tiver sido reescrita e aprovada nesta pasta, o arquivo antigo correspondente em `sistema/` continua válido.

## Responsabilidades desta área

Esta pasta concentra, progressivamente:

- estado atual e STATUS;
- progressão causal;
- atualização de fichas;
- Livro como registro canônico definitivo;
- salvamento e fechamento de capítulo;
- distinção entre Livro, STATUS, Progressão, ficha e material reservado;
- regras de correção e substituição de cânone.

Conhecimento relevante consolidado não constitui uma camada separada de Persistência. Quando precisar continuar disponível para interpretar um personagem, ele pertence ao campo `Conhecimento atual relevante` da ficha.

O Livro preserva como e quando uma descoberta aconteceu. A Progressão só registra consequências causalmente vivas que tenham surgido dessa descoberta.

## Arquivos aprovados nesta área

- `status.md` — como e onde o personagem está agora;
- `progressao.md` — consequências estabelecidas que continuam causalmente vivas;
- `atualizacao-de-ficha.md` — quando e como uma mudança pode ser consolidada na ficha;
- `livro.md` — registro canônico definitivo da campanha;
- `fechamento-de-capitulo.md` — protocolo atual de salvamento e fechamento de capítulo.

## Arquivos antigos como fonte de migração

- `../protocolo-de-fechamento-de-capitulo.md` — versão antiga do protocolo; substituída nesta arquitetura por `fechamento-de-capitulo.md`.
- Regras antigas de estado, progressão, cronologia e organização ainda existentes em documentos de sistema permanecem como fontes de migração até revisão específica.

A nova arquitetura não exige uma camada separada de Cronologia.

Quando for necessário consultar quando ou em que ordem algo aconteceu, a fonte histórica é o Livro. Um índice ou resumo cronológico pode ser criado como ferramenta opcional em campanhas muito longas, mas não constitui camada obrigatória nem fonte separada de cânone.

## Princípio

Persistência não serve para repetir tudo que aconteceu.

Cada camada guarda uma coisa diferente:

```text
Livro       → o que aconteceu.
Progressão  → o que ainda pode causar consequência futura.
STATUS      → onde e como continuar exatamente agora.
Ficha       → o que mudou de forma estável no personagem e o que precisa permanecer disponível para interpretá-lo.
Mestre      → o que precisa continuar verdadeiro sem ser revelado antes da hora.
```

> **Salvar não é resumir tudo; é preservar corretamente o que continua relevante.**
