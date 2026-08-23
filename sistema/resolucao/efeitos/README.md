# Efeitos

Status: APROVADO

Esta pasta reúne os efeitos centrais do sistema em páginas curtas de consulta.

Cada página responde somente a quatro perguntas:

```text
o que o efeito faz
→ manifestação-base
→ escala ou resultado
→ regra exclusiva, se existir
```

Regras compartilhadas não são repetidas em cada efeito.

## Estrutura comum dos efeitos persistentes

Quando um efeito permanece na cena e não possui exceção própria:

`D = nível do efeito usado + (Perícia aplicável × 0,2)`

`V = maior entre [1] e o Atributo estrutural da Fonte`

A Fonte e a Vida estrutural pertencem a `../fonte-e-vida-estrutural.md`.

Enquanto `V > 0`, o efeito funciona integralmente. Dano estrutural não reduz sua intensidade por si só.

O efeito termina quando sua Duração termina ou quando chega a `V0`, o que acontecer primeiro. Em `V0`, aquela instância deixa de existir e não retorna apenas porque ainda restaria Duração.

Vida estrutural não é recuperada por Cura, descanso ou regeneração de VIDA comum.

## Aplicações iguais no mesmo alvo

O mesmo efeito persistente aplicado novamente ao mesmo alvo consolida uma única instância.

Mesma Duração:

`D consolidada = maior D`

`V consolidada = maior V atual`

Durações diferentes:

`D consolidada = média das duas D`

`V consolidada = média das duas V atuais`

`Duração consolidada = maior Duração`

As médias mantêm decimais.

Da terceira aplicação em diante, comparar a nova aplicação com o **estado consolidado atual**, não com uma média histórica das aplicações originais. Se a instância atual já sofreu dano estrutural, usar sua Vida restante atual.

Se a instância anterior já chegou a `V0`, uma nova aplicação cria uma nova instância completa.

Efeitos diferentes não se fundem.

## Escala-base

Quando uma página usar a escala geral:

`[2] inicial forte` | `[4] relevante` | `[8] completo` | `[16] profundo/amplo` | `[32] absoluto`

Os nomes concretos pertencem a cada efeito.

## Manifestação e Ampliação

Cada efeito registra sua manifestação-base no formato:

`Alcance / Alvos / Área ou Tamanho / Duração`

Alterações acima da base usam `../consolidacao.md`.

Ampliação muda escala de manifestação; não amplia repertório.

## Índice

- `dano.md`
- `cura.md`
- `dissipar.md`
- `sentidos.md`
- `controle.md`
- `mobilidade.md`
- `supressao.md`
- `protecao.md`
- `informacao.md`
- `invocacao.md`
- `transformacao.md`
- `sono.md`
- `ilusao.md`
- `emocao.md`
- `deslocar.md`

> **Consulte a página do efeito; consulte as regras gerais somente quando elas realmente forem necessárias.**
