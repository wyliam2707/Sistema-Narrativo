# Criação

Status: APROVADO

Esta pasta responde à pergunta:

> **Como uma campanha nasce e fica pronta para começar?**

`criacao/` contém procedimentos de construção. Ela materializa a campanha, transforma conceitos em fichas, conduz aprovação, pareia informações e prepara o estado inicial.

Ela não redefine o conteúdo mecânico da personagem, autoridade das personas, resolução de ações, narração ou persistência.

## Estrutura

```text
criacao/
├── README.md
├── estrutura-da-campanha.md
├── calibracao.md
├── personagem.md
└── pareamento.md
```

- `estrutura-da-campanha.md` — scaffold inicial que deve ser criado;
- `calibracao.md` — como converter conceito/cânone em capacidades mecânicas;
- `personagem.md` — como construir e revisar uma ficha em blocos;
- `pareamento.md` — como verificar consistência entre fichas antes da abertura.

## Princípios

Durante a criação:

- fazer uma pergunta por vez;
- não pedir novamente informação já fornecida;
- interpretar respostas livres normalmente;
- perguntar somente o que ainda fizer diferença real;
- consolidar uma etapa antes de avançar;
- salvar somente conteúdo aprovado;
- não preencher campo de ficha antes do momento de sua revisão.

> **Criação conduz. `personagem/` define o que os campos significam. `persistencia/` define onde a verdade aprovada permanece.**

## Fluxo geral

```text
Nome da campanha
→ materializar estrutura
→ Direção narrativa e cenário
→ registrar protagonista humano
→ registrar demais personagens iniciais com agência
→ confirmar elenco inicial
→ calibrar e revisar fichas
→ parear informações
→ definir início da história
→ consolidar estado inicial
→ CRIAÇÃO: CONCLUÍDA
→ primeira cena
```

Nenhuma ficha entra em revisão enquanto ainda houver personagem inicial com agência a registrar.

A situação inicial só é definida depois que as fichas relevantes foram aprovadas e pareadas.

## Checkpoint

Enquanto a criação estiver em andamento, o `README.md` da campanha registra somente onde retomar.

```text
CRIAÇÃO: EM ANDAMENTO
Etapa atual: Revisão das fichas
Personagem atual: ...
Bloco atual: ...
```

Quando terminar:

```text
CRIAÇÃO: CONCLUÍDA
```

O conteúdo concreto permanece nas fontes próprias; o checkpoint apenas orienta a retomada.

## Etapa — Nome e estrutura

Perguntar o nome e verificar se `campanhas/<nome>/` já existe.

```text
já existe
→ não sobrescrever
→ continuar a existente ou escolher outro nome

nome livre
→ aplicar estrutura-da-campanha.md
→ registrar CRIAÇÃO: EM ANDAMENTO
```

## Etapa — Direção narrativa e cenário

Definir somente o suficiente para saber que campanha está sendo criada, como gênero, tom, foco, ritmo, humor, romance/intimidade e atmosfera quando relevantes.

Durante a criação, registrar apenas aquilo que já foi aprovado e necessário para continuidade.

## Etapa — Registrar protagonista

As três informações universais de nascimento são:

```text
NOME
IMPORTÂNCIA
CONTROLE
```

O protagonista humano usa:

```text
CONTROLE: JOGADOR HUMANO
```

Criar sua ficha usando `../personagem/ficha.md`, preencher apenas os três campos acima e manter:

```text
Status: PENDENTE DE REVISÃO
```

Os demais campos permanecem vazios até `personagem.md` mandar revisá-los.

## Etapa — Registrar outros personagens com agência

Registrar todos os personagens iniciais que terão:

```text
CONTROLE: JOGADOR IA
CONTROLE: JOGADOR IA EVENTUAL
```

Cada peça recebe sua própria ficha. Não iniciar a revisão antes de o JOGADOR HUMANO confirmar que o elenco inicial com agência está completo.

O significado de `CONTROLE` pertence a `../personas/`.

## Etapa — Calibração e revisão

Usar:

```text
calibracao.md
→ transforma Conceito em Patamar, Atributos, Perícias, Poderes e Traços coerentes

personagem.md
→ organiza proposta, discussão, aprovação e salvamento em cinco blocos
```

Os cinco blocos são:

```text
1 - Identidade e Conceito
2 - Patamar, Atributos e Perícias
3 - Poderes e capacidades
4 - Traços, Recursos e relações
5 - Conferência final
```

Por padrão:

```text
JOGADORES IA
→ JOGADORES IA EVENTUAIS
→ protagonista humano
```

Em cada bloco:

```text
propor
→ discutir/corrigir
→ aprovar
→ salvar somente o aprovado
→ avançar checkpoint
```

Depois do Bloco 5:

```text
Status: APROVADO
```

## Etapa — Pareamento

Depois que todas as fichas iniciais estiverem aprovadas, aplicar `pareamento.md`.

O pareamento resolve somente lacunas cruzadas necessárias para iniciar a história sem contradições importantes.

## Etapa — Início da história

Somente depois da revisão e do pareamento, definir a situação concreta inicial em:

```text
campanhas/<nome>/estado/atual.md
```

Quando não houver desgaste previamente estabelecido:

```text
Vida atual = Vida Máxima
Mana atual = Mana Máxima
```

Para `CONTROLE: JOGADOR HUMANO`:

```text
Trama [30]
```

conforme `../personagem/trama.md`.

Se a abertura já estabelecer ferimento, gasto, Status ou outra condição, registrar o estado realmente aprovado.

Depois:

```text
README da campanha
→ CRIAÇÃO: CONCLUÍDA
→ remover checkpoint
→ apontar para estado/atual.md
```

Somente então começar a primeira cena.

## Fronteiras

```text
como construir inicialmente?       → criacao/
o que cada campo/capacidade é?     → ../personagem/
quem decide?                        → ../personas/
como calcular?                      → ../resolucao/
como aplicar durante o jogo?        → ../operacao/
como narrar?                        → ../narracao/
onde guardar depois de estabelecido?→ ../persistencia/
```

## Regra final

> **`criacao/` existe para transformar escolhas aprovadas em uma campanha pronta para jogar. Quando a primeira cena começa, a construção inicial terminou e as demais áreas assumem suas responsabilidades.**
