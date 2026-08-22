# STATUS

Status: APROVADO

STATUS registra **como o personagem está agora**.

Ele reúne estados atuais e mutáveis que ainda podem produzir consequência para continuidade ou resolução, sem alterar por si só quem o personagem é de forma permanente.

```text
FICHA
→ quem o personagem é

STATUS
→ como o personagem está neste momento
```

## Estrutura básica

```text
STATUS:
Vida:
Dano acumulado:
Energia:
Condições:
Efeitos Ativos:
Local:
```

Nem todo personagem precisa usar todos os campos. Um campo só é registrado quando fizer sentido para aquela entidade e para a situação atual.

## Vida

A referência estrutural comum é:

`1 grau de Vida = 5 pontos`

Um personagem completo usa `V35`, equivalente a sete graus, e a apresentação narrativa continua seguindo a régua:

`0–4 Ileso | 5–9 Ferido | 10–14 Ferido* | 15–19 Grave | 20–24 Grave* | 25–29 Crítico | 30–34 Crítico* | 35 Incapacitado`

Para personagens, o STATUS pode continuar mostrando a condição narrativa e o Dano acumulado em vez de tratar a ficha como uma barra abstrata de PV.

Exemplo: `Vida: Ferido* | Dano acumulado: 12`.

`Vida` comunica o estado físico atual do personagem.

`Dano acumulado` registra a posição matemática usada pela resolução para manter continuidade entre aplicações de dano. O valor `35` marca a referência de Incapacitado; não obriga a ficção a tratar toda sobrevivência como uma barra rígida.

Não existe obrigação de passar por todos os estados em sequência. Um acontecimento pode alterar vários estados de uma vez quando a ficção e a resolução justificarem isso.

A régua também não protege o personagem contra uma assimetria evidente. Quando a natureza e a intensidade de um efeito tornam sobrevivência incoerente, a consequência pode ultrapassar a progressão normal.

`Incapacitado` não significa `Morto`.

Incapacitado significa que o personagem não consegue continuar agindo normalmente por causa de seu estado físico. Pode estar desacordado, em choque, imobilizado ou simplesmente incapaz de continuar.

Morte é uma consequência distinta, definida pela ficção e pelas regras de resolução. Ela não é um nível adicional de VIDA.

## Energia

ENERGIA registra a Reserva atual do personagem e, quando existir, a carga disponível em uma Bateria.

A regra de cálculo, custos de uso, recuperação e transferência pertence a `../resolucao/energia.md`. O STATUS apenas preserva os valores já estabelecidos.

A Reserva pode ser lida em cinco estados narrativos:

`Cheia | Alta | Média | Baixa | Crítica | Esgotada`

Os cinco estados com Energia disponível dividem igualmente a Reserva máxima.

O valor numérico pode ser mostrado junto do estado para facilitar o controle.

A notação operacional padrão é mantida em uma única linha:

`Energia [10/100] - Bateria [40/40] - Descanso [45]-[45]`

`Energia [atual/máxima]` registra a Reserva própria.

`Bateria [atual/máxima]` registra a carga externa disponível.

`Descanso [X]-[Y]` registra quanto ainda pode ser recuperado em cada camada. O primeiro valor é a parcela de esforço recente recuperável por um fôlego de aproximadamente 5 minutos; o segundo é o desgaste profundo que exige aproximadamente 1 a 2 horas.

Depois do fôlego curto, sua parcela pode ficar em zero enquanto o desgaste profundo permanece. Exemplo: `Energia [55/100] - Bateria [40/40] - Descanso [0]-[45]`.

Quando o personagem não possui Bateria, esse trecho é omitido. Quando não existe recuperação pendente, o trecho de Descanso também pode ser omitido.

A Bateria é uma reserva separada. Sua presença, natureza e patamar pertencem à ficha; sua carga atual pertence ao STATUS.

Os estados comunicam rapidamente a condição da Reserva. Os números preservam a precisão necessária para gasto, recuperação e continuidade.

## Condições

Condição é um estado temporário que altera a situação do personagem sem mudar permanentemente quem ele é.

Exemplos:

```text
Atordoado
Envenenado
Exausto
Imobilizado
Sangrando
Cego
Amaldiçoado
Confuso
Queimando
```

Condições não possuem bônus ou penalidades numéricas automáticas.

Uma condição diz exatamente o que foi estabelecido pela ficção, e a resolução interpreta suas consequências quando ela for relevante.

Exemplo: `Cego` significa que o personagem não enxerga. Não significa automaticamente `-2` ou qualquer outro modificador universal.

Uma condição permanece enquanto sua causa ou seu efeito continuar existindo e sendo relevante. Quando deixa de existir ou de importar, ela sai do STATUS.

