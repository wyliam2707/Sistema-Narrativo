# Regras Básicas

Status: REFORMULAÇÃO / NÃO IMPLEMENTADO

Esta pasta existe para reconstruir e simplificar as regras fundamentais do Sistema Narrativo sem alterar automaticamente as regras aprovadas atuais.

## Entrada

```text
Nova campanha
→ CRIACAO-DE-CAMPANHA.md

Nova temporada
→ CRIACAO-DE-TEMPORADA.md

Continuar campanha
→ INICIO-E-RETOMADA.md
```

Esses arquivos são portas de entrada. Eles reutilizam as áreas existentes e não criam uma segunda camada de operação.

## Fluxo de criação

```text
PASSO 01 — CAMPANHA
→ define a narrativa persistente.

PASSO 02 — TEMPORADA
→ cria o arco atual com começo e encerramento.

PASSO 03 — FICHAS
→ usa campanha + temporada para decidir o que precisa ser definido nas personagens.
```

Cada passo serve de base para o seguinte sem predeterminar suas respostas.

```text
CAMPANHA
→ sobre o que a história é.

TEMPORADA
→ como esse foco será explorado agora.

FICHAS
→ quem são as personagens e o que precisam levar para tomar decisões coerentes nesta história.
```

Quando uma temporada termina:

```text
EPÍLOGO
→ consolida como ela realmente terminou.

“E AGORA?”
→ define a direção da próxima temporada.
```

Problemas abertos não escolhem automaticamente o próximo arco.

## Regra de localização

`regras-basicas/` contém somente **regras, procedimentos e modelos de funcionamento**.

Nenhum estado vivo de uma campanha deve ser armazenado aqui.

```text
regras-basicas/
→ como o sistema funciona
→ regras de resolução
→ autoridade das personas
→ procedimentos
→ modelos de ficha e registro

campanhas/<nome>/
→ o que é verdade naquela campanha
→ narrativa persistente
→ roteiro da temporada ativa
→ fichas reais
→ estado atual
→ conhecimentos
→ relações
→ processos em andamento
→ prazos
→ eventos futuros estabelecidos
→ planos do Opositor
→ registros do Narrador
→ livro e demais dados da campanha
```

> **Regra fica em `regras-basicas/`. Verdade da mesa fica em `campanhas/<nome>/`.**

## Estrutura

```text
regras-basicas/
├── CRIACAO-DE-CAMPANHA.md
├── CRIACAO-DE-TEMPORADA.md
├── INICIO-E-RETOMADA.md
├── nucleo/
├── jogador/
├── mestre/
├── opositor/
└── registro/
```

### Núcleo

Regras comuns usadas por todos: resolução, combate, tempo, alcance, Vida, Mente, Mana, Potência e autoridade das cadeiras.

### Jogador

Ficha, Atributos, Perícias, Poderes, equipamentos, Traços, Recursos e uso da própria personagem.

A linguagem central é:

```text
ATRIBUTO + PERÍCIA
→ mede execução.

PODER / EQUIPAMENTO
→ capacidade extraordinária utilizável e graduável.

TRAÇO
→ verdade absoluta daquela personagem dentro da descrição aprovada.

RECURSO
→ posse, acesso ou infraestrutura estável sustentada pela história.
```

A ficha da personagem é sua principal fonte de interpretação. Ela preserva personalidade, desejos, medos, hábitos, relações e conhecimento relevante sem precisar duplicar livros ou cenário inteiro.

Os blocos interpretativos não precisam responder às mesmas perguntas em toda campanha. Eles são orientados pela Narrativa da Campanha e pelo Roteiro da Temporada.

```text
FICHA
→ quem a personagem é e o que precisa permanecer disponível para interpretá-la nesta história.

ESTADO ATUAL
→ como ela está agora.

LIVROS / CENÁRIO / ARQUIVOS
→ contexto externo consultado quando necessário.
```

Traço não é bônus. Quando relevante, o Narrador aplica exatamente a verdade descrita e somente depois resolve o que ainda permanecer incerto.

### Mestre

Julgamento e apresentação da sentença: quando testar, como interpretar, aplicar Traços relevantes, narrar, manter perspectiva e parar diante de nova escolha.

O Mestre preserva duas direções diferentes:

```text
mestre/narrativa.md
→ identidade persistente da campanha.

mestre/roteiro.md
→ temporada ativa.
```

O Mestre não controla o Opositor.

### Opositor

Decisões e continuidade do lado adversarial.

Planos e prazos reais pertencem à campanha correspondente.

### Registro

Regras sobre o que precisa permanecer verdadeiro e onde salvar dentro de `campanhas/<nome>/`.

## Roteamento simples

```text
Quero criar uma campanha
→ CRIACAO-DE-CAMPANHA.md

Quero criar a próxima temporada
→ CRIACAO-DE-TEMPORADA.md

Quero começar ou continuar
→ INICIO-E-RETOMADA.md

É uma regra comum a todos?
→ Núcleo

É ficha, capacidade ou verdade própria de personagem?
→ Jogador

É julgamento ou narração imparcial?
→ Mestre

É decisão adversarial?
→ Opositor

Precisa continuar verdadeiro?
→ Registro
```

## Princípio de trabalho

```text
regra nova
→ discutir
→ testar
→ registrar aqui
→ revisar
→ somente depois substituir a regra antiga correspondente
```

Enquanto a reformulação estiver em andamento, os arquivos desta pasta não substituem automaticamente as regras aprovadas em `sistema/`.

## Direção

A meta é reduzir consultas durante a sessão e deixar o sistema simples de executar por uma IA.

> **Complexidade na construção; simplicidade na mesa.**
