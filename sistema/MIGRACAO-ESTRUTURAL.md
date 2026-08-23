# Migração Estrutural do Sistema

Status: EM ANDAMENTO — ARQUITETURA PRINCIPAL ALINHADA

Este arquivo controla a transição da estrutura antiga, concentrada diretamente em `sistema/`, para a arquitetura atual em subpastas.

## Princípio de migração

> **Arquivo antigo não é removido apenas porque existe uma pasta nova. Primeiro sua função precisa estar coberta pela arquitetura atual; depois a remoção exige revisão e confirmação explícita.**

Quando uma regra nova foi explicitamente revisada e aprovada, ela prevalece sobre formulações antigas incompatíveis.

## Status possíveis

- `NOVA ESTRUTURA` — área criada, ainda podendo depender de fontes antigas em pontos não migrados;
- `EM REVISÃO` — área nova possui conteúdo aprovado, mas ainda recebe consolidação;
- `REFERÊNCIA PRINCIPAL` — regra nova é a fonte operacional atual para seu tema;
- `FONTE HISTÓRICA` — arquivo antigo ainda existe, mas não prevalece contra regra nova aprovada;
- `REMOVIDO` — arquivo antigo já foi integralmente substituído e removido após confirmação explícita.

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

### `criacao/`
Status: `REFERÊNCIA PRINCIPAL`.

Responsabilidade: criação de novas campanhas, checkpoint, estrutura-base de `campanhas/<nome>/`, destino canônico de cada etapa, criação conceitual, revisão mecânica por blocos e hand-off automático para `estado/atual.md` antes da primeira cena.

### `personagem/`
Status: `REFERÊNCIA PRINCIPAL`.

Responsabilidade: definição estável de personagens, calibração, escala, `FIS | RES | MEN | VON`, Perícias, Poderes, TRAÇOS, REL, ficha e NPCs.

### `personas/`
Status: `REFERÊNCIA PRINCIPAL`.

Responsabilidade: `JOGADOR HUMANO | JOGADOR IA | JOGADOR IA EVENTUAL | OPOSITOR | NARRADOR`, incluindo autoridade e escopo de consulta.

### `resolucao/`
Status: `REFERÊNCIA PRINCIPAL / EM REVISÃO CONTÍNUA`.

Responsabilidade: intenção versus resultado, leitura da ficha, comparação, motor de disputa, combate, Dano, Energia, Cura, efeitos, Consolidação, Dissipar, contenção e social.

### `agencia/`
Status: `NOVA ESTRUTURA`.

Responsabilidade: autonomia, vida fora da câmera, continuidade de vontade própria e separação de conhecimento. Fontes antigas permanecem úteis apenas nos pontos ainda não reescritos.

### `narracao/`
Status: `EM MIGRAÇÃO`.

Responsabilidade: apresentação da ficção, ritmo, ponto de parada, voz, foco e limites de controle narrativo. O padrão antigo de escrita continua fonte de estilo somente nos pontos ainda não substituídos.

### `persistencia/`
Status: `REFERÊNCIA PRINCIPAL`.

Responsabilidade: STATUS, Progressão, atualização de ficha, Livro, fechamento de capítulo, material reservado e correção de cânone.

STATUS e Progressão permanecem conceitos do sistema, mas não criam arquivos obrigatórios próprios na campanha. O presente operacional e os fios causais ativos são persistidos em `estado/atual.md`, salvo quando a natureza do fato exigir ficha, mundo, mestre ou livro.

### `operacao/`
Status: `REFERÊNCIA PRINCIPAL`.

Responsabilidade: ordem das declarações, consulta, julgamento, ponto de parada e registro. `operacao/ciclo-de-cena.md` é a referência atual do ciclo.

## Porta de entrada atual

`sistema/00-LEIA-PRIMEIRO.md` é o roteador operacional atual.

```text
NOVA CAMPANHA
→ sistema/criacao/README.md

CONTINUAR
→ campanhas/<nome>/README.md
```

## Legados removidos após substituição completa

Em 2026-08-23, após revisão e confirmação explícita, foram removidos:

```text
sistema/README.md
sistema/calibracao-independente.md
sistema/modelos.md
sistema/protocolo-de-criacao.md
sistema/organizacao-de-aventura.md
sistema/ciclo-de-jogadores.md
sistema/resolucao-de-acoes.md
sistema/informacao-e-descoberta.md
sistema/progressao-narrativa.md
sistema/protocolo-de-fechamento-de-capitulo.md
```

