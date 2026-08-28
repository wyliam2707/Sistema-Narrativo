# Campanhas

Esta pasta é a raiz de **todos os dados vivos das campanhas** do Sistema Narrativo.

As regras ficam em `regras-basicas/`.

Tudo que for verdade específica de uma campanha deve ser salvo dentro de sua própria pasta em `campanhas/<nome>/`.

```text
regras-basicas/
→ regras, procedimentos e modelos

campanhas/<nome>/
→ estado real da mesa
```

## O que pertence à campanha

Podem e devem ser preservados aqui, conforme a estrutura de cada campanha:

- fichas reais;
- personagens;
- estado atual;
- Vida, Mente, Mana, condições e recursos;
- conhecimento das personagens;
- relações;
- mundo e cenário;
- acontecimentos estabelecidos;
- processos em andamento;
- prazos;
- eventos futuros já julgados;
- planos e registros do Opositor;
- registros do Narrador;
- capítulos e Livro;
- qualquer outra verdade que precise continuar existindo naquela campanha.

> **Se é uma verdade da mesa e não uma regra do sistema, pertence a `campanhas/<nome>/`.**

## Estrutura

Cada campanha deve existir em sua própria subpasta:

```text
campanhas/
├── README.md
├── <nome-da-campanha>/
└── <outra-campanha>/
```

A estrutura interna pode conter áreas como:

```text
campanhas/<nome>/
├── README.md
├── estado/
├── personagens/
├── mundo/
├── mestre/
├── opositor/
└── livro/
```

Nem toda campanha precisa usar exatamente todas essas pastas.

## Como localizar campanhas disponíveis

Não manter neste arquivo uma lista manual de campanhas ou de seus estados, porque ela pode envelhecer.

Quando o jogador escolher **continuar uma campanha existente**:

```text
1. listar as subpastas atuais de campanhas/.
2. abrir campanhas/<nome>/README.md de cada candidata.
3. usar o estado declarado no README da própria campanha.
4. apresentar ao jogador somente opções realmente disponíveis.
```

O README de cada campanha é a fonte principal para dizer se ela está:

```text
CRIAÇÃO: EM ANDAMENTO
→ pode retomar a criação pelo checkpoint apropriado.

CRIAÇÃO: CONCLUÍDA
→ pode continuar conforme regras-basicas/INICIO-E-RETOMADA.md.

TESTE / LEGADO / INCOMPATÍVEL
→ não oferecer como campanha jogável por padrão.
→ migrar ou examinar somente se o jogador pedir.
```

Se existir apenas uma campanha válida, ainda assim confirmar com o jogador que deseja continuar aquela campanha antes de abrir a ficção.

## Fonte da verdade

Não inferir o estado da campanha pelo nome da pasta, pela memória da conversa ou por uma lista antiga.

```text
campanhas/<nome>/README.md
→ estado geral e roteamento da campanha.

campanhas/<nome>/estado/atual.md
→ ponto operacional de retomada.

campanhas/<nome>/personagens/
→ fichas relevantes.

campanhas/<nome>/mestre/narrativa.md
→ identidade persistente.

campanhas/<nome>/mestre/roteiro.md
→ temporada ativa, quando existir.
```

Depois da escolha da campanha, seguir `regras-basicas/INICIO-E-RETOMADA.md` e consultar somente o que for necessário para reconstruir a mesa.

## Regra final

> **`regras-basicas/` explica como jogar. `campanhas/<nome>/` guarda o que existe e aconteceu. Para continuar, descobrir as campanhas pela estrutura atual e confiar no README de cada campanha, não em listas manuais.**
