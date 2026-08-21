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
Mana/Energia:
Condições:
Efeitos Ativos:
Local:
```

Nem todo personagem precisa usar todos os campos. Um campo só é registrado quando fizer sentido para aquela entidade e para a situação atual.

## Vida

VIDA é um estado conceitual, nunca uma quantidade de pontos.

Escala:

```text
Ileso
Ferido
Grave
Crítico
Incapacitado
```

Os estados representam a condição física geral do personagem naquele momento.

Não existe obrigação de passar por todos em sequência. Um acontecimento pode alterar vários estados de uma vez quando a ficção e a resolução justificarem isso.

`Incapacitado` não significa `Morto`.

Incapacitado significa que o personagem não consegue continuar agindo normalmente por causa de seu estado físico. Pode estar desacordado, em choque, imobilizado ou simplesmente incapaz de continuar.

Morte é uma consequência distinta, definida pela ficção e pelas regras de resolução. Ela não é um sexto nível de VIDA.

## Mana / Energia

Mana ou Energia também é um estado conceitual, nunca uma reserva numérica de pontos.

Escala:

```text
Cheia
Média
Baixa
Crítica
```

Ela representa a condição atual da reserva de energia extraordinária disponível ao personagem.

`Crítica` significa que ainda existe energia disponível, mas a reserva está no limite. Isso não impede automaticamente o uso de uma capacidade.

As regras que determinam quando a reserva muda, quais ações exigem energia e quais consequências podem ocorrer em estado Crítico pertencem à resolução.

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

```text
STATUS:
Vida: Grave
Mana: Crítica
Condições:
- Envenenado
- Atordoado
Efeitos Ativos:
Local: Corredor Norte
```

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

```text
FICHA:
RES [2]
Regeneração [1]

STATUS:
Vida: Grave
Mana: Baixa
Local: Biblioteca
```

`RES [2]` e `Regeneração [1]` descrevem capacidades estáveis do personagem.

`Vida: Grave`, `Mana: Baixa` e `Local: Biblioteca` descrevem apenas seu estado atual.

Se uma mudança deixar de ser temporária e passar a alterar de forma estável quem o personagem é, ela deve ser tratada pela camada apropriada de persistência e, quando necessário, consolidada na ficha.

> **STATUS registra o presente. A ficha registra o personagem.**
