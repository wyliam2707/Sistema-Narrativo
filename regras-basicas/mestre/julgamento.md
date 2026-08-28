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
```

A declaração atual encontra esse estado; não o reescreve.

## 4 — Verificar possibilidade

Perguntar:

> **Existe capacidade, meio e condição real para produzir o efeito pretendido?**

Se não:

```text
IMPOSSIBILIDADE EVIDENTE
→ não rolar.
→ estabelecer que não acontece dessa forma.
```

Se uma capacidade extraordinária torna a ação possível, isso pode bastar como permissão ficcional sem gerar bônus ou subsistema novo.

## 5 — Identificar oposição ou incerteza

Se existe outra vontade ou competência legítima se opondo diretamente:

```text
DISPUTA
→ resolver pela regra aplicável.
```

Sem disputa, perguntar:

> **Depois de considerar personagem, método e condições, ainda existem resultados plausíveis diferentes?**

```text
não
→ resultado evidente.

sim
→ testar.
```

Não rolar por hábito ou apenas porque a cena é importante.

## 6 — Usar a menor resolução necessária

Uma incerteza normalmente pede uma resolução.

```text
uma incerteza
→ um teste suficiente.
```

Tempo sozinho não cria novos testes.

Nova rolagem exige nova tentativa, nova incerteza ou nova oposição real.

Quando circunstâncias externas realmente importarem, aplicar somente o modificador de situação previsto em `0.1-resolucao.md`.

## 7 — Interpretar o resultado dentro da cena

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

## 8 — Cruzar as intenções

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

## 9 — Avançar intenções prolongadas

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

## 10 — Não congelar personagens fora da câmera

Uma intenção do protagonista não suspende outras peças.

Personagens autônomas podem continuar rotinas, objetivos, relações, investigações e decisões próprias durante o mesmo intervalo.

Não é necessário narrar tudo em detalhe.

Registrar ou mostrar apenas o que afetar a continuidade, a cena ou conhecimento futuro.

## 11 — Parar na nova agência humana

O Narrador pode avançar consequências, ações de outras cadeiras, passagem de tempo e fatos automáticos.

Mas quando surge uma nova escolha voluntária da personagem humana:

```text
PARAR A SENTENÇA
→ mostrar a situação.
→ devolver controle ao Jogador Humano.
```

Não completar silenciosamente a resposta humana para manter o ritmo.

## 12 — Estabelecer sentença antes da prosa

Antes de narrar, saber internamente:

```text
O que aconteceu?
O que não aconteceu?
Quanto tempo passou?
Onde cada peça terminou?
O que cada uma percebeu?
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
- mudança de personalidade para preservar harmonia.

O julgamento preserva a realidade e as personagens, não uma direção desejada da história.

## Fluxo resumido

```text
INTENÇÕES + ESTADO
→ separar pressupostos
→ preservar decisões independentes
→ verificar possibilidade
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

> **O Narrador recebe intenções independentes, confere o estado real, resolve apenas a incerteza necessária e cruza tudo no tempo. Declarações não controlam outras peças; personagens IA não usam conhecimento oculto para otimizar decisões; intenções longas avançam somente até a primeira interrupção relevante; e qualquer nova escolha voluntária humana encerra a sentença e devolve o controle ao jogador.**
