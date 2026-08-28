# Regras Básicas

Status: CANÔNICO / ATUAL

Esta pasta é a **fonte canônica das regras atuais do Sistema Narrativo**.

Sua finalidade é manter o motor leve, narrativo e executável por IA sem depender de uma segunda camada de regras.

> **Complexidade na construção; simplicidade na mesa.**

## Entrada

```text
Nova campanha
→ CRIACAO-DE-CAMPANHA.md

Nova temporada
→ CRIACAO-DE-TEMPORADA.md

Começar ou continuar campanha
→ INICIO-E-RETOMADA.md
```

## Fluxo de criação

```text
CAMPANHA
→ define sobre o que a história é.

TEMPORADA
→ define o arco atual.

FICHAS
→ definem quem são as personagens e o que precisam levar para decidir de forma coerente nessa história.
```

Quando uma temporada termina:

```text
EPÍLOGO
→ consolida o resultado real.

“E AGORA?”
→ abre a definição da próxima direção.
```

Problemas ainda abertos continuam verdadeiros, mas não escolhem automaticamente o próximo arco.

## Regra de localização

`regras-basicas/` contém somente regras, procedimentos e modelos de funcionamento.

Nenhum estado vivo de campanha deve ser armazenado aqui.

```text
regras-basicas/
→ como o sistema funciona.

campanhas/<nome>/
→ o que é verdade naquela mesa.
```

> **Regra fica aqui. Verdade concreta fica na campanha.**

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

Regras comuns: resolução, combate, tempo, alcance, movimento, Vida, Mente, Mana, Potência e autoridade das cadeiras.

Também define:

```text
JOGADOR HUMANO
JOGADOR IA
JOGADOR IA EVENTUAL
OPOSITOR
NARRADOR
```

Iniciativa de uma peça não concede autoridade sobre as demais. Conhecimento técnico da IA não se transforma automaticamente em conhecimento da personagem.

### Jogador

Ficha, Atributos, Perícias, Poderes, equipamentos, Traços, Recursos e interpretação da própria personagem.

```text
ATRIBUTO + PERÍCIA
→ mede execução.

PODER / EQUIPAMENTO
→ capacidade extraordinária utilizável e graduável.

TRAÇO
→ verdade absoluta dentro da descrição aprovada.

RECURSO
→ posse, acesso ou infraestrutura estável.
```

A ficha é a principal fonte de interpretação da personagem, mas não substitui cenário, Livro ou outras fontes externas quando elas forem necessárias.

Blocos interpretativos devem priorizar aquilo que realmente pode mudar decisões dentro do foco da campanha.

### Mestre

Julgamento e apresentação da sentença: interpretar intenções, aplicar verdades relevantes, testar somente quando existir incerteza real, narrar o resultado e parar quando surgir nova decisão voluntária.

```text
mestre/narrativa.md
→ identidade persistente da campanha.

mestre/roteiro.md
→ temporada ativa.
```

O Mestre julga; não joga pelo Opositor nem transforma iniciativa do protagonista em obediência alheia.

### Opositor

Movimenta o lado adversarial dentro de conhecimento, meios, tempo e oportunidades legítimos.

Planos, processos e prazos reais pertencem à campanha correspondente.

Oposição nova não deve ser criada retroativamente para invalidar uma solução já declarada ou julgada.

### Registro

Preserva o que precisa continuar verdadeiro e define onde salvar dentro de `campanhas/<nome>/`.

```text
registro/fontes-da-campanha.md
→ onde cada verdade pertence.

registro/salvar-a-historia.md
→ salvar sem continuar jogando.

registro/fechar-capitulo.md
→ checkpoint, reset operacional e reancoragem.

registro/estado-atual.md
→ fotografia do presente.

registro/livro-e-capitulos.md
→ histórico canônico.

registro/canonizacao-e-correcoes.md
→ mudanças permanentes e correções de cânone.
```

## Roteamento simples

```text
Criar campanha
→ CRIACAO-DE-CAMPANHA.md

Criar próxima temporada
→ CRIACAO-DE-TEMPORADA.md

Começar ou continuar
→ INICIO-E-RETOMADA.md

Regra comum a todos
→ nucleo/

Ficha ou capacidade própria de personagem
→ jogador/

Julgamento ou apresentação imparcial
→ mestre/

Decisão adversarial
→ opositor/

Algo precisa continuar verdadeiro
→ registro/

Corrigir fato já canônico ou consolidar mudança permanente
→ registro/canonizacao-e-correcoes.md
```

## Carregamento

Não reler toda a árvore por hábito.

```text
entrada da campanha
→ carregar núcleo operacional.

situação exige detalhe específico
→ consultar a regra pertinente.

fim de capítulo
→ seguir registro/fechar-capitulo.md e reancorar as fontes essenciais.
```

O sistema deve operar por **consulta sob demanda**, não por carregamento integral obrigatório de todo arquivo em toda sessão.

## Vigência dos arquivos

A partir desta consolidação, `regras-basicas/` substitui integralmente a antiga árvore `sistema/`.

Cabeçalhos editoriais antigos dentro de alguns arquivos, como `REFORMULAÇÃO / NÃO IMPLEMENTADO`, não reativam regras removidas nem tornam `sistema/` necessário. A vigência operacional é definida por esta pasta e pelas regras atuais nela contidas; um arquivo só deixa de valer se estiver explicitamente marcado como rascunho, legado ou incompatível.

## Regra de trabalho

Não criar subsistema preventivamente.

```text
necessidade real aparece
→ identificar a função ausente ou ambígua
→ corrigir somente essa função
→ manter o restante simples.
```

> **Preservar função, remover duplicação e criar regra somente quando ela realmente evita ambiguidade ou perda de continuidade.**
