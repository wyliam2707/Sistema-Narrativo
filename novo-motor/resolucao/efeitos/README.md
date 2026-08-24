# Efeitos

Status: APROVADO

Esta pasta reúne os efeitos centrais do sistema em páginas de consulta operacional.

Cada página deve permitir resolver seu próprio efeito sem exigir retorno a este índice para a mecânica principal.

Estrutura preferida:

```text
o que o efeito faz
→ manifestação-base
→ resolução
→ escala ou resultado
→ regra exclusiva, se existir
→ persistência / encerramento, quando aplicável
```

Regras compartilhadas podem ser repetidas intencionalmente dentro das páginas para reduzir saltos de consulta durante a narração. Este README permanece como índice e referência de consistência.

## Resolução comum

Quando uma página não possuir fórmula própria e houver incerteza real:

`Efeito efetivo = patamar do efeito usado + 1 + (Perícia aplicável × 0,2)`

Sem Perícia aplicável:

`Efeito efetivo = patamar do efeito usado + 1`

Quando outra personagem estiver resistindo ativamente:

`Resistência ativa = Base da oposição + (Suporte da oposição × 0,2)`

Sem Suporte aplicável, usa-se apenas a Base da oposição. Resistências passivas, estruturas, proteções ou outros mecanismos usam o valor que realmente responde à ação.

`Resultado = 2^(Efeito efetivo − Resistência efetiva)`

Quando houver escala própria, ler o maior degrau que o Resultado alcançar. Regras específicas do efeito prevalecem sobre esta estrutura comum.

## Estrutura comum dos efeitos persistentes

Quando um efeito permanece na cena e não possui exceção própria:

`D = patamar do efeito usado + (Perícia aplicável × 0,2)`

`V = maior entre [1] e o Atributo estrutural da Fonte`

O Atributo estrutural vem da natureza real da Fonte e `V` fica fixado na criação da instância.

Enquanto `V > 0`, o efeito funciona integralmente. Dano estrutural não reduz sua intensidade por si só.

O efeito termina quando sua Duração termina ou quando chega a `V0`, o que acontecer primeiro. Em `V0`, aquela instância deixa de existir e não retorna apenas porque ainda restaria Duração.

Vida estrutural não é recuperada por Cura, descanso ou regeneração de VIDA comum.

## Aplicações iguais no mesmo alvo

Quando a página do efeito não possuir exceção própria, o mesmo efeito persistente aplicado novamente ao mesmo alvo consolida uma única instância.

Mesma Duração:

`D consolidada = maior D`

`V consolidada = maior V atual`

Durações diferentes:

`D consolidada = média das duas D`

`V consolidada = média das duas V atuais`

`Duração consolidada = maior Duração`

As médias mantêm decimais.

Da terceira aplicação em diante, comparar a nova aplicação com o estado consolidado atual. Se a instância atual já sofreu dano estrutural, usar sua Vida restante atual.

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

- `geral.md`
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

> **Durante o jogo, abra diretamente a página do efeito. O README existe para roteamento e consistência, não como etapa obrigatória da resolução.**