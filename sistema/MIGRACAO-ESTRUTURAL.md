# Migração Estrutural do Sistema

Status: CONCLUÍDA

Este arquivo registra historicamente a transição da estrutura antiga, concentrada diretamente em `sistema/`, para a arquitetura atual em subpastas.

> **A migração terminou. Este documento não é fonte operacional de regra; as subpastas atuais são canônicas.**

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

Todas as oito áreas são referências atuais para seus respectivos temas.

```text
criacao/      → nascimento e estrutura de campanha
personagem/   → definição estável das peças
personas/     → autoridade e controle
resolucao/    → resultado e mecânicas
agencia/      → continuidade de vontade e ganchos
narracao/     → apresentação da sentença
persistencia/ → estado, livro, cânone e salvamento
operacao/     → sequência de jogo e administração
```

## Porta de entrada

```text
NOVA CAMPANHA
→ sistema/criacao/README.md

CONTINUAR
→ campanhas/<nome>/README.md
```

Roteador geral:

```text
sistema/00-LEIA-PRIMEIRO.md
```

## Legados removidos

Em 2026-08-23, depois de revisão e confirmação explícita, foram removidos os documentos antigos ou temporários abaixo.

### Primeira limpeza

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

### Limpeza final

```text
sistema/agencia-de-personagens.md
sistema/modo-rpg.md
sistema/checklist-do-narrador.md
sistema/narracao-e-escrita-padrao.md
sistema/exemplo-de-estilo.md
sistema/comandos-administrativos.md
sistema/criacao/PENDENCIAS.md
sistema/personagem/MAPA-DE-ORIGEM.md
sistema/CONTINUIDADE-REVISAO-ATUAL.md
```

Esses caminhos não são mais fontes válidas e não devem ser recriados para restaurar formulações antigas.

## Substituições principais

```text
calibracao-independente.md
→ personagem/calibracao.md

modelos.md
→ personagem/ficha.md + arquivos especializados

protocolo-de-criacao.md
→ criacao/README.md + criacao/estrutura-da-campanha.md

ciclo-de-jogadores.md + modo-rpg.md + checklist-do-narrador.md
→ personas/ + operacao/

resolucao-de-acoes.md + informacao-e-descoberta.md
→ resolucao/

agencia-de-personagens.md
→ agencia/ + personas/

narracao-e-escrita-padrao.md + exemplo-de-estilo.md
→ narracao/

progressao-narrativa.md + protocolo-de-fechamento-de-capitulo.md
→ persistencia/

comandos-administrativos.md
→ operacao/comandos-administrativos.md
```

## Regras estruturais que substituíram o modelo antigo

```text
Atributos
→ FIS | RES | MEN | VON

campanha atual
→ campanhas/<nome>/

NPC persistente reservado
→ mestre/ em vez de mundo/npcs/ como padrão

estado operacional
→ estado/atual.md

controle
→ JOGADOR HUMANO | JOGADOR IA | JOGADOR IA EVENTUAL | NPC

mesa
→ JOGADORES declaram
→ OPOSITOR apresenta movimento/oposição
→ NARRADOR julga, narra a sentença e registra

combate
→ turnos simultâneos de 10 segundos

aplicação imediata
→ 10 segundos
```

## Regras mecânicas consolidadas

```text
Custo = patamar efetivamente usado + Ampliação usada

Efeito efetivo = Potência usada + 1 + (Perícia efetiva × 0,2)

Resultado/Progresso = 2^(Efeito efetivo − Resistência efetiva)

Ataque efetivo = Dano + 1 + (Perícia efetiva × 0,2)

Efeito persistente → [D x / V5]

Proteção → V5
Invocação → V10
Personagem → V35

Dissipar → dano contra V de STATUS persistente

Contenção por agente → Sustentada, sem D/V próprio

Vários agentes → somam Resultados compatíveis, não Atributos
```

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
MESTRE      → material reservado
LIVRO       → o que aconteceu
```

## Material que continua legado

Campanhas antigas em:

```text
aventuras/
```

continuam preservadas como material de campanha legado e não são convertidas automaticamente.

Isso é diferente dos antigos documentos universais de `sistema/`, cuja migração foi concluída.

## Regra final

> **A arquitetura atual é a única fonte operacional do sistema. Este arquivo existe apenas para registrar a migração concluída e impedir que documentos removidos sejam restaurados por engano.**
