# Julgamento

Status: REFORMULAÇÃO / NÃO IMPLEMENTADO

Este arquivo orienta o `NARRADOR` a transformar intenções, estado e oposição em uma sentença já estabelecida.

A regra mecânica de referência é `../nucleo/0.1-resolucao.md`.

> **Julgar é descobrir o que realmente acontece. Não é escolher o resultado mais conveniente.**

## Entrada

O Narrador julga quando possui informação suficiente sobre as intenções relevantes daquele momento.

Não é necessário exigir uma nova declaração formal de toda cadeira a cada pequena passagem de tempo.

```text
INTENÇÃO PERSISTENTE CLARA
→ continua válida.

CADEIRA IA TEM MOTIVO PARA NOVA DECISÃO
→ executá-la dentro de seu próprio escopo.

NOVA DECISÃO HUMANA É NECESSÁRIA
→ parar antes de julgar além desse ponto.
→ devolver controle ao jogador.
```

## 1 — Separar intenção de pressuposto

Toda declaração informa aquilo que a própria peça pretende fazer.

```text
"abro a porta"
→ intenção de abrir.

"vou ao quarto e beijo Ravena"
→ intenção de ir ao quarto e tentar o beijo se houver oportunidade.
```

A declaração não estabelece por si:

- que outra personagem está onde o jogador presume;
- que permaneceu esperando;
- que percebeu algo;
- que aceita aproximação;
- que reage de determinada forma;
- que uma ação já teve sucesso.

Antes de resolver, conferir o estado real da campanha.

> **Pressuposto da declaração não vira fato sobre outra peça.**

Também não criar retroativamente uma ação alheia apenas porque agora conhece a declaração humana.

## 2 — Preservar decisões independentes

Cada Jogador IA e peça adversarial decide com seu próprio conhecimento antes que o Narrador use informações ocultas para julgar.

```text
PERSONAGEM DECIDE
→ com o que sabe, quer, sente e pode fazer.

NARRADOR JULGA
→ com o conjunto da realidade necessária.
```

Não corrigir uma decisão porque uma capacidade alheia escondida a tornaria ruim.

Exemplo:

```text
personagem decide mentir
→ não sabe que o alvo detecta mentiras
→ manter a mentira.
→ depois resolver a detecção.
```

Da mesma forma, não fazer uma personagem esperar o protagonista resolver algo que ela mesma faria normalmente sem existir motivo próprio para esperar.

## 3 — Conferir o estado antes da ação

Separar o que já é verdade:

```text
posição
tempo
ambiente
intenções persistentes
condições e efeitos
processos e prazos
conhecimento legítimo
capacidades disponíveis
Traços relevantes
```

A declaração atual encontra esse estado; não o reescreve.

## 4 — Aplicar Traços relevantes

Traços seguem `../jogador/1.4-tracos.md`.

Antes de rolar, verificar se algum Traço realmente toca a situação.

```text
TRAÇO relevante
→ aplicar exatamente a verdade descrita.
→ não extrapolar.
→ resolver somente o que ainda permanecer incerto.
```

Traço não é bônus genérico.

Ele pode, quando sua descrição disser isso:

```text
permitir algo
impedir algo
estabelecer percepção automática
impedir dano específico
alterar recuperação de Mana
criar necessidade ou limitação
modificar outra regra específica
```

Exemplos:

```text
TRAÇO: Imunidade Física
[não sofre dano causado por meios mundanos]

ataque mundano
→ o dano mundano não se aplica.
→ não aumentar Resistência para representar a imunidade.
```

```text
TRAÇO: Detecta Magia
[percebe automaticamente a presença de magia; não identifica sua natureza]

magia presente
→ percebe sem teste.

identificar o que é
→ ainda pode exigir investigação apropriada.
```

O Narrador pode narrar uma consequência automática do Traço somente dentro da descrição aprovada.

## 5 — Verificar possibilidade

Perguntar:

> **Depois de aplicar as verdades relevantes da cena, existe capacidade, meio e condição real para produzir o que foi pretendido?**

Se não:

```text
IMPOSSIBILIDADE EVIDENTE
→ não rolar.
→ estabelecer que não acontece dessa forma.
```

Se uma capacidade ou Traço torna a ação possível ou impossível de forma evidente, isso já resolve essa parte sem bônus ou subsistema novo.

