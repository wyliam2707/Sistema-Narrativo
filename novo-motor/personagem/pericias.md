# Perícias

Status: EM DESENVOLVIMENTO

Perícias representam áreas amplas de conhecimento, experiência, exploração e interação com o mundo.

Elas não representam, por si só, potência. O Atributo define a função usada na ação; a Perícia define o campo de treinamento ou conhecimento aplicado.

## Lista básica

### Comuns

```text
Esportes [X] | Exploração [X] | Expressão [X] | Sociedade [X]
Investigação [X] | Crime [X] | Ofícios [X] | Idiomas [X]
```

Perícias comuns podem ser tentadas sem treinamento quando a ação estiver dentro de conhecimento ou experiência cotidiana plausível.

### Somente treinadas

```text
Arcano [X] | Ocultismo [X] | Natureza [X] | Medicina [X]
Engenharia [X] | Ciência [X] | Tecnologia [X] | História [X]
```

Quando uma tarefa realmente depende de conhecimento especializado desses campos, é necessário treinamento correspondente.

## Uma ação pode aceitar Perícias diferentes

Não existe a regra `ação X = Perícia X`.

A situação apresenta um problema. A abordagem do personagem determina quais Perícias podem ser coerentes.

Exemplo:

```text
Seguir rastros

Exploração
→ acompanhar terreno, direção, deslocamento e sinais de passagem.

Investigação
→ analisar marcas, padrões, interrupções e inconsistências.

Natureza
→ interpretar vegetação, pegadas, comportamento animal e sinais naturais.
```

> **A ação define o problema. A abordagem define a Perícia aplicável.**

## Atributo e Perícia

O mesmo campo pode usar funções diferentes conforme a ação.

Exemplo:

```text
Esportes + POD Corpo
→ aplicar potência física com técnica.

Esportes + HAB Corpo
→ correr, saltar, nadar ou executar movimento técnico.

Esportes + RES Corpo
→ sustentar esforço prolongado.
```

A Perícia não fica presa permanentemente a um único Atributo.

## Escala atual

As Perícias usam escala de `[0]` a `[5]`.

```text
[0] → sem bônus de treinamento relevante.
[1] a [5] → graus crescentes de treinamento, domínio ou especialização.
```

O detalhamento qualitativo de cada grau ainda pode ser refinado durante o desenvolvimento.

O valor máximo atual é:

```text
Perícia máxima: [5]
```

## Áreas das Perícias

### Esportes
Atividade física treinada, condicionamento, corrida, salto, natação, escalada e práticas atléticas.

### Exploração
Orientação, viagem, navegação, leitura de terreno, sobrevivência prática e deslocamento por ambientes difíceis.

### Expressão
Música, atuação, dança, escrita, artes visuais, performance e outras formas de expressão.

### Sociedade
Costumes, instituições, leis, política, etiqueta, relações sociais e funcionamento de grupos e organizações.

### Investigação
Análise de evidências, pesquisa, reconstrução de acontecimentos, pistas e dedução aplicada.

### Crime
Submundo, segurança, contrabando, métodos criminosos, falsificação, redes ilegais e práticas relacionadas.

### Ofícios
Produção prática e trabalhos especializados, como carpintaria, cozinha, costura, ferraria e outros ofícios coerentes com a formação do personagem.

### Idiomas
Línguas, escrita, leitura, tradução e conhecimento linguístico.

### Arcano
Magia, feitiços, runas, encantamentos, itens mágicos, artefatos, alquimia e funcionamento de efeitos mágicos.

### Ocultismo
Demônios, espíritos, mortos-vivos, cultos, possessões, entidades ocultas, maldições e outros seres ou fenômenos sobrenaturais relacionados.

### Natureza
Animais, plantas, ecossistemas, clima, sinais naturais e conhecimento especializado do mundo natural.

### Medicina
Anatomia, doenças, diagnóstico, tratamento, primeiros socorros e procedimentos médicos.

### Engenharia
Estruturas, construção, mecanismos, fabricação, reparos e aplicação técnica de princípios de projeto.

### Ciência
Conhecimento científico, método científico, física, química, biologia, matemática e áreas relacionadas.

### Tecnologia
Computadores, eletrônica, sistemas tecnológicos, dispositivos e infraestrutura tecnológica.

### História
Povos, civilizações, acontecimentos históricos, guerras, linhagens, registros antigos, ruínas e arqueologia quando pertinente.

## Combate

A lista acima continua voltada a exploração, conhecimento e interação. Os bônus específicos usados em ataque, quando existirem, permanecem registrados no bloco de Ataques da ficha e no motor de combate.

As regras gerais de teste usam `1d20 + Atributo + Perícia aplicável`, conforme `../resolucao/resolucao-d20.md`.
