# Criação de Campanha

Status: REFORMULAÇÃO / NÃO IMPLEMENTADO

Este arquivo define o mínimo necessário para criar uma campanha jogável usando `regras-basicas/`.

> **Criar apenas o que precisa existir antes da primeira cena. O restante pode surgir depois, quando se tornar relevante.**

## Estrutura mínima

Criar:

```text
campanhas/<nome>/
├── README.md
├── personagens/
└── estado/
    └── atual.md
```

Outras áreas podem existir quando forem necessárias:

```text
mundo/
mestre/
opositor/
livro/
```

Não criar arquivos vazios apenas para completar uma estrutura ideal.

## Fluxo de criação

Trabalhar em etapas curtas:

```text
1. nome e proposta da campanha
2. direção narrativa e cenário suficiente
3. personagens iniciais com agência
4. fichas necessárias
5. situação inicial
6. conferir se já é possível jogar
7. iniciar
```

Perguntar somente o que ainda fizer diferença real e não pedir novamente informação já fornecida.

## Personagens iniciais

Registrar as personagens que precisam existir desde o começo.

Cada ficha segue `jogador/1.0-descricao-da-ficha.md` e recebe, no mínimo:

```text
Nome
Estado da Ficha
Importância
CONTROLE
Conceito
capacidades necessárias para o início
```

Personagens centrais ou recorrentes podem receber mais detalhes quando isso ajudar interpretação e decisão.

NPCs menores não precisam de ficha completa.

Campos ainda irrelevantes podem permanecer ausentes.

## Mecânica da ficha

Atributos, Perícias, Poderes e recursos seguem as regras de `jogador/`.

A ficha só precisa conter valores que já tenham sido legitimamente estabelecidos.

```text
CAMPO AUSENTE
→ ainda não foi necessário estabelecer

VALOR 0
→ zero foi realmente estabelecido
```

Se algo omitido se tornar necessário durante a campanha, estabelecer de forma coerente com conceito e fatos anteriores, nunca retroativamente para favorecer ou impedir uma ação já declarada.

## Estado inicial

`estado/atual.md` deve registrar apenas o presente necessário para abrir a primeira cena.

Quando relevante:

```text
local
momento ou período
personagens presentes
situação imediata
Vida/Mente/Mana atuais
condições ou efeitos ativos
processos ou prazos que já estejam correndo
```

Não escrever histórico longo no Estado Atual.

## README da campanha

O `README.md` da campanha funciona como porta de entrada.

Deve indicar pelo menos:

```text
Nome da campanha
CRIAÇÃO: EM ANDAMENTO ou CONCLUÍDA
personagem do JOGADOR HUMANO
personagens com JOGADOR IA, quando houver
se JOGADOR IA EVENTUAL e OPOSITOR são necessários
onde está o Estado Atual
```

Durante a criação, pode registrar uma linha curta de retomada:

```text
Etapa atual: ...
```

## Quando a campanha está pronta

A criação pode terminar quando já for possível responder com segurança:

```text
quem é o protagonista humano?
quem mais possui agência no início?
quem controla cada peça?
qual é a situação inicial?
o Narrador consegue apresentar a primeira cena sem inventar uma decisão essencial do jogador?
```

Se sim:

```text
CRIAÇÃO: CONCLUÍDA
→ seguir INICIO-E-RETOMADA.md
→ primeira cena
```

Não exigir que todo o mundo, todos os NPCs, todos os antagonistas ou toda a história futura estejam definidos antes de começar.

## Criação emergente depois do início

Lacunas futuras podem ser completadas durante a campanha conforme `nucleo/1.7-criacao-emergente.md`.

O que surgir como verdade da campanha é salvo pela regra de Registro na fonte apropriada.

## Regra final

> **Uma campanha está pronta quando possui peças suficientes, autoridades claras e uma situação inicial concreta. Construa o bastante para começar; deixe o mundo crescer durante o jogo sem preencher antecipadamente o que ainda não importa.**
