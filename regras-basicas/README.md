# Regras Básicas

Status: REFORMULAÇÃO / NÃO IMPLEMENTADO

Esta pasta existe para reconstruir e simplificar as regras fundamentais do Sistema Narrativo sem alterar automaticamente as regras aprovadas atuais.

## Estrutura

```text
regras-basicas/
├── nucleo/
├── jogador/
├── mestre/
├── opositor/
└── registro/
```

### Núcleo

Regras comuns usadas por todos: testes, dificuldades, resultados, Defesas, Resistências, alcance, dano, Vida, Mana e outras mecânicas universais.

### Jogador

Regras necessárias para usar a própria ficha, Perícias, Poderes, recursos e opções durante a sessão.

### Mestre

Regras de julgamento: decidir quando testar, estabelecer dificuldades, interpretar circunstâncias e aplicar consequências.

O Mestre não controla o Opositor.

### Opositor

Regras para decidir e executar as ações voluntárias de adversários e forças contrárias ao Jogador.

### Registro

Regras sobre o que precisa permanecer verdadeiro: ficha, recursos atuais, condições, relações, conhecimento e estado da campanha.

## Roteamento simples

```text
É uma regra comum a todos?
→ Núcleo

É uma escolha ou uso da personagem do jogador?
→ Jogador

É julgamento ou aplicação imparcial da regra?
→ Mestre

É decisão de um adversário?
→ Opositor

Precisa continuar verdadeiro depois da resolução?
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

Enquanto a reformulação estiver em andamento, os arquivos desta pasta não substituem automaticamente `sistema/resolucao/`, `sistema/personagem/`, `sistema/operacao/` ou outras regras aprovadas.

## Direção

A meta é reduzir consultas durante a sessão e colocar na ficha os valores finais que o jogador realmente usa.

> Complexidade na construção; simplicidade na mesa.
