# Arsenal

Status: EM DESENVOLVIMENTO

Esta pasta reúne exemplos de equipamentos usados pelo `novo-motor/`.

Ela pertence exclusivamente ao desenvolvimento experimental em `novo-motor/` e não altera o sistema canônico em `sistema/`.

## Objetivo

Registrar equipamentos prontos para consulta rápida durante criação, combate e resolução.

Categorias iniciais:

```text
Armas
Armaduras
Itens
```

## Princípio

Cada equipamento deve trazer apenas as informações necessárias para ser usado no jogo.

Sempre que possível, sua descrição deve ser autocontida e evitar exigir consulta a vários arquivos para entender seu funcionamento.

## Armas

Exemplos futuros podem registrar informações como:

```text
Nome
Tipo
Dano
Alcance
POD mínimo, quando houver
Propriedades especiais
```

Armas cujo dano depende diretamente da potência do usuário podem acrescentar `POD Corpo` ou `POD Mente`, conforme sua natureza.

Armas com potência própria, como armas de fogo, podem possuir Dano próprio e usar POD apenas como requisito de manejo quando a regra específica assim determinar.

## Armaduras

Exemplos futuros podem registrar informações como:

```text
Nome
Tipo
Defesa ou bônus aplicável
RD, quando houver
POD mínimo, quando houver
Propriedades especiais
```

A fórmula e o funcionamento definitivo das armaduras ainda dependem do desenvolvimento do motor de resolução.

## Itens

Itens incluem equipamentos relevantes que não sejam tratados principalmente como arma ou armadura.

Exemplos futuros podem registrar:

```text
Nome
Tipo
Uso
Efeito
Limitações
Cargas ou custo, quando houver
```

## Regra de desenvolvimento

Esta pasta contém exemplos e referências de equipamento.

Ela não deve criar silenciosamente novas regras gerais. Quando um equipamento depender de uma regra ainda não definida, o campo deve permanecer pendente até que o motor correspondente seja decidido.

> **O Arsenal mostra como um equipamento funciona. As regras gerais continuam pertencendo ao motor de resolução.**
