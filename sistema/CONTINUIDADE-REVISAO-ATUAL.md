# Continuidade Atual — Revisão do Sistema

Status: CHECKPOINT PARA RETOMADA
Data do checkpoint: 2026-08-22
Branch de trabalho: `revisao/personagem`

Este arquivo resume somente o estado atual da revisão. Arquivos antigos continuam preservados como fontes históricas de migração, mas não prevalecem quando uma regra nova explicitamente aprovada os substitui.

## 1. Estado da campanha usada como teste

A campanha `Castelo dos Corvos` permanece PAUSADA enquanto o sistema é revisado.

Não avançar a ficção automaticamente. Usar a campanha apenas como evidência ou exemplo mecânico até o JOGADOR HUMANO pedir explicitamente para retomá-la.

## 2. Arquitetura atual

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

Responsabilidades:

`personagem/ → quem a entidade é e do que é capaz` | `personas/ → quem decide` | `resolucao/ → o que acontece` | `agencia/ → continuidade de vontade própria` | `narracao/ → como mostrar` | `persistencia/ → o que permanece` | `operacao/ → ordem de aplicação`.

## 3. Personas e ciclo

Axioma:

> **Os JOGADORES movem suas peças. O OPOSITOR move o cenário. O NARRADOR organiza, julga e registra.**

Papéis:

`JOGADOR HUMANO | JOGADOR IA | JOGADOR IA EVENTUAL | OPOSITOR | NARRADOR`

Ciclo atual:

`JOGADOR HUMANO → JOGADOR IA → EVENTUAL → OPOSITOR → NARRADOR organiza/consulta/julga/apresenta/registra → nova janela`

A resolução termina quando a consequência volta a exigir escolha.

## 4. Personagem — atributos atuais

A ficha usa quatro Atributos universais:

`FIS | RES | MEN | VON`

- `FIS` — capacidade corporal: força, velocidade, coordenação, reação, precisão física, equilíbrio e movimento;
- `RES` — quanto o corpo/estrutura suporta;
- `MEN` — perceber, compreender, raciocinar, lembrar, analisar e executar precisão mental quando pertinente;
- `VON` — determinação, resistência mental, sustentação e imposição volitiva quando pertinente.

Princípio:

> **FIS age. RES suporta.**

A ficha descreve o personagem; não existe distribuição para produzir justiça entre personagens.

Atributo, Perícia, Poder e equipamento não são somados automaticamente.

Exemplo: `FIS [2] | Pistola Dano [1] | Espada Mágica Dano [3]` lê `corpo [2] | pistola [1] | espada [3]`, sem `2+3`.

## 5. Escalas da ficha

Atributos: `[0]–[5]`, qualitativos e não lineares.

`[0] humano | [1] além do humano | [2] super-humano | [3] poderoso | [4] extremo | [5] ápice`

Perícias: abertas, `[+0]–[+5]`. O específico prevalece sobre o geral; não se somam.

Poderes: `[1]–[5]`, organizados por fonte/repertório. Poder `[0]` não existe. Uma capacidade estável de equipamento pode ser Poder.

TRAÇOS são verdades qualitativas estáveis, sem grau numérico.

REL registra relação recorrente de `-5` a `+5` sem modificador automático.

## 6. Princípio de resolução

`RESULTADO EVIDENTE → estabelece | IMPOSSIBILIDADE EVIDENTE → estabelece | INCERTEZA REAL → resolve`

Motor geral:

`Perícia efetiva = Perícia de aplicação − Perícia de oposição`

`Efeito efetivo = Potência usada + 1 + (Perícia efetiva × 0,2)`

`Resultado/Progresso = 2^(Efeito efetivo − Resistência efetiva)`

Não existe `Ampliação não paga`.

## 7. Combate e Dano

`Ataque efetivo = Dano + 1 + (Perícia efetiva × 0,2)`

`Dano aplicado = 2^(Ataque efetivo − Defesa efetiva)`

Referência sem diferença de Perícia:

`igual → 2 | +1 → 4 | +2 → 8 | +3 → 16 | +4 → 32 | +5 → 64 | -1 → 1 | -2 → 0,5 | -3 → 0,25`

Dano abaixo de `0,25` não é acumulado. Mesmo `0,25` não cria capacidade de afetar um alvo quando o mecanismo é ficcionalmente incapaz.

VIDA de personagem:

`0–4 Ileso | 5–9 Ferido | 10–14 Ferido* | 15–19 Grave | 20–24 Grave* | 25–29 Crítico | 30–34 Crítico* | 35 Incapacitado`

Incapacitado não significa morto.

## 8. Energia e Ampliação

Reserva pelo maior Atributo:

`[0]→10 | [1]→20 | [2]→40 | [3]→60 | [4]→80 | [5]→100`

Quando uma capacidade consome Energia:

`Custo = patamar efetivamente usado + Ampliação usada`

A Ampliação é paga integralmente antes da resolução. Se não houver Energia suficiente, o JOGADOR reduz potência usada, Ampliação ou ambas antes de resolver.

