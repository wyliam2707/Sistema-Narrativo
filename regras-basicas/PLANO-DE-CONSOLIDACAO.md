# Plano de Consolidação — regras-basicas

Status: EM TRABALHO

Este arquivo acompanha a substituição funcional de `sistema/` por uma estrutura mais leve em `regras-basicas/`.

## Objetivo

```text
NARRADOR A
→ usa somente sistema/

NARRADOR B
→ usa somente regras-basicas/

MESMA CAMPANHA
MESMAS DECLARAÇÕES
→ ambos conseguem executar as funções necessárias da mesa.
```

A meta não é copiar a arquitetura antiga. É preservar função com menos carga operacional.

## Funções já consolidadas

### Tribunal e autoridade

`nucleo/` define Jogador Humano, Jogador IA, Jogador IA Eventual, Opositor e Narrador, com separação de autoridade e conhecimento.

### Agência e continuidade

A função antiga de `sistema/agencia/` foi absorvida por:

```text
Jogadores IA
+ Opositor
+ Registro
+ processos e prazos
```

Não é necessário recriar uma pasta `agencia/`.

### Operação da mesa

```text
situação aberta
→ cadeiras declaram
→ Narrador julga
→ resolve somente quando necessário
→ narra
→ registra
```

### Narração

`mestre/` cobre julgamento, perspectiva, fala, ritmo, descrição, dramatização, resumo e limite da sentença.

### Registro

`registro/` separa passado, presente, conhecimento, mundo, material do Mestre e material do Opositor.

### Fichas e mecânica

`jogador/` e `nucleo/` já possuem a estrutura atual de ficha, Atributos, Perícias, Poderes, Potência, combate, Vida/Mente, Mana, alcance, movimento, iniciativa e recuperação.

### START e retomada — CONSOLIDADO

```text
INICIO-E-RETOMADA.md
```

Uma IA pode carregar uma campanha usando `regras-basicas/` + `campanhas/<nome>/`, reconstruir as cadeiras e consultar detalhes sob demanda.

### Criação de campanha — CONSOLIDADO

```text
CRIACAO-DE-CAMPANHA.md
```

A criação exige somente o suficiente para começar a primeira cena com peças, autoridades e situação inicial claras.

## Próxima etapa

A próxima etapa não é adicionar novos subsistemas.

É testar a equivalência operacional:

```text
regras-basicas/
+
campanhas/<nome>/
```

A IA deve conseguir:

- criar ou retomar campanha;
- montar as cadeiras;
- interpretar fichas;
- receber e julgar declarações;
- resolver ações e combate;
- usar Poderes e recursos;
- manter continuidade e oposição;
- narrar resultados;
- registrar e salvar a história;
- continuar sem consultar `sistema/`.

Quando uma falha aparecer no teste, corrigir somente a função ausente ou ambígua, sem criar especificações preventivas.

## Regra de trabalho

> **Preservar função, remover duplicação e só criar regra quando uma necessidade real aparecer. Complexidade na construção; simplicidade na mesa.**
