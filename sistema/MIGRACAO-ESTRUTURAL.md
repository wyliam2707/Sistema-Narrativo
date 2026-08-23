# Migração Estrutural do Sistema

Status: EM ANDAMENTO — ARQUITETURA PRINCIPAL ALINHADA

Este arquivo controla a transição da estrutura antiga, concentrada diretamente em `sistema/`, para a arquitetura atual em subpastas.

## Princípio de migração

> **Nenhum arquivo antigo é apagado, movido ou declarado obsoleto apenas porque existe uma pasta nova.**

Arquivos antigos são preservados como fontes históricas. Quando uma regra nova foi explicitamente revisada e aprovada, ela prevalece sobre formulações antigas incompatíveis.

## Status possíveis

- `NOVA ESTRUTURA` — área criada, ainda podendo depender de fontes antigas em pontos não migrados;
- `EM REVISÃO` — área nova possui conteúdo aprovado, mas ainda recebe consolidação;
- `REFERÊNCIA PRINCIPAL` — regra nova é a fonte operacional atual para seu tema;
- `FONTE HISTÓRICA` — arquivo antigo permanece preservado, mas não prevalece contra regra nova aprovada;
- `OBSOLETA` — somente poderá ser usada quando houver autorização explícita para arquivamento ou remoção.

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

`criacao/README.md` substitui `protocolo-de-criacao.md` para novas campanhas.

### `personagem/`
Status: `REFERÊNCIA PRINCIPAL`.

Responsabilidade: definição estável de personagens, calibração, escala, `FIS | RES | MEN | VON`, Perícias, Poderes, TRAÇOS, REL, ficha e NPCs.

A organização interna foi alinhada à estrutura atual de campanha: personagens com agência ficam em `personagens/`; NPCs persistentes ficam em `mestre/`; revisão inicial usa os cinco blocos da criação atual.

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

Responsabilidade: apresentação da ficção, ritmo, ponto de parada, voz, foco e limites de controle narrativo. A pasta já foi alinhada à estrutura atual de campanhas; o padrão antigo de escrita continua fonte de estilo somente nos pontos ainda não substituídos.

### `persistencia/`
Status: `REFERÊNCIA PRINCIPAL`.

Responsabilidade: STATUS, Progressão, atualização de ficha, Livro, fechamento de capítulo, material reservado e correção de cânone.

STATUS e Progressão permanecem conceitos do sistema, mas não criam arquivos obrigatórios próprios na campanha. O presente operacional e os fios causais ativos são persistidos em `estado/atual.md`, salvo quando a natureza do fato exigir ficha, mundo, mestre ou livro.

### `operacao/`
Status: `REFERÊNCIA PRINCIPAL`.

Responsabilidade: ordem das declarações, consulta, julgamento, ponto de parada e registro. `operacao/ciclo-de-cena.md` substitui o ciclo operacional antigo onde houver conflito.

## Porta de entrada atual

`sistema/00-LEIA-PRIMEIRO.md` é o roteador operacional atual.

```text
NOVA CAMPANHA
→ sistema/criacao/README.md

CONTINUAR
→ campanhas/<nome>/README.md
```

Ele aponta para as subpastas vigentes e não deve tratar arquivos históricos como referências principais.

## Mapa das principais fontes antigas

| Arquivo antigo | Área nova principal | Situação atual |
|---|---|---|
| `README.md` | `personagem/` + `resolucao/` | FONTE HISTÓRICA nas regras já migradas |
| `protocolo-de-criacao.md` | `criacao/` | FONTE HISTÓRICA; criação atual em `criacao/README.md` |
| `ciclo-de-jogadores.md` | `operacao/` + `personas/` | FONTE HISTÓRICA; ciclo atual em `operacao/ciclo-de-cena.md` |
| `agencia-de-personagens.md` | `agencia/` | FONTE HISTÓRICA para pontos ainda não reescritos |
| `narracao-e-escrita-padrao.md` | `narracao/` | FONTE HISTÓRICA ainda útil para estilo enquanto não houver substituição completa |
| `modo-rpg.md` | `operacao/` | FONTE HISTÓRICA para procedimentos ainda não migrados |
| `checklist-do-narrador.md` | `operacao/` | FONTE HISTÓRICA para itens ainda não migrados |
| `protocolo-de-fechamento-de-capitulo.md` | `persistencia/` | FONTE HISTÓRICA; referência atual em `persistencia/fechamento-de-capitulo.md` |

## Regras explicitamente substituídas

As seguintes formulações antigas não devem voltar por consulta a arquivos históricos:

- atributos `FOR` e `AGI` separados → `FIS`;
- ficha de cinco atributos → `FIS | RES | MEN | VON`;
- soma automática de atributo, perícia, poder ou equipamento → não existe;
- `Ampliação não paga` e pagamento parcial → pagamento integral;
- custo por antiga escala abstrata de Ampliação → degraus acima da manifestação-base;
- efeitos persistentes por “Consolidação restante” → `D/V5`;
- Proteção `V4` → `V5`;
- Invocação `V12` → `V10`;
- remoção genérica de efeito → Dissipar como efeito próprio de Dano contra STATUS persistente;
- ciclo antigo conflitante → `operacao/ciclo-de-cena.md`;
- novas campanhas em `aventuras/<nome>/` → `campanhas/<nome>/`;
- protocolo antigo de criação → `criacao/README.md`;
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

## Varredura estrutural pós-criação — 2026-08-23

A revisão das pastas após a consolidação do novo processo de criação corrigiu:

- `00-LEIA-PRIMEIRO.md` — deixou de encaminhar a IA para regras históricas como se fossem atuais;
- `personagem/README.md` — passou a usar `campanhas/`, fichas individuais de eventuais e NPCs em `mestre/`;
- `personagem/criacao.md` — alinhado aos cinco blocos, à ordem `JOGADOR IA → EVENTUAL → protagonista`, ao salvamento por bloco e às versões escolhidas pelo jogador;
- `personagem/npcs.md` — persistência alinhada a `mestre/`;
- `persistencia/README.md` — STATUS e Progressão mantidos como conceitos, com armazenamento concreto em `estado/atual.md` e demais fontes conforme função;
- `persistencia/material-reservado.md` — alinhado a `campanhas/<nome>/mestre/`;
- `operacao/README.md` — alinhado ao roteador atual e ao `ciclo-de-cena.md`;
- `narracao/README.md` — terminologia e direção narrativa alinhadas às campanhas atuais.

`personas/`, `agencia/` e `resolucao/` foram revisadas nesta varredura e não exigiram mudança estrutural para as regras novas avaliadas.

## Regra contra duplicação contraditória

Quando conteúdo semelhante existir em dois lugares:

1. verificar se o tema já possui referência nova explicitamente aprovada;
2. se possuir, essa referência prevalece;
3. usar o arquivo antigo apenas para recuperar contexto não contraditório ainda não migrado;
4. nunca manter duas regras incompatíveis como igualmente canônicas;
5. correção explícita mais recente do JOGADOR HUMANO tem prioridade.

## Procedimento de continuação

1. consultar `CONTINUIDADE-REVISAO-ATUAL.md`;
2. consultar este mapa;
3. consultar a pasta atual responsável pelo tema;
4. recorrer a arquivo histórico somente quando o ponto ainda não estiver coberto;
5. não apagar originais sem autorização explícita.

> **A estrutura nova governa onde já foi aprovada. A antiga permanece preservada para história e migração, não para restaurar regras substituídas.**
