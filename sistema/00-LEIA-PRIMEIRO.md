# LEIA PRIMEIRO — Como usar o Sistema Narrativo

Este arquivo é a **porta de entrada operacional** do sistema.

Ele não redefine mecânicas já consolidadas nas subpastas atuais. Sua função é encaminhar cada tarefa para a fonte correta e impedir que arquivos históricos sejam tratados como regra principal por engano.

## Entrada do sistema

Ao iniciar um RPG, perguntar:

> **Nova campanha ou continuar uma campanha existente?**

```text
NOVA CAMPANHA
→ sistema/criacao/README.md

CONTINUAR
→ campanhas/<nome>/README.md
```

Para nova campanha, `sistema/criacao/README.md` é a referência principal do processo.

Para continuar uma campanha do fluxo atual, o `README.md` da própria campanha é a primeira fonte concreta. Ele indica onde consultar personagens, estado, mundo, material reservado e livro e, enquanto a criação estiver em andamento, de onde retomar.

Não pedir ao jogador para repetir informações que os arquivos já fornecem.

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

Responsabilidades:

```text
criacao/      → como uma nova campanha nasce e onde seus dados são salvos
personagem/   → quem a entidade é e do que é capaz
personas/     → quem decide e qual autoridade possui
resolucao/    → o que acontece
agencia/      → continuidade de vontade própria
narracao/     → como mostrar o que aconteceu
persistencia/ → o que precisa permanecer
operacao/     → em que ordem aplicar e consultar as áreas
```

## Ordem operacional de consulta

Não existe obrigação de abrir todos os arquivos do sistema antes de jogar.

Consultar somente o necessário para a função atual.

Para uma sessão em andamento, as referências principais são:

1. `sistema/operacao/ciclo-de-cena.md` — ordem das declarações, movimento do cenário, julgamento e ponto de parada;
2. `sistema/personas/` — autoridade e escopo de consulta de cada persona;
3. `sistema/personagem/` — ficha, atributos, perícias, poderes e definição estável dos personagens;
4. `sistema/resolucao/` — regra específica necessária para descobrir o resultado;
5. `sistema/agencia/` — autonomia e continuidade quando forem relevantes;
6. `sistema/narracao/` — apresentação da ficção;
7. `sistema/persistencia/` — registro do resultado e da continuidade.

Para criar uma campanha nova, começar por:

```text
sistema/criacao/README.md
```

Para continuar uma campanha atual, começar por:

```text
campanhas/<nome>/README.md
```

## Campanhas atuais e material legado

O fluxo atual usa:

```text
campanhas/<nome>/
```

Material antigo em:

```text
aventuras/
```

permanece preservado como legado. Não mover, apagar, reestruturar ou converter automaticamente.

Arquivos antigos diretamente em `sistema/` também permanecem preservados para migração e recuperação de contexto, mas **não prevalecem quando o tema já possui uma referência nova aprovada**.

Isso inclui, entre outros, versões antigas de:

- ciclo de jogadores;
- resolução;
- agência;
- modo RPG;
- criação de campanha;
- fechamento de capítulo;
- regras mecânicas concentradas no antigo `sistema/README.md`.

O mapa de substituição está em `sistema/MIGRACAO-ESTRUTURAL.md`.

## Estrutura das campanhas atuais

Toda campanha criada pelo fluxo atual usa como base:

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

Separação central:

```text
PERSONAGENS → quem são as peças
ESTADO      → como as coisas estão agora
MUNDO       → o que existe
MESTRE      → o que é reservado à condução
LIVRO       → o que aconteceu
```

## Prioridade

Quando houver conflito, seguir nesta ordem:

1. correção explícita mais recente do `JOGADOR HUMANO`;
2. regra nova explicitamente aprovada na arquitetura atual;
3. fonte canônica da própria campanha;
4. arquivo histórico, somente nos pontos ainda não substituídos.

O antigo `sistema/README.md`, `sistema/ciclo-de-jogadores.md`, `sistema/protocolo-de-criacao.md` e outros documentos preservados na raiz de `sistema/` não devem ser usados para restaurar regras que já foram substituídas nas subpastas atuais.

> **Arquivos antigos preservam a história da migração. As subpastas atuais governam o sistema onde suas regras já foram aprovadas.**
