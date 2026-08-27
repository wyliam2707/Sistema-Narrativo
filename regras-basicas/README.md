# Regras Básicas

Status: REFORMULAÇÃO / NÃO IMPLEMENTADO

Esta pasta existe para reconstruir e simplificar as regras fundamentais do Sistema Narrativo sem alterar automaticamente as regras aprovadas atuais.

## Regra de localização

`regras-basicas/` contém somente **regras, procedimentos e modelos de funcionamento**.

Nenhum estado vivo de uma campanha deve ser armazenado aqui.

```text
regras-basicas/
→ como o sistema funciona
→ regras de resolução
→ autoridade das personas
→ procedimentos
→ modelos de registro

campanhas/<nome>/
→ o que é verdade naquela campanha
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

Exemplo:

```text
regras-basicas/opositor/registro-reservado.md
→ explica COMO funciona o registro adversarial.

campanhas/<nome>/opositor/...
→ guarda os planos adversariais REAIS daquela campanha.
```

> **Regra fica em `regras-basicas/`. Verdade da mesa fica em `campanhas/<nome>/`.**

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

Arquivos desta pasta podem definir modelos de registro do Opositor, mas os planos e prazos reais pertencem à campanha correspondente.

### Registro

Regras sobre o que precisa permanecer verdadeiro: ficha, recursos atuais, condições, relações, conhecimento e estado da campanha.

Os dados efetivamente preservados por essas regras ficam dentro de `campanhas/<nome>/`.

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
→ aplicar a regra de Registro
→ salvar em campanhas/<nome>/
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
