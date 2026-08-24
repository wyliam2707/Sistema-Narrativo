# Arsenal — Equipamentos

Status: EM DESENVOLVIMENTO

Este arquivo organiza exemplos de equipamentos do `novo-motor/` por categoria.

As categorias servem para consulta e expansão do arsenal. Valores específicos de outras categorias só devem ser preenchidos quando forem definidos pelo motor.

## Corpo a Corpo

Armas e formas de ataque usadas diretamente em combate físico próximo.

Formato:

```text
Nome - Alcance - Dano - Crítico - Tipo - Pegada
```

Campos:

```text
Nome     → arma ou forma de ataque.
Alcance  → Toque ou, quando possível, também Arremesso.
Dano     → dano base da arma; armas corporais somam POD quando indicado.
Crítico  → faixa de ameaça e multiplicador.
Tipo     → natureza principal do dano.
Pegada   → 1 mão ou 2 mãos. Ataques desarmados usam —.
```

Exemplos:

```text
Arte Marcial - Toque - 1d6 + POD - 20 x2 - Contusão - —
Faca - Toque / Arremesso - 1d4 + POD - 19-20 x2 - Perfuração - 1 mão
Bastão - Toque - 1d6 + POD - 20 x2 - Contusão - 1 mão
Espada - Toque - 1d8 + POD - 19-20 x2 - Corte - 1 mão
Machado - Toque - 1d10 + POD - 20 x3 - Corte - 2 mãos
Martelo - Toque - 1d10 + POD - 20 x3 - Contusão - 2 mãos
Lança - Toque / Arremesso - 1d8 + POD - 20 x3 - Perfuração - 2 mãos
```

## Disparo

Armas que possuem potência própria e atacam à distância.

Modelo:

```text
Nome:
Dano:
POD mínimo:
Alcance:
Propriedades:
Observações:
```

Quando houver requisito de POD e o usuário estiver abaixo dele, aplica-se a regra de penalidade definida pelo motor de resolução.

Exemplos a preencher:

```text
Pistola
Revólver
Rifle
Escopeta
Arco
Besta
```

## Magia

Focos, armas ou instrumentos usados para canalizar ataques e efeitos mágicos.

Modelo:

```text
Nome:
Dano ou efeito base:
POD mínimo:
Alcance:
Propriedades:
Observações:
```

O uso de magia pode envolver `HAB Mente` para aplicação/acerto e `POD Mente` para potência, conforme a regra específica do efeito.

Exemplos a preencher:

```text
Cajado
Varinha
Orbe
Grimório
Amuleto
Foco arcano
```

## Itens

Equipamentos que não pertencem diretamente às categorias de ataque anteriores.

Modelo:

```text
Nome:
Tipo:
Efeito:
Requisito:
Uso:
Observações:
```

Exemplos a preencher:

```text
Armadura
Escudo
Kit médico
Ferramentas
Comunicador
Lanterna
Poção
Dispositivo tecnológico
```

> **O Arsenal registra equipamentos. As regras gerais de resolução permanecem nos arquivos do motor.**