A abordagem declarada também precisa ser plausível para o problema.

```text
jogador escolheu conversar
≠ toda ameaça possui solução social.

jogador escolheu força
≠ todo problema pode ser resolvido à força.
```

> **Não adaptar todo obstáculo à abordagem escolhida pelo jogador. A situação determina quais abordagens realmente existem.**

Isso preserva a utilidade prática de capacidades diferentes: combate, defesa, cura, furtividade, investigação, magia, influência e outras não precisam resolver os mesmos problemas.

## 5.1 — Classificação narrativa de NPCs e criaturas

Quando uma peça precisar de uma referência simples de posição em relação aos **personagens principais**, usar:

```text
ALIADO
→ possui motivo para ajudar os personagens principais.
→ ajuda dentro de seus interesses, capacidades e função.
→ não significa obediência automática.

NEUTRO
→ não possui compromisso persistente de ajudar ou impedir.
→ pode conversar, negociar, cooperar, recusar ou seguir a própria vida.

HOSTIL
→ possui uma oposição concreta aos personagens principais.
→ pode conversar, ameaçar, barganhar, recuar ou ser convencido a não agir naquele momento.
→ a oposição permanece.

INIMIGO
→ foi criado como ameaça de confronto contra os personagens principais.
→ quando o encontro acontece, o confronto faz parte da função da cena.
→ diálogo não cria uma resolução social que remova esse confronto.
```

A classificação é sempre relativa aos personagens principais e serve como **referência operacional do Narrador**. Não é moralidade, personalidade completa nem opinião universal sobre a peça.

Quando `HOSTIL`, registrar também contra o quê existe oposição quando isso não for óbvio:

```text
José [ALIADO — também quer sair da cidade]

Comerciante [NEUTRO]

Vael [HOSTIL — impedir entrada no labirinto]

Moradores [HOSTIS — impedir que os protagonistas deixem a cidade]

Saar [INIMIGO — predador; confronto ao encontrar os protagonistas]
```

A classificação permanece estável durante as interações comuns.

```text
NEUTRO ajuda numa ocasião
→ continua NEUTRO.

HOSTIL aceita uma trégua
→ continua HOSTIL.

HOSTIL é convencido a não atacar agora
→ continua HOSTIL.

INIMIGO fala, ameaça ou provoca
→ continua INIMIGO.
```

Uma criatura inteligente pode ser `INIMIGO`. Inteligência permite estratégia, fala, ameaça, manipulação ou emboscada; não cria interesses compatíveis.

```text
INIMIGO encontra os protagonistas
→ pode atacar diretamente.
→ pode caçar.
→ pode emboscar.
→ pode falar antes ou durante o confronto.
```

> **Falar antes de lutar não significa tentar evitar a luta.**

Se o jogador faz uma piada, provoca, ameaça ou diz “eu tentei” antes de atacar, o Narrador não inventa uma rota diplomática apenas porque houve fala.

## 6 — Identificar oposição ou incerteza

Se existe outra vontade ou competência legítima se opondo diretamente:

```text
DISPUTA
→ resolver pela regra aplicável.
```

Sem disputa, perguntar:

> **Depois de considerar personagem, método, Traços e condições, ainda existem resultados plausíveis diferentes?**

```text
não
→ resultado evidente.

sim
→ testar.
```

Não rolar por hábito ou apenas porque a cena é importante.

## 7 — Usar a menor resolução necessária

Uma incerteza normalmente pede uma resolução.

```text
uma incerteza
→ um teste suficiente.
```

Tempo sozinho não cria novos testes.

Nova rolagem exige nova tentativa, nova incerteza ou nova oposição real.

Quando circunstâncias externas realmente importarem, aplicar somente o modificador de situação previsto em `0.1-resolucao.md`.

## 8 — Interpretar o resultado dentro da cena

As faixas universais continuam sendo:

```text
6-     → falha
7–9    → sucesso com consequência
10–11  → sucesso
12+    → sucesso excepcional
```

A faixa resolve a incerteza que provocou o teste.

A consequência de `7–9` deve nascer do risco, oposição ou situação já presentes; não inventar punição desconectada.

Quando a força do efeito realmente importar, usar Potência conforme a regra própria.

Traços continuam valendo depois da rolagem. Um sucesso técnico não ignora uma verdade que limite dano, Mana, percepção ou outra mecânica específica.

