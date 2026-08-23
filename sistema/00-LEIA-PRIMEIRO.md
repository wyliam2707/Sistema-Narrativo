# LEIA PRIMEIRO — Como usar o Sistema Narrativo

Este arquivo é a **porta de entrada operacional** do sistema.

Ele não redefine mecânicas. Sua função é encaminhar cada tarefa para a fonte correta.

## Entrada do sistema

Ao iniciar um RPG, perguntar:

> **Nova campanha ou continuar uma campanha existente?**

```text
NOVA CAMPANHA
→ sistema/criacao/README.md

CONTINUAR
→ campanhas/<nome>/README.md
```

Para nova campanha, `sistema/criacao/README.md` é a referência principal.

Para continuar uma campanha atual, o `README.md` da própria campanha é a primeira fonte concreta. Não pedir ao jogador para repetir informações que os arquivos já fornecem.

## Arquitetura atual

```text
sistema/
├── criacao/
├── personagem/
├── personas/
├── resolucao/
├── agencia/
├── narracao/
├── persistencia/
└── operacao/
```

```text
criacao/      → como uma campanha nasce
personagem/   → quem a entidade é e do que é capaz
personas/     → quem decide e qual autoridade possui
resolucao/    → o que acontece
agencia/      → continuidade de vontade própria
narracao/     → como mostrar o que aconteceu
persistencia/ → o que precisa permanecer
operacao/     → em que ordem aplicar e consultar as áreas
```

## Ordem operacional de consulta

Consultar somente o necessário para a função atual.

Para uma sessão em andamento:

1. `sistema/operacao/ciclo-de-cena.md` — ordem das declarações e julgamento;
2. `sistema/personas/` — autoridade de cada persona;
3. `sistema/personagem/` — definição das peças;
4. `sistema/resolucao/` — mecânica necessária;
5. `sistema/agencia/` — continuidade e ganchos quando relevantes;
6. `sistema/narracao/` — apresentação da ficção;
7. `sistema/persistencia/` — registro do resultado e continuidade.

## Estrutura das campanhas atuais

```text
campanhas/<nome-da-campanha>/
├── README.md
├── personagens/
│   └── README.md
├── estado/
│   └── atual.md
├── mundo/
│   └── README.md
├── mestre/
│   └── README.md
└── livro/
    └── README.md
```

```text
PERSONAGENS → quem são as peças
ESTADO      → como as coisas estão agora
MUNDO       → o que existe
MESTRE      → material reservado
LIVRO       → o que aconteceu
```

## Material legado de campanhas

Material antigo em:

```text
aventuras/
```

permanece preservado como legado de campanhas. Não mover, apagar, reestruturar ou converter automaticamente.

A migração dos documentos antigos de `sistema/` foi concluída. O histórico técnico está em:

```text
sistema/MIGRACAO-ESTRUTURAL.md
```

Arquivos antigos já removidos não são fontes válidas e não devem ser procurados para restaurar regras anteriores.

## Prioridade

Quando houver conflito:

1. correção explícita mais recente do `JOGADOR HUMANO`;
2. regra canônica atual da arquitetura;
3. fonte canônica da própria campanha.

> **As subpastas atuais governam o sistema. O histórico de migração registra de onde ele veio, não cria uma segunda fonte de regra.**
