# Simplificação da Resolução

Status: RASCUNHO / NÃO IMPLEMENTADO

Este documento registra possibilidades discutidas para reduzir a complexidade cognitiva e a fragmentação do sistema sem descartar o núcleo atual de resolução.

## Diagnóstico inicial

O núcleo matemático atual é relativamente simples:

```text
resultado evidente
→ estabelece

impossibilidade evidente
→ estabelece

incerteza real
→ resolve
```

Quando existe teste:

```text
4d6 + Atributo
```

Perícia relevante concede dado adicional conforme a regra vigente.

Contra cenário usa-se Dificuldade. Contra oposição ativa usa-se oposição ou valor fixo quando uma regra específica determinar.

O principal problema percebido não é a matemática em si, mas a **fragmentação operacional**: uma única ação pode exigir consulta a vários módulos diferentes para saber ordem, resolução, Poder, Mana, Defesa, Resistência, Status e persistência.

## Direção de simplificação

A meta exploratória é:

> **manter a modularidade na criação, mas reduzir drasticamente a modularidade durante o uso em mesa.**

O jogador deve conseguir tomar a maior parte das decisões usando somente a própria ficha física.

## Poderes: construção antes da sessão

Possibilidade principal:

- usar tabelas modulares durante criação e evolução do personagem;
- montar um Poder combinando efeito, potência, alcance, alvo, duração e limitações;
- calcular o custo permanente do Poder pela configuração máxima comprada;
- registrar o Poder finalizado na ficha;
- não abrir novamente a tabela de construção durante a sessão.

Fluxo proposto:

```text
CRIAÇÃO / EVOLUÇÃO
→ tabela modular
→ monta Poder
→ calcula custo
→ grava Poder pronto na ficha

JOGO
→ consulta ficha
→ escolhe Poder
→ escolhe apenas opções que já estejam previstas nele
→ paga Mana
→ resolve
```

## Poderes escaláveis

Alguns Poderes podem possuir uma faixa de potência já comprada.

Exemplo conceitual:

```text
Golpe — Potência [2–4]
Alcance: corpo a corpo
Alvo: 1
Dano: 2d8 a 4d8 + atributo apropriado
Mana: 2 a 4
```

O custo de criação é calculado pela potência máxima, neste caso `4`.

Durante o jogo, o jogador pode escolher uma potência menor dentro da faixa e pagar menos Mana.

Exemplo:

```text
2d8 → 2 Mana
3d8 → 3 Mana
4d8 → 4 Mana
```

Assim o personagem compra a capacidade máxima, mas não é obrigado a usar sempre a intensidade máxima.

## Poderes fixos

Poderes que não precisam de escala podem ser escritos diretamente como efeitos fechados.

Exemplos conceituais:

### Teleporte

Move o usuário para um lugar conhecido ou para um destino identificável por um vínculo pessoal pertencente ao próprio usuário.

A ficha deve registrar diretamente suas condições e seu custo, sem exigir reconstrução de Alcance, Modo, Distância ou outras dimensões no momento do uso.

### Raio de Energia

```text
Alcance: Médio
Alvo: 1
Dano: 2d8 + INT
Custo de Mana: definido na ficha
```

### Armadura Arcana

```text
Alcance: Toque
Alvo: 1
Duração: 1 hora
Efeito: RD [2]
Custo de Mana: definido na ficha
```

Esses exemplos não são regras aprovadas; servem apenas para testar o formato.

## Pontos de Poder

Possibilidade a estudar:

O personagem recebe uma quantidade de **Pontos de Poder** durante a criação/evolução.

Esses pontos compram permanentemente as capacidades da ficha.

```text
Pontos de Poder
→ custo de possuir a capacidade

Mana
→ custo de usar a capacidade durante a aventura
```

Para Poderes escaláveis, os Pontos de Poder são calculados pelo maior efeito disponível.

## Ficha física como interface principal

Princípio de design em estudo:

> **Se uma escolha acontece frequentemente durante o jogo, ela deve estar visível na ficha. Se acontece apenas durante a criação, pode permanecer no livro/tabela de construção.**

A ficha de um Poder deve tentar concentrar:

```text
Nome
Potência ou faixa, quando existir
Mana
Alcance
Alvo
Duração
Efeito
```

O jogador não deveria precisar consultar uma tabela de construção para usar um Poder que já possui.

## Possível simplificação do fluxo de mesa

Uma direção desejada seria aproximar a experiência do jogador de algo como:

```text
1. declarar intenção
2. verificar se é evidente, impossível ou incerta
3. se incerta, fazer o teste apropriado
4. em combate, comparar com a Defesa aplicável
5. se acertar, aplicar exatamente o efeito escrito na ficha
```

O objetivo não é necessariamente remover profundidade, mas deslocar a complexidade para os momentos em que ela é útil: criação, evolução e preparação.

## Pontos ainda em aberto

Antes de implementar qualquer mudança, ainda é necessário estudar:

- custo em Pontos de Poder de cada tipo de efeito;
- relação entre potência máxima e custo de Mana;
- quais efeitos devem ser escaláveis e quais devem ser fixos;
- se DF/RF/DM/RM continuam separados ou podem ser simplificados;
- se tipos de Defesa Absoluta/Total/Parcial/Nula continuam necessários;
- se Resistência de Efeito deve existir separada da Defesa em todos os casos;
- ordem final de RD, Escudo, Trama e Vida;
- quanto da documentação atual deve virar regra central e quanto deve virar apenas orientação/exemplo;
- formato final da ficha física.

## Regra deste rascunho

> **Nenhuma ideia registrada aqui altera o sistema vigente até ser explicitamente aprovada e migrada para os módulos oficiais.**