Limite de Ampliação:

`Ampliação [X] = patamar máximo do efeito + maior entre MEN e VON`

Dimensões gerais:

`Alcance | Alvos | Área/Tamanho | Duração`

Alcance:

`Toque → Curto → Médio → Longo → Visão → Simpático`

Alvos:

`1 +0 | 2 +1 | 4 +2 | 8 +3 | 16 +4 | 32 +5`

Área/Tamanho:

`Pontual/Humano +0 | Pequena +1 | Média +2 | Grande +3 | Enorme +4 | Massiva +5`

Duração:

`Instantâneo → Cena → Hora → Dia → Semana → Permanente`

## 9. Efeitos persistentes e Graus de Vida

`1 grau de Vida = 5`

Referência:

`Efeito persistente → V5 | Proteção/Barreira → V5 | Invocação/estrutura equivalente → V10 | Personagem → V35`

Todo efeito persistente, benéfico ou prejudicial:

`Efeito [D x / V5] — Duração`

`D` é a Defesa estrutural, normalmente o Efetivo que estabeleceu o efeito.

Perder Vida não reduz a intensidade do efeito. Enquanto `V > 0`, ele permanece integral; em `V0`, termina.

## 10. Dissipar

Dissipar é efeito próprio de Dano contra STATUS persistente:

`Dissipar efetivo vs D do STATUS → Dano aplicado → reduz V`

Base:

`Dissipar — Médio / 1 alvo / Pontual / Instantâneo / 1 STATUS / Efetivo máximo [nível]`

Quantidade específica de STATUS:

`1 +0 | 2 +1 | 4 +2 | 6 +3 | 16 +4 | 32 +5`

STATUS, Alvos e Área são dimensões diferentes e podem ser ampliadas separadamente.

## 11. Invocação e Transformação

Invocação base:

`Médio / 1 criação / Tamanho Humano / Cena`

Criação invocada:

`D = RES | V10`

Distribuição com os quatro Atributos:

`Inv [1] → 1 atributo [1]` | `Inv [2] → 1[2] ou 2[1]` | `Inv [3] → 1[3] ou 2[2] ou 3[1]` | `Inv [4] → 1[4] ou 2[3] ou 3[2] ou 4[1]` | `Inv [5] → 1[5] ou 2[4] ou 3[3] ou 4[2]`.

Transformação física redefine `FIS` e `RES`; `MEN`, `VON`, VIDA e Energia permanecem originais.

`T1 → [1]/[0] | T2 → [2]/[0] ou [1]/[1] | T3 → [3]/[0] ou [2]/[2] | T4 → [4]/[0] ou [3]/[3] | T5 → [5]/[0] ou [4]/[4]`.

## 12. Contenção

Três estruturas diferentes:

`Poder Imobilizar → efeito persistente D/V5`

`Personagem/Invocação viva segurando → condição Sustentada pela ação do agente, sem D/V próprio`

`Algemas/estrutura física → estrutura própria, ex. FIS [3] | V10`

Em contenção sustentada, cada agente gasta ação para manter. O alvo continua escolhendo ações coerentes: escapar, atacar quem o segura, usar magia possível etc.

Vários agentes não somam Atributos. Cada um resolve; Resultados compatíveis podem ser somados na mesma janela.

Exemplo: `4 guardas FIS [2] vs alvo FIS [2] → 2+2+2+2 = 8 → Imobilizado [8] — Sustentado`.

## 13. STATUS

STATUS é atualizado assim que a consequência é estabelecida.

Exemplos compactos:

`Cegueira [D2,4 / V5] — Cena | Proteção [D3,0 / V5] — Cena | Imobilizado [8] — Sustentado por 4 guardas | Algemado — Algemas [FIS3 / V10]`.

STATUS registra o presente; ficha registra quem o personagem é.

## 14. Migração

Não apagar os arquivos antigos durante a revisão.

Quando uma formulação antiga contradiz uma regra nova explicitamente aprovada, a regra nova prevalece. `MIGRACAO-ESTRUTURAL.md` registra a arquitetura e as referências principais.

## 15. Estado atual da revisão

A varredura de consistência iniciada em 2026-08-22 alinhou os arquivos principais de `personagem/`, `resolucao/`, `persistencia/`, `operacao/` e `agencia/` às regras acima.

Não existe uma próxima mecânica presumida neste checkpoint. Ao retomar, consultar este arquivo e os arquivos específicos da área antes de escolher o próximo conceito a revisar.

## Regra de retomada

1. consultar `CONTINUIDADE-REVISAO-ATUAL.md`;
2. consultar `MIGRACAO-ESTRUTURAL.md`;
3. usar a arquitetura nova como referência principal nas áreas já substituídas;
4. consultar arquivos antigos somente como fonte histórica nos pontos ainda não migrados;
5. não apagar ou mesclar conteúdo antigo sem autorização explícita;
6. manter `Castelo dos Corvos` pausado até pedido explícito de retomada.
