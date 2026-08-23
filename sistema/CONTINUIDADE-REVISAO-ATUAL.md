# Continuidade Atual — Revisão do Sistema

Status: CHECKPOINT PARA RETOMADA
Data do checkpoint: 2026-08-23
Branch de trabalho: `revisao/personagem`

Este arquivo resume o estado atual da revisão.

Arquivos antigos continuam preservados como fontes históricas de migração, mas não prevalecem quando uma regra nova explicitamente aprovada os substitui.

## 1. Arquitetura atual

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
criacao/      → como uma campanha nasce e onde seus dados são salvos
personagem/   → quem a entidade é e do que é capaz
personas/     → quem decide
resolucao/    → o que acontece
agencia/      → continuidade de vontade própria
narracao/     → como mostrar
persistencia/ → o que permanece e onde salvar
operacao/     → ordem de aplicação
```

## 2. Entrada atual do sistema

```text
NOVA CAMPANHA
→ sistema/criacao/README.md

CONTINUAR
→ campanhas/<nome>/README.md
```

`sistema/00-LEIA-PRIMEIRO.md` é o roteador atual.

`aventuras/` e os antigos protocolos diretamente em `sistema/` permanecem como legado e não são apagados nem migrados automaticamente.

## 3. Estrutura atual de campanha

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

A fonte principal é `sistema/criacao/estrutura-da-campanha.md`.

## 4. Processo de criação aprovado

A criação usa:

```text
Nome da campanha
→ Direção narrativa e cenário
→ Protagonista
→ Personagens com agência de jogador
→ Início da história
→ Revisão mecânica e aprovação
```

Princípios consolidados:

- conceito primeiro, mecânica depois;
- cada informação possui uma fonte principal;
- checkpoint da criação fica no `README.md` da própria campanha;
- conteúdo ainda em discussão não é persistido como definitivo;
- cada bloco mecânico aprovado é salvo imediatamente;
- personagens com agência possuem fichas individuais;
- `GERÊNCIA` é linguagem de escolha; o dado persistido é `CONTROLE`;
- personagens conhecidos usam a versão escolhida e modificada pelo jogador como cânone local;
- nova campanha nunca sobrescreve automaticamente uma campanha existente;
- arquivos operacionais iniciais usam modelos determinísticos definidos em `estrutura-da-campanha.md`;
- depois da última ficha aprovada, `estado/atual.md` é consolidado automaticamente, o README recebe `CRIAÇÃO: CONCLUÍDA` e somente então começa a primeira cena.

Ordem da revisão mecânica inicial:

```text
JOGADOR IA
→ JOGADOR IA EVENTUAL
→ protagonista
```

Blocos:

```text
1 - Identidade e conceito
2 - Atributos e perícias
3 - Poderes e capacidades
4 - Traços e relações
5 - Conferência final
```

## 5. Personas e ciclo operacional

Axioma:

> **Os JOGADORES movem suas peças. O OPOSITOR move o cenário. O NARRADOR organiza, julga e registra.**

Papéis atuais:

```text
JOGADOR HUMANO
JOGADOR IA
JOGADOR IA EVENTUAL
OPOSITOR
NARRADOR
```

A referência atual do ciclo é:

```text
sistema/operacao/ciclo-de-cena.md
```

Uma persona `JOGADOR IA EVENTUAL` pode administrar várias peças autorizadas, mas cada personagem continua com ficha, conhecimento, relações e objetivos próprios.

## 6. Personagem — atributos atuais

A ficha usa quatro Atributos universais:

```text
FIS | RES | MEN | VON
```

- `FIS` — capacidade corporal de agir: força, velocidade, coordenação, reação, precisão física, equilíbrio e movimento;
- `RES` — quanto o corpo ou estrutura suporta;
- `MEN` — perceber, compreender, raciocinar, lembrar, analisar e executar precisão mental quando pertinente;
- `VON` — determinação, resistência mental, sustentação e imposição volitiva quando pertinente.

Princípio:

> **FIS age. RES suporta.**

Atributo, Perícia, Poder e equipamento não são somados automaticamente.

## 7. Escalas da ficha

Atributos: `[0]–[5]`, qualitativos e não lineares.

```text
[0] humano
[1] além do humano
[2] super-humano
[3] poderoso
[4] extremo
[5] ápice
```

Perícias: abertas, `[+0]–[+5]`.

Poderes: `[1]–[5]`, organizados por fonte/repertório. Poder `[0]` não existe.

TRAÇOS são verdades qualitativas estáveis sem grau numérico.

REL registra relações recorrentes de `-5` a `+5` sem modificador automático.

## 8. Princípio de resolução

```text
RESULTADO EVIDENTE       → estabelece
IMPOSSIBILIDADE EVIDENTE → estabelece
INCERTEZA REAL           → resolve
```

Motor geral:

```text
Perícia efetiva = Perícia de aplicação − Perícia de oposição

Efeito efetivo = Potência usada + 1 + (Perícia efetiva × 0,2)

Resultado/Progresso = 2^(Efeito efetivo − Resistência efetiva)
```

Não existe `Ampliação não paga`.

## 9. Combate e Dano

```text
Ataque efetivo = Dano + 1 + (Perícia efetiva × 0,2)

