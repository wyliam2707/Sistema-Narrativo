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
├── personas/
├── resolucao/
├── agencia/
├── narracao/
├── persistencia/
├── operacao/
└── personagem/
```

### `personagem/`
Status: `REFERÊNCIA PRINCIPAL`.

Responsabilidade: definição estável de personagens, criação, calibração, escala, `FIS | RES | MEN | VON`, Perícias, Poderes, TRAÇOS, REL, ficha e NPCs.

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
Status: `REFERÊNCIA PRINCIPAL`.

Responsabilidade: STATUS, Progressão, atualização de ficha, Livro, fechamento de capítulo, material reservado e correção de cânone.

### `operacao/`
Status: `REFERÊNCIA PRINCIPAL` para o ciclo de cena.

Responsabilidade: ordem das declarações, consulta, julgamento, ponto de parada e registro. `operacao/ciclo-de-cena.md` substitui o ciclo operacional antigo onde houver conflito.

## Mapa das principais fontes antigas

| Arquivo antigo | Área nova principal | Situação atual |
|---|---|---|
| `README.md` | `personagem/` + `resolucao/` | FONTE HISTÓRICA nas regras já migradas |
| `00-LEIA-PRIMEIRO.md` | `operacao/` | FONTE HISTÓRICA / pontos ainda não migrados podem ser consultados |
| `ciclo-de-jogadores.md` | `operacao/` + `personas/` | FONTE HISTÓRICA; ciclo atual em `operacao/ciclo-de-cena.md` |
| `agencia-de-personagens.md` | `agencia/` | FONTE HISTÓRICA para pontos ainda não reescritos |
| `narracao-e-escrita-padrao.md` | `narracao/` | FONTE HISTÓRICA ainda útil para estilo |
| `modo-rpg.md` | `operacao/` | FONTE HISTÓRICA para procedimentos ainda não migrados |
| `checklist-do-narrador.md` | `operacao/` | FONTE HISTÓRICA para itens ainda não migrados |
| `protocolo-de-fechamento-de-capitulo.md` | `persistencia/` | FONTE HISTÓRICA; nova referência em `persistencia/fechamento-de-capitulo.md` |

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
- ciclo antigo quando conflitante → substituído por `operacao/ciclo-de-cena.md`.

## Regras estruturais atuais que não podem ser reintroduzidas de forma antiga

`Custo = patamar efetivamente usado + Ampliação usada`

`Efeito efetivo = Potência usada + 1 + (Perícia efetiva × 0,2)`

`Ataque efetivo = Dano + 1 + (Perícia efetiva × 0,2)`

`Efeito persistente → [D x / V5]`

`Proteção → V5 | Invocação/estrutura equivalente → V10 | Personagem → V35`

`Dissipar → dano contra V de STATUS persistente`

`Contenção por agente → Sustentada pela ação, sem D/V próprio`

`Vários agentes → somam Resultados compatíveis, não Atributos`

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
