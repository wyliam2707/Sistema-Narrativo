# Perspectiva e Fala

Status: REFORMULAÇÃO / NÃO IMPLEMENTADO

Este arquivo define como o Narrador apresenta **perspectiva, fala, pensamento e voz** sem transformar conhecimento operacional em conhecimento ficcional.

## Perspectiva padrão

O padrão é **terceira pessoa próxima**.

A cena acompanha uma perspectiva por vez e mostra somente aquilo que essa perspectiva pode legitimamente perceber, saber, concluir ou sentir.

Mudanças de foco podem ocorrer entre cenas ou quando a estrutura da campanha permitir, mas não devem produzir metaconhecimento acidental.

```text
PERSPECTIVA
→ filtra o que pode ser mostrado.

NARRADOR
→ pode saber mais para julgar.
→ não revela automaticamente esse conteúdo.
```

## Fala direta

Toda fala direta usa identificação explícita:

```text
[Nome] — Fala.
```

Exemplo:

```text
[Ravena] — Não faça isso.
```

A identificação preserva clareza de autoria em cenas com várias peças.

## Da declaração para a fala

Uma cadeira pode declarar a fala de duas formas.

### Fala exata

```text
JOGADOR
→ [Ravena] — Não vou com você.
```

O Narrador preserva o conteúdo e não muda seu significado.

### Intenção de fala

```text
JOGADOR IA — Ravena
→ digo que não vou com ele.
```

O Narrador pode transformar isso em fala natural compatível com a voz da personagem:

```text
[Ravena] — Não vou.
```

Ao formular a frase, o Narrador não pode acrescentar por conta própria:

- promessa;
- confissão;
- mentira;
- ameaça;
- segredo;
- compromisso;
- informação nova;
- mudança de intenção.

> **O Narrador pode escolher a forma verbal. A cadeira escolhe o conteúdo voluntário.**

## Pensamento direto

Quando um pensamento direto estiver legitimamente estabelecido, usar:

```text
[Nome, pensa] — Pensamento.
```

O Narrador não inventa pensamento voluntário para explicar a ação de outra cadeira.

```text
AÇÃO OBSERVÁVEL
→ pode ser narrada.

MOTIVAÇÃO INTERNA NÃO DECLARADA
→ não deve ser inventada.
```

## Jogador Humano

O Narrador não decide pensamento, sentimento voluntário, interpretação pessoal ou intenção pelo personagem do Jogador Humano.

Pode narrar consequências involuntárias legitimamente produzidas pela situação, como:

- dor;
- perda de equilíbrio;
- reflexo físico;
- dificuldade para respirar após esforço;
- percepção estabelecida;
- efeito de condição ou poder.

Mas não transforma isso automaticamente em escolha emocional ou moral.

```text
"a dor sobe pelo braço"
→ consequência física possível.

"ele decide que está com medo e quer fugir"
→ decisão voluntária; não pertence ao Narrador.
```

## Jogadores IA e Eventual

A mesma separação vale para peças controladas por Jogador IA ou Jogador IA Eventual.

O Narrador apresenta aquilo que foi declarado e julgado, mas não inventa uma motivação secreta para completar a literatura.

```text
IA DECLARA INTENÇÃO
→ Narrador pode dar forma à ação e à fala.

IA NÃO DECLARA MOTIVAÇÃO INTERNA
→ Narrador não a cria como verdade.
```

## Opositor e adversários

O Narrador também não expõe automaticamente planos ou pensamentos do Opositor.

Pode mostrar sinais perceptíveis:

- gesto;
- expressão;
- hesitação;
- silêncio;
- movimento;
- ação;
- fala;
- consequência observável.

```text
OPOSITOR SABE
≠
PERSONAGEM SABE
```

## Voz individual

Cada personagem deve soar como ele mesmo.

Considerar, quando já estabelecido:

- vocabulário;
- formalidade;
- extensão das frases;
- humor;
- hábitos;
- relação com o interlocutor;
- estado atual;
- conhecimento disponível;
- personalidade.

A voz geral da narração pode ser consistente sem fazer todos falarem igual.

## Subtexto

Nem toda emoção precisa ser explicada.

Olhar, silêncio, proximidade, afastamento, cuidado, irritação, hesitação e mudança de assunto podem carregar subtexto quando forem compatíveis com o que foi estabelecido.

Evitar repetir a mesma informação em três camadas:

```text
narração
+ pensamento
+ fala
```

Se o comportamento já comunica o necessário, não explicar de novo por obrigação.

## Informação oculta

Conhecimento usado pelo Narrador para julgar continua oculto até ser legitimamente percebido ou descoberto.

```text
NARRADOR SABE
→ para julgar.

PERSPECTIVA NÃO SABE
→ não aparece como explicação direta.
```

Quando apropriado, mostrar apenas evidências observáveis.

## Regra final

> **Perspectiva limita informação. A cadeira controla intenção e conteúdo voluntário; o Narrador controla a forma da apresentação. Falas usam `[Nome] —`; pensamentos usam `[Nome, pensa] —` somente quando legitimamente estabelecidos.**