Dano aplicado = 2^(Ataque efetivo − Defesa efetiva)
```

Referência sem diferença de Perícia:

```text
igual → 2
+1 → 4
+2 → 8
+3 → 16
+4 → 32
+5 → 64
-1 → 1
-2 → 0,5
-3 → 0,25
```

Dano abaixo de `0,25` não é acumulado. Mesmo `0,25` não cria capacidade ficcional inexistente de afetar o alvo.

VIDA de personagem:

```text
0–4   Ileso
5–9   Ferido
10–14 Ferido*
15–19 Grave
20–24 Grave*
25–29 Crítico
30–34 Crítico*
35    Incapacitado
```

Incapacitado não significa morto.

## 10. Energia e Ampliação

Reserva pelo maior Atributo:

```text
[0] → 10
[1] → 20
[2] → 40
[3] → 60
[4] → 80
[5] → 100
```

Quando uma capacidade consome Energia:

```text
Custo = patamar efetivamente usado + Ampliação usada
```

A Ampliação é paga integralmente antes da resolução.

Limite:

```text
Ampliação [X] = patamar máximo do efeito + maior entre MEN e VON
```

Dimensões gerais:

```text
Alcance | Alvos | Área/Tamanho | Duração
```

## 11. Efeitos persistentes e Vida estrutural

```text
1 grau de Vida = 5
```

Referência:

```text
Efeito persistente             → V5
Proteção/Barreira              → V5
Invocação/estrutura equivalente→ V10
Personagem                     → V35
```

Todo efeito persistente consolidado:

```text
Efeito [D x / V5] — Duração
```

Perder Vida não reduz sua intensidade. Enquanto `V > 0`, o efeito permanece integral; em `V0`, termina.

## 12. Dissipar

Dissipar é efeito próprio de Dano contra STATUS persistente:

```text
Dissipar efetivo vs D do STATUS
→ Dano aplicado
→ reduz V
```

STATUS, Alvos e Área são dimensões diferentes e podem ser ampliadas separadamente quando a regra específica permitir.

## 13. Invocação, Transformação e Contenção

Invocação base:

```text
Médio / 1 criação / Tamanho Humano / Cena
```

Criação invocada:

```text
D = RES | V10
```

Transformação física redefine `FIS` e `RES`; `MEN`, `VON`, VIDA e Energia permanecem originais salvo regra específica.

Contenção distingue:

```text
Poder Imobilizar
→ efeito persistente D/V5

Personagem/Invocação viva segurando
→ condição Sustentada pela ação do agente, sem D/V próprio

Algemas/estrutura física
→ estrutura própria, por exemplo FIS [3] | V10
```

Vários agentes não somam Atributos. Resultados compatíveis podem ser somados quando representam a mesma contenção coordenada.

## 14. Persistência atual

STATUS continua sendo o conceito de **como o personagem está agora**.

Progressão continua sendo o conceito de **consequência estabelecida que ainda possui potencial causal futuro**.

Na estrutura atual, eles não exigem arquivos separados na campanha.

```text
estado/atual.md
→ Vida/Energia atuais
→ condições e efeitos ativos
→ localização
→ situações em andamento
→ intenções futuras ainda ativas
→ fios causais pendentes
→ demais dados necessários para continuar agora
```

Quando a natureza de um fato muda:

```text
parte estável do personagem → personagens/
verdade estável do cenário  → mundo/
material reservado          → mestre/
história ocorrida           → livro/
```

## 15. Varredura estrutural concluída em 2026-08-23

Depois da consolidação do novo processo de criação, foram revisadas as pastas atuais para impedir que regras antigas voltassem por caminhos internos.

Corrigidos:

- `sistema/00-LEIA-PRIMEIRO.md`;
- `sistema/MIGRACAO-ESTRUTURAL.md`;
- `sistema/personagem/README.md`;
- `sistema/personagem/criacao.md`;
- `sistema/personagem/npcs.md`;
- `sistema/persistencia/README.md`;
- `sistema/persistencia/material-reservado.md`;
- `sistema/operacao/README.md`;
- `sistema/narracao/README.md`.

Revisados sem necessidade de alteração estrutural nesta rodada:

- `sistema/personas/`;
- `sistema/agencia/`;
- `sistema/resolucao/`.

As regras mecânicas internas dessas áreas permanecem válidas conforme seus próprios documentos aprovados.

## 16. Material legado

Não apagar automaticamente arquivos antigos durante a revisão.

Quando uma formulação antiga contradiz uma regra nova explicitamente aprovada, a regra nova prevalece.

Referência de migração:

```text
sistema/MIGRACAO-ESTRUTURAL.md
```

## 17. Estado da campanha usada como teste

A campanha `Castelo dos Corvos` permanece PAUSADA enquanto o sistema é revisado.

Não avançar a ficção automaticamente. Usá-la apenas como evidência ou exemplo mecânico até pedido explícito de retomada.

## Regra de retomada

1. consultar `CONTINUIDADE-REVISAO-ATUAL.md`;
2. consultar `MIGRACAO-ESTRUTURAL.md`;
3. usar as subpastas atuais como referência principal nas áreas já substituídas;
4. consultar arquivos antigos somente nos pontos ainda não migrados;
5. para criação, usar `criacao/README.md`;
6. para campanhas atuais, começar por `campanhas/<nome>/README.md`;
7. não apagar ou mesclar conteúdo antigo sem autorização explícita.

> **A arquitetura atual governa o sistema. O legado permanece preservado para migração, não para restaurar regras substituídas.**
