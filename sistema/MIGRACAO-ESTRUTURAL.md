# Migração Estrutural do Sistema

Status: EM ANDAMENTO

Este arquivo controla a transição da estrutura antiga, concentrada diretamente em `sistema/`, para a arquitetura atual em subpastas.

## Princípio de migração

> **Nenhum arquivo antigo é apagado, movido ou declarado obsoleto apenas porque existe uma pasta nova.**

Arquivos antigos são preservados como fontes históricas até que deixem de ser úteis. Quando uma regra nova foi explicitamente revisada e aprovada, ela prevalece sobre formulações antigas incompatíveis.

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

Responsabilidade: criação de novas campanhas, checkpoint de criação, estrutura-base de `campanhas/<nome>/`, destino canônico de cada etapa, criação conceitual, revisão mecânica por blocos e hand-off automático para `estado/atual.md` antes da primeira cena.

`criacao/README.md` substitui `protocolo-de-criacao.md` como referência para novas campanhas.

### `personagem/`
Status: `REFERÊNCIA PRINCIPAL / EM ALINHAMENTO ESTRUTURAL`.

Responsabilidade: definição estável de personagens, calibração, escala, `FIS | RES | MEN | VON`, Perícias, Poderes, TRAÇOS, REL, ficha e NPCs.

As regras mecânicas permanecem atuais. Referências internas à organização antiga de campanhas devem ser alinhadas a `criacao/estrutura-da-campanha.md`.

### `personas/`
Status: `REFERÊNCIA PRINCIPAL` para papéis e autoridade operacional.

Responsabilidade: `JOGADOR HUMANO | JOGADOR IA | JOGADOR IA EVENTUAL | OPOSITOR | NARRADOR`, incluindo escopo de consulta.

### `resolucao/`
Status: `REFERÊNCIA PRINCIPAL / EM REVISÃO CONTÍNUA`.

Responsabilidade: intenção versus resultado, leitura da ficha, comparação, motor de disputa, combate, Dano, Energia, Cura, efeitos, Consolidação, Dissipar, contenção e social.

As formulações novas de resolução prevalecem sobre fórmulas incompatíveis dos arquivos antigos.

### `agencia/`
Status: `NOVA ESTRUTURA`.

Responsabilidade: autonomia, vida fora da câmera, continuidade de vontade própria e separação de conhecimento. O documento antigo de agência permanece fonte histórica nos pontos ainda não reescritos.

### `narracao/`
Status: `NOVA ESTRUTURA`.

Responsabilidade: apresentação da ficção, ritmo, ponto de parada, voz, foco e limites de controle narrativo. O padrão antigo de narração continua fonte nos pontos de estilo ainda não migrados.

### `persistencia/`
Status: `REFERÊNCIA PRINCIPAL / EM ALINHAMENTO ESTRUTURAL`.

Responsabilidade: STATUS, Progressão, atualização de ficha, Livro, fechamento de capítulo, material reservado e correção de cânone.

STATUS e Progressão continuam conceitos válidos do sistema. Sua **persistência concreta nas campanhas atuais** deve respeitar a estrutura aprovada: estado operacional e fios causais ativos pertencem a `campanhas/<nome>/estado/atual.md`, salvo quando a natureza do fato exigir ficha, mundo, mestre ou livro.

### `operacao/`
Status: `REFERÊNCIA PRINCIPAL` para o ciclo de cena.

Responsabilidade: ordem das declarações, consulta, julgamento, ponto de parada e registro. `operacao/ciclo-de-cena.md` substitui o ciclo operacional antigo onde houver conflito.

## Porta de entrada atual

`sistema/00-LEIA-PRIMEIRO.md` é o roteador operacional atual.

Ele deve apontar para as subpastas vigentes e **não** para arquivos históricos como se fossem referências principais.

Fluxo:

```text
NOVA CAMPANHA
→ sistema/criacao/README.md

CONTINUAR
→ campanhas/<nome>/README.md
```

## Mapa das principais fontes antigas

| Arquivo antigo | Área nova principal | Situação atual |
|---|---|---|
| `README.md` | `personagem/` + `resolucao/` | FONTE HISTÓRICA nas regras já migradas |
| `protocolo-de-criacao.md` | `criacao/` | FONTE HISTÓRICA; criação atual em `criacao/README.md` |
| `ciclo-de-jogadores.md` | `operacao/` + `personas/` | FONTE HISTÓRICA; ciclo atual em `operacao/ciclo-de-cena.md` |
| `agencia-de-personagens.md` | `agencia/` | FONTE HISTÓRICA para pontos ainda não reescritos |
| `narracao-e-escrita-padrao.md` | `narracao/` | FONTE HISTÓRICA ainda útil para estilo enquanto não houver substituição aprovada |
| `modo-rpg.md` | `operacao/` | FONTE HISTÓRICA para procedimentos ainda não migrados |
| `checklist-do-narrador.md` | `operacao/` | FONTE HISTÓRICA para itens ainda não migrados |
| `protocolo-de-fechamento-de-capitulo.md` | `persistencia/` | FONTE HISTÓRICA; referência atual em `persistencia/fechamento-de-capitulo.md` |

