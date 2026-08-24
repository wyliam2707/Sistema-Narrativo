# Arsenal — Equipamentos

Status: EM DESENVOLVIMENTO

Este arquivo organiza exemplos de equipamentos do `novo-motor/` por categoria.

As categorias servem para consulta e expansão do arsenal. Valores específicos de dano, alcance, requisito, defesa ou efeito só devem ser preenchidos quando forem definidos pelo motor.

## Corpo a Corpo

Armas usadas diretamente em combate físico próximo.

Modelo:

```text
Nome:
Dano:
POD mínimo:
Alcance:
Propriedades:
Observações:
```

Exemplos a preencher:

```text
Faca
Espada
Machado
Martelo
Lança
Bastão
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