Nem toda descrição momentânea precisa virar condição. Registra-se apenas o que puder continuar relevante para ações ou cenas seguintes.

### Condição produzida por efeito persistente

Quando a condição é produzida por um **efeito persistente consolidado**, ela recebe estrutura própria:

`Condição [D x / V5] — Duração`

`D` é a Defesa estrutural do efeito, igual ao Efetivo que realmente o estabeleceu. `V5` é sua Vida padrão, equivalente a um grau.

Exemplo: `Cegueira [D2,4 / V5] — Cena`.

Enquanto houver Vida, a condição continua com o resultado que foi estabelecido. Perder Vida não reduz automaticamente o grau narrativo do efeito. Em `V0`, o efeito termina e sai do STATUS.

### Condição sustentada por agente

Uma condição causada diretamente por um personagem, criatura ou Invocação ativa que continua realizando a ação **não recebe D/V próprio apenas por estar registrada no STATUS**.

Ela é marcada como `Sustentada` e aponta para a fonte que precisa continuar agindo.

Exemplos: `Agarrado [2] — Sustentado pelo Guarda` | `Imobilizado [8] — Sustentado por 4 guardas`.

A manutenção consome a ação dos agentes que continuam sustentando a contenção. Se eles deixam de agir, são incapacitados ou perdem o mecanismo que mantém a condição, a situação é atualizada conforme a resolução.

O personagem contido continua escolhendo suas próprias ações dentro do que a posição permite: pode tentar escapar, atacar quem o segura, usar uma capacidade possível ou escolher outro mecanismo coerente.

> **Efeito persistente cria estrutura D/V. Agente ativo sustenta uma condição com a própria ação.**

## Efeitos Ativos

Efeito Ativo é uma capacidade, proteção, alteração ou fenômeno temporário que continua produzindo efeito sobre o personagem, objeto ou ambiente.

Exemplos:

```text
Proteção Mágica
Invisibilidade
Forma de Lobo
Barreira Mental
Runa de Proteção
Voo sustentado
Maldição ativa
Bênção ativa
```

Diferença principal:

```text
CONDIÇÃO
→ descreve como o personagem está

EFEITO ATIVO
→ descreve algo temporário que está agindo sobre ele ou sendo mantido por ele
```

Um Efeito Ativo não precisa ter duração numérica obrigatória. Ele permanece enquanto a ficção, sua fonte ou a resolução estabelecerem que permanece.

Evita-se duplicação. Se um Efeito Ativo já descreve adequadamente o estado temporário relevante, não é necessário registrar uma segunda Condição dizendo a mesma coisa.

Registra-se um Efeito Ativo apenas quando sua permanência puder alterar decisões ou resoluções futuras.

### Estrutura de efeitos persistentes

Todo efeito persistente consolidado, **benéfico ou prejudicial**, usa a mesma estrutura:

`Efeito [D x / V5] — Duração`

Exemplos: `Cegueira [D2,4 / V5] — Cena | Bênção [D3,0 / V5] — Cena`.

Efeitos instantâneos, como Cura já aplicada, não permanecem com `D/V` no STATUS.

`Dissipar` é um efeito separado que causa dano sobre a Vida desses STATUS persistentes. Ele usa o mesmo motor normal de ataque e defesa: `Dissipar efetivo vs D → Dano → reduz V`. Em `V0`, o efeito sai do STATUS.

### Proteção

Proteção/Barreira usa um grau de Vida:

`Proteção [D x / V5] — Duração`

Sua Defesa vem da regra própria da Proteção. Exemplo: `Proteção [D2,4 / V5] — Cena`.

Quando sua Vida chega a `0`, a Proteção é rompida e sai do STATUS.

### Invocação

Invocações possuem dois graus de Vida:

`Invocação [D = RES / V10]`

Quando uma Invocação é atacada diretamente, sua `RES` funciona como Defesa estrutural e o dano reduz `V10`.

Uma prisão mantida por Invocação registra a criação que sustenta a condição.

Exemplo: `Preso — Invocação [D4 / V10] — Cena`.

O `D4` indica que a criação possui `RES [4]` para resistir a ataques dirigidos contra sua estrutura. O mecanismo que mantém alguém preso pode envolver outro Atributo, como `FIS`, conforme a função da criação; isso não transforma RES em defesa universal para toda tentativa de fuga.

### Estrutura física aplicada

Uma estrutura física que continua prendendo alguém depois que seus agentes soltam é registrada como a própria fonte da contenção, não como um efeito mágico abstrato.

Exemplo: `Algemado — Algemas [FIS3 / V10]`.

`FIS [3]` descreve o mecanismo físico da contenção quando a tentativa é vencê-la corporalmente. `V10` registra a Vida estrutural do objeto. Outras formas de escapar ou destruir a estrutura usam o mecanismo e a defesa realmente aplicáveis.

