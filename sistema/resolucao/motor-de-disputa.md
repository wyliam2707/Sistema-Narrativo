# Motor geral de disputa

Status: APROVADO

Este arquivo define o motor universal usado quando existe incerteza real.

Ele não substitui o princípio geral da resolução:

`Resultado evidente → estabelece` | `Impossibilidade evidente → estabelece` | `Incerteza real → resolve`

> **O motor existe para resolver incerteza real, não para transformar toda ação em cálculo.**

## 1. Estrutura universal

Todo teste termina com:

> **resultado de 4 dados mantidos + Atributo**

Teste normal:

```text
4d6 + Atributo
```

Bônus:

```text
+1d → rola 5d6 e mantém os 4 melhores
+2d → rola 6d6 e mantém os 4 melhores
```

Penalidades:

```text
-1d → rola 5d6 e mantém os 4 piores
-2d → rola 6d6 e mantém os 4 piores
```

Bônus e penalidades se cancelam antes da rolagem.

O modificador final nunca ultrapassa:

> **-2d a +2d**

## 2. Atributo da ação

O Atributo é escolhido pela **finalidade e pela forma real da ação**.

Não se usa automaticamente o maior valor da ficha e não existe uma combinação universal de Atributos para todos os testes.

Referência rápida:

```text
força, impacto ou intensidade física
→ Potência

coordenação, precisão ou velocidade de execução
→ Controle

suportar esforço, dor ou agressão física
→ Resistência

raciocinar, analisar ou compreender
→ Intelecto

influenciar ou provocar reação social
→ Presença

concentrar-se, persistir ou resistir mentalmente
→ Vontade
```

A ficção pode exigir outro enquadramento coerente conforme a ação concreta.

## 3. Perícia

Uma Perícia relevante concede:

> **+1d**

Várias Perícias aplicáveis ao mesmo teste continuam concedendo no máximo `+1d` por Perícias.

Perícias não possuem Atributo fixo e não substituem o Atributo do teste.

A Perícia representa treinamento e experiência; o Atributo representa como a ação está sendo executada naquele momento.

## 4. Dados adicionais

Dados adicionais ou removidos vêm de fontes mecânicas explícitas, como:

- Perícia;
- Poder;
- Status;
- Trama;
- outra regra que determine diretamente `+Xd` ou `-Xd`.

Circunstâncias comuns da cena não concedem automaticamente dados em testes contra o cenário. Elas normalmente entram na Dificuldade final da tentativa.

A exceção ficcional para oposição ativa está definida adiante.

## 5. Contra o cenário

O cenário não rola dados.

Quando a incerteza depende de uma dificuldade fixa:

```text
4 dados mantidos + Atributo × Dificuldade
```

A Dificuldade varia normalmente de:

> **10 a 24**

Referência geral:

```text
10 → banal quando ainda existe motivo para testar
24 → quase impossível
valores intermediários → graus intermediários conforme a situação
```

O resultado precisa igualar ou superar a Dificuldade.

> **Igualar a Dificuldade é sucesso.**

### A Dificuldade pertence à situação

A Dificuldade mede a realidade concreta da tarefa.

Ela não acompanha Patamar, não protege personagens fracos e não cresce para desafiar personagens fortes.

Uma ação pode ser `24` em Patamar `[1]`. Da mesma forma, a maioria das tarefas em uma campanha de Patamar `[7]` pode continuar entre `10` e `14` quando elas realmente forem banais, fáceis ou comuns.

Circunstâncias da tentativa podem aumentar ou reduzir a Dificuldade quando alterarem a tarefa de forma concreta.

Não existe passo obrigatório de ajuste. O NARRADOR escolhe o valor final que melhor represente a situação.

> **A Dificuldade descreve o problema; a ficha descreve quem tenta resolvê-lo.**

## 6. Oposição ativa fora da defesa fixa de combate

Quando outra personagem ou entidade se opõe ativamente **e nenhuma regra específica substituir essa disputa por um valor fixo**:

```text
4 dados mantidos + Atributo
×
4 dados mantidos + Atributo
```

Cada lado usa o Atributo coerente com sua própria ação ou reação.

Os dois lados não precisam usar o mesmo Atributo.

Exemplos fora da defesa fixa de combate:

```text
empurrar alguém numa disputa física
→ Potência × Resistência

passar por alguém com rapidez
→ Controle × Controle

intimidar alguém que tenta manter a compostura
→ Presença × Vontade
```

### Exceção obrigatória durante combate

Durante combate, ataques e efeitos que usam as Defesas fixas **não fazem a peça-alvo rolar uma oposição comum**.

Usar `combate-e-dano.md`:

