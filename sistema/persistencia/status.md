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

VIDA continua sendo um estado conceitual. Ela não é uma reserva de pontos de vida.

Para manter a progressão entre consequências, a resolução pode registrar separadamente o **Dano acumulado** como memória matemática de bastidor.

A apresentação da VIDA segue esta régua:

`0–4 Ileso | 5–9 Ferido | 10–14 Ferido* | 15–19 Grave | 20–24 Grave* | 25–29 Crítico | 30–34 Crítico* | 35 Incapacitado`

Exemplo: `Vida: Ferido* | Dano acumulado: 12`.

`Vida` comunica o estado físico atual do personagem.

`Dano acumulado` registra apenas a posição matemática usada pela resolução para manter continuidade entre aplicações de dano. Ele não é tratado como pontos de vida, não mede saúde total e não substitui a interpretação da ficção.

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

`Energia [10/100] - Bateria [40/40] - Descanso [5m:+45 / 2h:+45]`

`Energia [atual/máxima]` registra a Reserva própria.

`Bateria [atual/máxima]` registra a carga externa disponível.

`Descanso [5m:X / 2h:Y]` registra quanto ainda pode ser recuperado em cada janela de descanso. O primeiro valor é a parcela de esforço recente recuperável por um fôlego de aproximadamente 5 minutos; o segundo é o desgaste profundo que exige aproximadamente 1 a 2 horas.

Depois do fôlego curto, sua parcela pode ficar em zero enquanto o desgaste profundo permanece. Exemplo: `Energia [55/100] - Bateria [40/40] - Descanso [5m:+0 / 2h:+45]`.

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

Exemplo:

```text
Cego
```

significa que o personagem não enxerga. Não significa automaticamente `-2` ou qualquer outro modificador universal.

Uma condição permanece enquanto sua causa ou seu efeito continuar existindo e sendo relevante. Quando deixa de existir ou de importar, ela sai do STATUS.

Nem toda descrição momentânea precisa virar condição. Registra-se apenas o que puder continuar relevante para ações ou cenas seguintes.

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

`STATUS: Vida: Grave | Dano acumulado: 18 | Energia [22/60] - Bateria [40/60] - Descanso [5m:+19 / 2h:+19] | Condições: Envenenado, Atordoado | Local: Corredor Norte`

Se uma Proteção Mágica terminou, ela simplesmente deixa de aparecer em Efeitos Ativos. Se Atordoado deixou de existir, sai de Condições.

STATUS não guarda histórico.

O que aconteceu permanece no Livro. Se um fato passado continua causalmente vivo, pertence à Progressão; se alterou de forma estável o personagem, pode ser consolidado na ficha.

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

Exemplo:

`FICHA: RES [2] | Regeneração [1] | Bateria [3]`

`STATUS: Vida: Grave | Dano acumulado: 18 | Energia [22/40] - Bateria [36/60] | Local: Biblioteca`

`RES [2]`, `Regeneração [1]` e `Bateria [3]` descrevem capacidades estáveis do personagem.

`Vida: Grave`, `Dano acumulado: 18`, `Energia [22/40]` e `Bateria [36/60]` descrevem apenas seu estado atual.

Se uma mudança deixar de ser temporária e passar a alterar de forma estável quem o personagem é, ela deve ser tratada pela camada apropriada de persistência e, quando necessário, consolidada na ficha.

> **STATUS registra o presente. A ficha registra o personagem.**