## Referência de Vida estrutural

A régua comum fica:

`Efeito persistente → V5` | `Proteção/Barreira → V5` | `Invocação/estrutura equivalente → V10` | `Personagem → V35`

Vida e Defesa são dimensões distintas. A Defesa diz quão difícil é causar dano; a Vida diz quanto dano a estrutura suporta antes de acabar.

## Localização

Local registra onde o personagem está no momento, apenas no nível de detalhe necessário para continuidade e resolução.

Exemplos:

```text
Local: Biblioteca do Castelo
Local: Telhado da Torre Norte
Local: Floresta, próximo ao rio
Local: Nova York — apartamento de Wanda
```

A localização deve ser específica o bastante para evitar deslocamentos narrativos acidentais ou confusão de continuidade, mas não precisa repetir detalhes que já pertencem ao cenário.

Posição exata dentro de um local só precisa ser registrada quando ela continuar relevante para a ação.

## Atualização do STATUS

STATUS acompanha somente estados atuais que ainda produzem consequência.

Existem três operações básicas:

```text
ENTRA
→ quando um novo estado relevante é estabelecido pela ficção.

MUDA
→ quando esse estado se altera de forma relevante.

SAI
→ quando deixa de existir ou de importar para continuidade ou resolução.
```

Exemplo:

`STATUS: Vida: Grave | Dano acumulado: 18 | Energia [22/60] - Bateria [40/60] - Descanso [19]-[19] | Condições: Envenenado, Atordoado | Local: Corredor Norte`

Se uma Proteção Mágica terminou, ela simplesmente deixa de aparecer em Efeitos Ativos. Se Atordoado deixou de existir, sai de Condições.

STATUS não guarda histórico.

O que aconteceu permanece no Livro. Se um fato passado continua causalmente vivo, pertence à Progressão; se alterou de forma estável o personagem, pode ser consolidado na ficha.

## Atualização operacional imediata

Durante resolução ativa, o STATUS é atualizado assim que a consequência correspondente é estabelecida.

`Energia` muda no momento em que o custo é pago. `Vida` e `Dano acumulado` mudam quando Dano ou Cura são aplicados. Condições e Efeitos Ativos entram, mudam ou saem assim que sua resolução os estabelece.

O NARRADOR não espera o fim da cena ou do turno para corrigir valores que já mudaram.

A apresentação pode permanecer compacta em uma única linha, mostrando somente o que ainda importa naquele momento.

Exemplo: `STATUS → Vida: Grave | Dano acumulado: 18 | Energia [39/60] | Proteção [D2,4 / V5] — Cena | Cegueira [D2,8 / V5] — Cena`.

Se Dissipar causar 2 de Dano na Cegueira, a próxima apresentação já mostra: `Cegueira [D2,8 / V3] — Cena`.

Quando um valor ou efeito muda, a próxima apresentação do STATUS já usa o novo estado.

> **Resolveu, atualizou. O STATUS sempre representa o presente, não o estado do começo do turno.**

## Autoridade sobre o STATUS

STATUS registra fatos estabelecidos, nunca intenções, previsões ou consequências ainda não resolvidas.

```text
JOGADOR / JOGADOR IA
→ declara ações e decisões do personagem.

OPOSITOR
→ apresenta pressão, ameaça e oposição.
→ não altera diretamente o STATUS como consequência ainda não resolvida.

NARRADOR
→ determina, pela ficção e pelas regras de resolução, o resultado estabelecido.

PERSISTÊNCIA
→ registra no STATUS o resultado já estabelecido.
```

Ninguém altera o STATUS apenas porque declarou uma intenção.

Quando não existe disputa real, não é necessário criar uma resolução artificial. Se um personagem encerra voluntariamente um efeito que controla e nada impede isso, o fato já está estabelecido e o Efeito Ativo pode ser removido.

## Fronteira com a ficha

STATUS não substitui a ficha.

Exemplo: `FICHA: RES [2] | Regeneração [1] | Bateria [3]` | `STATUS: Vida: Grave | Dano acumulado: 18 | Energia [22/40] - Bateria [36/60] | Local: Biblioteca`.

`RES [2]`, `Regeneração [1]` e `Bateria [3]` descrevem capacidades estáveis do personagem. `Vida: Grave`, `Dano acumulado: 18`, `Energia [22/40]` e `Bateria [36/60]` descrevem apenas seu estado atual.

Se uma mudança deixar de ser temporária e passar a alterar de forma estável quem o personagem é, ela deve ser tratada pela camada apropriada de persistência e, quando necessário, consolidada na ficha.

> **STATUS registra o presente. A ficha registra o personagem.**
