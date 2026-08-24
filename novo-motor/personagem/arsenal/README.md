# Arsenal

Status: EM DESENVOLVIMENTO

Esta pasta reúne exemplos de equipamentos usados pelo `novo-motor/`.

Ela pertence exclusivamente ao desenvolvimento experimental em `novo-motor/` e não altera o sistema canônico em `sistema/`.

## Objetivo

Registrar equipamentos prontos para consulta rápida durante criação, combate e resolução.

Estrutura atual:

```text
corpo-a-corpo.md → armas e ataques físicos próximos
disparo.md       → armas de projétil e energia
magia.md         → conjuração livre e focos mágicos
itens.md         → off-hand e armaduras
```

## Princípio

Cada equipamento deve trazer apenas as informações necessárias para ser usado no jogo.

Sempre que possível, sua descrição deve ser autocontida e evitar exigir consulta a vários arquivos para entender seu funcionamento.

Poucos perfis mecânicos podem representar muitas manifestações narrativas diferentes.

## Corpo a Corpo

Armas físicas próximas usam o formato:

```text
Nome - Alcance - Dano - Crítico - Tipo - Pegada
```

Quando `POD` aparece no dano dessas armas, significa `POD Corpo`.

Todo personagem possui automaticamente `Arte Marcial` como ataque corporal básico.

## Disparo

Armas de disparo usam o formato:

```text
Nome - Alcance - Dano - Crítico - Munição - Pegada - Época
```

A munição é abstrata. Não existe contagem de projéteis, carregadores ou tiros restantes.

Armas cuja potência vem do usuário, como arcos e fundas, podem somar `POD Corpo`. Armas com potência própria usam o dano indicado pela própria arma.

## Magia

Ataques e focos mágicos usam o formato:

```text
Nome - Alcance - Dano - Crítico - Tipo - Pegada
```

O acerto mágico usa `HAB Mente`; `POD Mente` entra na potência e no dano quando indicado.

`Conjurar Livre` representa o ataque mágico básico sem foco e sem ocupar as mãos.

## Itens Defensivos

Os perfis defensivos atuais são simples e especializados:

```text
Escudo → Esquiva +2
Foco Sensorial → Percepção +2
Armadura Leve → RD 2 | Falha mágica 1/6
Armadura Pesada [POD Corpo 2+] → RD 4 | Falha mágica 2/6
```

Itens de off-hand ocupam uma mão. Armaduras fornecem RD e podem interferir na conjuração.

## Regra de desenvolvimento

Esta pasta contém exemplos e referências de equipamento.

Ela não deve criar silenciosamente novas regras gerais. Quando um equipamento depender de uma regra ainda não definida, o campo deve permanecer pendente até que o motor correspondente seja decidido.

> **O Arsenal mostra como um equipamento funciona. As regras gerais continuam pertencendo ao motor de resolução.**