Substituições principais:

```text
README.md antigo                    → personagem/ + resolucao/
calibracao-independente.md         → personagem/calibracao.md
modelos.md                         → personagem/ficha.md + criacao/ + arquivos específicos
protocolo-de-criacao.md            → criacao/README.md + criacao/estrutura-da-campanha.md
organizacao-de-aventura.md         → criacao/estrutura-da-campanha.md + persistencia/
ciclo-de-jogadores.md              → operacao/ciclo-de-cena.md + personas/
resolucao-de-acoes.md              → resolucao/ + operacao/ciclo-de-cena.md
informacao-e-descoberta.md         → resolucao/informacao-e-investigacao.md
progressao-narrativa.md            → persistencia/progressao.md
protocolo-de-fechamento-de-capitulo.md → persistencia/fechamento-de-capitulo.md
```

Esses caminhos removidos não são mais fontes válidas e não devem ser procurados durante operação normal.

## Fontes históricas ainda existentes

Ainda permanecem porque contêm partes não totalmente migradas ou referência útil:

```text
agencia-de-personagens.md
modo-rpg.md
checklist-do-narrador.md
narracao-e-escrita-padrao.md
exemplo-de-estilo.md
```

Sua utilização é limitada aos pontos ainda não cobertos pela arquitetura atual.

## Regras explicitamente substituídas

As seguintes formulações antigas não devem voltar:

- atributos `FOR` e `AGI` separados → `FIS`;
- ficha de cinco atributos → `FIS | RES | MEN | VON`;
- soma automática de atributo, perícia, poder ou equipamento → não existe;
- `Ampliação não paga` e pagamento parcial → pagamento integral;
- custo por antiga escala abstrata de Ampliação → degraus acima da manifestação-base;
- efeitos persistentes por “Consolidação restante” → `D/V5`;
- Proteção `V4` → `V5`;
- Invocação `V12` → `V10`;
- remoção genérica de efeito → Dissipar como efeito próprio de Dano contra STATUS persistente;
- ciclo antigo → `operacao/ciclo-de-cena.md`;
- novas campanhas em `aventuras/<nome>/` → `campanhas/<nome>/`;
- revisão inicial em quatro blocos → cinco blocos da criação atual;
- NPC persistente em `mundo/npcs/` como padrão → `mestre/`;
- agrupamento de eventuais como uma peça → cada personagem com agência possui ficha própria;
- cânone externo como limite obrigatório → versão escolhida e consolidada pelo jogador é o cânone local da campanha;
- STATUS, Progressão e Cronologia como arquivos obrigatórios separados → presente operacional concentrado em `estado/atual.md`, com distribuição por função quando necessário.

## Estrutura atual de campanha

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
MESTRE      → o que é reservado à condução
LIVRO       → o que aconteceu
```

Fonte principal: `criacao/estrutura-da-campanha.md`.

## Regras mecânicas atuais que não podem ser reintroduzidas de forma antiga

`Custo = patamar efetivamente usado + Ampliação usada`

`Efeito efetivo = Potência usada + 1 + (Perícia efetiva × 0,2)`

`Ataque efetivo = Dano + 1 + (Perícia efetiva × 0,2)`

`Efeito persistente → [D x / V5]`

`Proteção → V5 | Invocação/estrutura equivalente → V10 | Personagem → V35`

`Dissipar → dano contra V de STATUS persistente`

`Contenção por agente → Sustentada pela ação, sem D/V próprio`

`Vários agentes → somam Resultados compatíveis, não Atributos`

## Regra contra duplicação contraditória

Quando conteúdo semelhante existir em dois lugares:

1. verificar se o tema já possui uma referência nova explicitamente aprovada;
2. se possuir, essa referência prevalece;
3. usar arquivo histórico ainda existente apenas para contexto não contraditório e ainda não migrado;
4. nunca manter duas regras incompatíveis como igualmente canônicas;
5. correção explícita mais recente do JOGADOR HUMANO tem prioridade.

## Procedimento de continuação

1. consultar `CONTINUIDADE-REVISAO-ATUAL.md`;
2. consultar este mapa;
3. consultar a pasta atual responsável pelo tema;
4. recorrer a arquivo histórico somente quando ele ainda existir e o ponto ainda não estiver coberto;
5. remover novo legado apenas depois de revisão e confirmação explícita.

> **A estrutura nova governa onde já foi aprovada. Legado só permanece enquanto ainda tiver função real.**
