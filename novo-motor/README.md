# Novo Motor

**Status: EM DESENVOLVIMENTO**

Esta pasta é o espaço experimental do novo motor. Ela permanece separada de `sistema/` até haver decisão explícita de migração.

## Arquitetura consolidada

A construção mecânica do personagem usa somente quatro blocos:

```text
ATRIBUTOS
+ PERÍCIAS
+ PODERES
+ PASSIVOS
↓
VALORES DERIVADOS
```

### Atributos

```text
Corpo — POD [ ] | HAB [ ] | RES [ ]
Mente — POD [ ] | HAB [ ] | RES [ ]
```

`POD` representa potência, `HAB` execução e controle, e `RES` resistência. Corpo e Mente definem a natureza da capacidade.

### Perícias

Perícias representam treinamento, conhecimento e experiência aplicáveis à situação. Elas não formam uma lista separada de ataques.

### Poderes

Poderes são efeitos ativos autocontidos. Cada Poder possui arquivo próprio em `personagem/poderes/`.

```text
Golpe [2]
Disparo [3]
Teleporte [5]
```

Nos Poderes ativos, `[X]` é o máximo de Energia que pode ser investido naquele Poder em um único uso.

O efeito-base pode custar `0`. Sempre que a intenção exigir uma ampliação acima de `0`, o narrador informa o custo e aguarda confirmação antes de gastar Energia.

Cada Poder define sua própria descrição, podendo usar POD, HAB, dados, valores fixos, alcance, alvo, área, duração e ampliações próprias. Não existe uma fórmula universal obrigatória para todos os Poderes.

### Passivos

Passivos são capacidades permanentes ou estáveis já incorporadas ao personagem. Cada Passivo possui arquivo próprio em `personagem/passivos/`.

```text
RD [3]
Vida Extra [30]
Proteção [2]
Sentido-Aranha
Imortalidade
Regeneração [2]
```

Nos Passivos, `[X]` não significa limite de Energia. O próprio arquivo do Passivo define o significado do valor.

### Valores Derivados

Depois dos quatro blocos, a ficha consolida os valores de consulta constante, como:

```text
Vida
Energia
Esquiva
Percepção
Vontade
Fortitude
RD
Deslocamento
```

Passivos que alteram esses valores já entram no total final mostrado na ficha.

## Sem camada mecânica de Arsenal

Armas, armaduras, escudos, focos, ferramentas de combate e manifestações semelhantes não formam uma camada mecânica separada.

A aparência pertence à ficção; a função pertence a Poderes e Passivos.

Exemplos:

```text
Golpe → soco, espada, garra, bastão.
Disparo → arco, pistola, batarang, raio.
RD → armadura, pele sobrenatural, traje tecnológico.
Proteção → escudo, reflexos, sentidos ampliados, campo defensivo.
```

Recursos narrativos relevantes, como uma base, veículo ou rede de contatos, podem continuar registrados na ficha sem formar inventário mecânico.

## Consulta sob demanda

Fluxo de Poder ativo:

```text
jogador declara que quer usar um Poder
→ listar os Poderes disponíveis
→ jogador escolhe um
→ abrir apenas o arquivo daquele Poder
→ mostrar efeito-base e ampliações
→ jogador declara a intenção
→ se couber no padrão, resolver
→ se exigir ampliação, informar o custo
→ jogador confirma
→ gastar Energia e resolver
```

> **O narrador nunca escolhe automaticamente uma ampliação que consuma Energia.**

## Regra de isolamento

1. tudo dentro de `novo-motor/` continua experimental;
2. não alterar `sistema/` por causa do novo motor sem decisão explícita;
3. regras antigas que contradigam esta arquitetura não têm precedência dentro do `novo-motor/`;
4. novos Poderes e Passivos devem ser registrados em arquivos próprios e autocontidos;
5. fórmulas ainda não fechadas de Valores Derivados ou resolução não devem ser inventadas para preencher lacunas.
