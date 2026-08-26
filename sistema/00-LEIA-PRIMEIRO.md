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

Esse material não redefine as regras de `sistema/`.

## Fontes atuais

As subpastas atuais de `sistema/` são as únicas fontes canônicas da arquitetura e das regras atuais.

Dentro de resolução mecânica:

```text
sistema/resolucao/motor-de-disputa.md
→ testes e oposições

sistema/resolucao/combate-e-dano.md
→ combate e Dano

sistema/resolucao/vida.md
→ Vida

sistema/resolucao/mana.md
→ Mana

sistema/resolucao/poderes/
→ Hubs e Poderes

sistema/resolucao/status/
→ Status temporários
```

Dentro de personagem:

```text
sistema/personagem/patamar.md
→ Patamar e criação mecânica

sistema/personagem/atributos.md
→ seis Atributos

sistema/personagem/pericias.md
→ Perícias

sistema/personagem/tracos/
→ catálogos de Traços

sistema/personagem/trama.md
→ Trama mecânica do protagonista humano
```

Arquivos removidos durante migrações anteriores não são fontes válidas e não devem ser procurados para restaurar regras antigas.

## Prioridade

Quando houver conflito:

1. correção explícita mais recente do `JOGADOR HUMANO`;
2. regra canônica atual da arquitetura;
3. fonte canônica da própria campanha.

> **As subpastas atuais governam o sistema. Material legado não cria uma segunda fonte de regra.**