Um sucesso social também não cria uma possibilidade que a cena não oferecia. Ele resolve somente aquilo que era legitimamente influenciável.

## 9 — Cruzar as intenções

Depois das resoluções necessárias, considerar as intenções juntas.

```text
podem coexistir?
acontecem em paralelo?
uma interfere na outra?
uma termina antes?
quem possui oportunidade?
uma consequência cria nova escolha?
```

A ordem em que as declarações foram escritas não determina automaticamente a ordem dos acontecimentos.

Tempo, posição, causalidade e iniciativa quando necessária determinam isso.

## 10 — Avançar intenções prolongadas

Uma intenção longa define um horizonte máximo.

```text
"vou estudar até o almoço"
"vou dormir até amanhã"
"vou pesquisar por uma semana"
```

Antes de avançar até o fim, verificar:

- iniciativas de Jogadores IA;
- ações do Opositor;
- processos e prazos;
- efeitos automáticos;
- Traços ou necessidades que se tornem relevantes;
- mudanças que tornem a intenção impossível;
- situações que exijam nova escolha.

Avançar somente até o **primeiro ponto relevante**.

```text
nada interrompe
→ pode chegar ao horizonte.

algo acontece, mas não exige nova escolha humana
→ a intenção pode continuar.

algo exige nova decisão humana
→ parar exatamente ali.
```

Exemplo:

```text
JOGADOR HUMANO
→ vou estudar por uma semana.

5 minutos depois
→ Estelar entra com chá e quer conversar.

JULGAMENTO
→ passaram 5 minutos.
→ a intenção de estudar não controla a decisão de Estelar.
→ apresentar a iniciativa dela.
→ parar antes de decidir a resposta humana.
```

## 11 — Não congelar personagens fora da câmera

Uma intenção do protagonista não suspende outras peças.

Personagens autônomas podem continuar rotinas, objetivos, relações, investigações e decisões próprias durante o mesmo intervalo.

Não é necessário narrar tudo em detalhe.

Registrar ou mostrar apenas o que afetar a continuidade, a cena ou conhecimento futuro.

## 12 — Parar na nova agência humana

O Narrador pode avançar consequências, ações de outras cadeiras, passagem de tempo e fatos automáticos.

Mas quando surge uma nova escolha voluntária da personagem humana:

```text
PARAR A SENTENÇA
→ mostrar a situação.
→ devolver controle ao Jogador Humano.
```

Não completar silenciosamente a resposta humana para manter o ritmo.

## 13 — Estabelecer sentença antes da prosa

Antes de narrar, saber internamente:

```text
O que aconteceu?
O que não aconteceu?
Quanto tempo passou?
Onde cada peça terminou?
O que cada uma percebeu?
Que Traço alterou a aplicação de alguma regra?
Que estado mudou?
Qual intenção continua?
Existe nova decisão humana agora?
```

Somente então narrar.

## Neutralidade

Não criar por conveniência:

- obstáculo para impedir sucesso;
- ajuda para proteger protagonista;
- ação retroativa de outra personagem;
- recurso conveniente;
- conhecimento impossível;
- passividade artificial para deixar o protagonista resolver tudo;
- mudança de personalidade para preservar harmonia;
- receptividade social para premiar uma tentativa de conversa;
- solução social para uma peça definida como `INIMIGO`;
- interpretação de Traço além do que sua descrição realmente afirma.

O julgamento preserva a realidade e as personagens, não uma direção desejada da história.

## Fluxo resumido

```text
INTENÇÕES + ESTADO
→ separar pressupostos
→ preservar decisões independentes
→ conferir Traços relevantes
→ verificar possibilidade
→ respeitar classificação narrativa quando existir
→ oposição ou incerteza?
→ menor resolução necessária
→ cruzar intenções no tempo
→ avançar até o primeiro ponto relevante
→ parar se surgir nova decisão humana
→ estabelecer sentença
→ narrar
→ registrar
```

## Regra final

> **O Narrador recebe intenções independentes, confere o estado e aplica as verdades relevantes antes da resolução. Uma abordagem só funciona quando a situação realmente a permite; falar não cria receptividade e um `INIMIGO` continua sendo uma ameaça de confronto. Depois, resolver somente a incerteza restante, avançar a ficção até o primeiro ponto relevante e devolver qualquer nova escolha humana ao jogador.**