## Regras explicitamente substituídas

As seguintes formulações antigas não devem voltar por consulta a arquivos históricos:

- atributos `FOR` e `AGI` separados → substituídos por `FIS`;
- ficha de cinco atributos → substituída por `FIS | RES | MEN | VON`;
- soma automática de atributo, perícia, poder ou equipamento → não existe;
- `Ampliação não paga` e pagamento parcial → substituídos por pagamento integral;
- custo por antiga escala abstrata de Ampliação → substituído por degraus acima da manifestação-base;
- efeitos persistentes tratados por “Consolidação restante” → substituídos por `D/V5`;
- Proteção `V4` → substituída por `V5`;
- Invocação `V12` ou referências anteriores → substituída por `V10`;
- remoção genérica de efeito → Dissipar é efeito próprio de Dano contra STATUS persistente;
- ciclo antigo quando conflitante → substituído por `operacao/ciclo-de-cena.md`;
- criação em `aventuras/<nome>/` → novas campanhas usam `campanhas/<nome>/`;
- protocolo antigo de criação → substituído por `criacao/README.md`;
- revisão de personagem em quatro blocos dentro do fluxo de campanha → criação atual usa cinco blocos definidos em `criacao/README.md`;
- NPC persistente em `mundo/npcs/` como padrão → campanhas atuais guardam NPCs persistentes/reservados em `mestre/`;
- agrupamento de personagens eventuais como uma única peça → cada personagem com agência possui ficha própria em `personagens/`;
- cânone externo como limite obrigatório de personagem conhecido → o jogador escolhe, altera e consolida a versão canônica local da campanha.

## Estrutura atual de campanha que não pode ser reintroduzida de forma antiga

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

Separação:

```text
PERSONAGENS → quem são as peças
ESTADO      → como as coisas estão agora
MUNDO       → o que existe
MESTRE      → o que é reservado à condução
LIVRO       → o que aconteceu
```

A fonte principal dessa estrutura é `criacao/estrutura-da-campanha.md`.

## Regras mecânicas atuais que não podem ser reintroduzidas de forma antiga

`Custo = patamar efetivamente usado + Ampliação usada`

`Efeito efetivo = Potência usada + 1 + (Perícia efetiva × 0,2)`

`Ataque efetivo = Dano + 1 + (Perícia efetiva × 0,2)`

`Efeito persistente → [D x / V5]`

`Proteção → V5 | Invocação/estrutura equivalente → V10 | Personagem → V35`

`Dissipar → dano contra V de STATUS persistente`

`Contenção por agente → Sustentada pela ação, sem D/V próprio`

`Vários agentes → somam Resultados compatíveis, não Atributos`

## Pendências encontradas na varredura estrutural

A revisão pós-criação encontrou referências antigas ainda presentes em áreas novas. Elas devem ser corrigidas **na própria área correspondente**, sem apagar seus conteúdos mecânicos válidos.

### `personagem/`

Ainda existem referências a:

- `aventuras/<campanha>/personagens/`;
- NPCs persistentes em `mundo/npcs/`;
- revisão em quatro blocos;
- ordem de revisão incluindo NPCs visíveis;
- tratamento antigo de versões canônicas.

Esses pontos devem ser alinhados à criação atual.

### `persistencia/`

STATUS e Progressão continuam válidos como conceitos, mas alguns textos ainda sugerem camadas ou arquivos concretos separados na campanha.

A estrutura atual concentra o presente operacional e fios causais ativos em `estado/atual.md`, distribuindo fatos estáveis para ficha, mundo ou mestre e história ocorrida para livro conforme a natureza da informação.

### `CONTINUIDADE-REVISAO-ATUAL.md`

O checkpoint ainda lista a arquitetura anterior sem `criacao/`. Deve ser atualizado depois que este alinhamento estrutural terminar, para não declarar a varredura concluída antes da hora.

## Regra contra duplicação contraditória

Durante a migração pode existir conteúdo semelhante em dois lugares.

Quando isso ocorrer:

1. verificar se o tema já possui uma referência nova explicitamente aprovada;
2. se possuir, essa referência prevalece;
3. usar o arquivo antigo apenas para recuperar contexto não contraditório ainda não migrado;
4. nunca manter duas regras incompatíveis como igualmente canônicas;
5. correção explícita mais recente do JOGADOR HUMANO tem prioridade sobre formulações anteriores.

## Procedimento de continuação

Antes de retomar uma revisão em outro chat:

1. consultar `CONTINUIDADE-REVISAO-ATUAL.md`;
2. consultar este mapa;
3. consultar o arquivo específico da área nova;
4. recorrer ao arquivo antigo somente se o ponto ainda não estiver coberto;
5. não apagar os originais sem autorização explícita.

> **A estrutura nova é a referência principal onde já foi aprovada; a antiga permanece preservada para história e migração, não para restaurar regras substituídas.**