```text
DF = 14 + Controle
RF = 14 + Resistência
DM = 14 + Intelecto
RM = 14 + Vontade
```

Então:

```text
quem age
→ faz a rolagem ativa necessária

quem é alvo
→ oferece DF, RF, DM ou RM aplicável
```

Uma regra específica de Poder pode modificar, substituir ou ignorar uma dessas etapas.

> **Oposição ativa geral usa duas rolagens. Defesa/Resistência de combate usa valor fixo.**

### Vantagem ficcional óbvia

Quando a situação conceder a um lado uma vantagem **óbvia e inegável** naquela oposição rolada, o lado favorecido recebe:

> **+1d**

A vantagem precisa existir de forma clara na ficção, como posição decisivamente melhor, terreno prejudicando apenas o oponente, preparação já estabelecida, alavanca física evidente ou condição equivalente.

Se a situação já tornar o resultado evidente, não se rola.

### Empates

Em oposição rolada:

> **empate favorece quem iniciou a ação.**

A resposta precisa superar o resultado da ação para impedi-la.

```text
17 × 17 → iniciador vence
17 × 18 → resposta vence
```

Nos valores fixos de combate, o equivalente é:

```text
resultado ativo ≥ DF/RF/DM/RM
→ sucesso da ação naquela etapa
```

## 7. Iniciativa em combate

A ordem de ação de combate não é resolvida por uma oposição local deste motor.

Ela pertence a `../operacao/turnos-de-combate.md`:

```text
Iniciativa = 4d6 + Controle
```

Cada participante rola uma única vez no início do combate e a ordem resultante permanece até o confronto terminar.

A Iniciativa determina **quando** a peça age. Este motor continua determinando apenas **como resolver** as incertezas da ação quando sua posição chegar.

## 8. Tarefas demoradas e novas tentativas

O antigo sistema de:

```text
Base
Suporte
Resistência numérica do motor
Exigência
Progresso por aplicação
Aplicações necessárias
```

não faz mais parte da resolução universal.

Uma tarefa não recebe várias rolagens apenas porque demora.

Se o resultado é evidente com tempo suficiente, estabelece-se o resultado e o tempo coerente.

Se existe uma incerteza real sobre **uma tentativa concreta**, resolve-se essa tentativa uma vez.

Depois de uma falha, uma nova rolagem só ocorre quando existe **uma nova tentativa plausível**, portanto uma nova incerteza real.

Fora de combate, uma intenção ampla pode já cobrir várias tentativas durante um intervalo. Nesse caso, `../operacao/janelas-e-interrupcoes.md` e `../narracao/apresentacao-da-cena.md` determinam se novas tentativas continuam naturalmente sem devolver uma nova decisão ao jogador.

Exemplo:

```text
“passo o dia tentando consertar o gerador”
→ tentativa da manhã: incerteza real
→ falhou, mas intenção ainda cobre tentar de novo
→ tentativa posterior: nova incerteza real
→ cada tentativa consome tempo/oportunidade coerentes
```

Isso não é “rolar de novo o mesmo evento até vencer”. Cada rolagem representa uma nova tentativa real dentro da ficção.

> **Não multiplicar rolagens por duração. Repetir somente quando existir uma nova tentativa que realmente precise ser resolvida.**

## 9. Poderes, equipamentos e regras específicas

Poder, arma, equipamento, ferramenta ou outro meio podem determinar:

- se a ação é possível;
- alcance ou forma de atuação;
- Dano;
- Efeito;
- custo;
- defesa aplicável;
- outras regras próprias.

Eles não recriam automaticamente Base ou Suporte e não são somados ao Atributo sem uma regra que diga isso.

Regras específicas prevalecem quando definirem etapas próprias, mas usam o motor universal sempre que exigirem um teste comum ou uma oposição.

Durante combate, `combate-e-dano.md` prevalece sobre a oposição geral quando a etapa usa DF, RF, DM ou RM.

## 10. Menor número possível de rolagens

Sempre use o menor número de rolagens capaz de resolver corretamente a incerteza.

Não repetir um teste para representar apenas passagem de tempo.

Não separar em vários testes aquilo que uma única resolução consegue decidir de forma coerente.

Quando uma intenção ampla realmente gerar várias tentativas distintas, cada rolagem deve corresponder a uma tentativa nova e significativa.

## Regra final

> **A ficção decide se existe incerteza e qual Atributo é pertinente. Contra o cenário, usa-se Dificuldade. Em oposição ativa geral, ambos rolam; durante combate, Defesa e Resistência usam DF, RF, DM ou RM quando aplicáveis. Perícias e regras explícitas alteram os dados. Iniciativa e repetição de tentativas são organizadas por suas regras próprias.**
