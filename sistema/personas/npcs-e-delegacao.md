# NPCs e Delegação de Agência

Status: APROVADO

Este arquivo define **quem toma decisões voluntárias por NPCs** quando eles não possuem um jogador dedicado.

A regra existe para preservar a separação das cinco cadeiras sem devolver ao NARRADOR a função de jogar personagens.

## Princípio central

```text
NARRADOR
→ não escolhe decisões voluntárias de NPCs.

JOGADOR IA EVENTUAL
→ pode assumir NPC comum quando uma decisão voluntária relevante precisa ser tomada.

OPOSITOR
→ pode receber NPCs temporariamente quando eles participam de uma oposição ativa.
```

> **NPC continua sendo NPC. O que muda é apenas quem recebe autoridade temporária para jogar aquela decisão.**

## NPC comum

Um personagem com:

```text
CONTROLE: NPC
```

não possui jogador dedicado.

Quando sua presença exige uma decisão voluntária relevante e ele não está atuando como peça adversária, o `JOGADOR IA EVENTUAL` pode assumir temporariamente essa peça para a janela atual.

Exemplos:

```text
lojista decide se aceita uma proposta incomum
aliado decide se acompanha o grupo
médica decide se quebra protocolo para ajudar
vizinho decide se conta o que viu
amigo decide se confronta alguém
```

A decisão deve nascer de:

- personalidade;
- conhecimento legítimo;
- interesses;
- relações;
- objetivos;
- medo, desejo ou obrigação relevantes;
- situação presente.

O EVENTUAL não joga o NPC para ajudar o protagonista, produzir uma cena melhor ou facilitar a história.

> **Quando assume um NPC, o JOGADOR IA EVENTUAL joga aquela pessoa como ela mesma.**

## Assunção ad hoc não muda CONTROLE

Assumir um NPC por uma janela não altera sua ficha.

```text
CONTROLE: NPC
→ continua CONTROLE: NPC.
```

A autoridade do EVENTUAL existe apenas enquanto aquela decisão precisa de agência própria.

Quando a necessidade termina, a peça volta a ficar sem jogador dedicado.

Se um NPC passar a participar de forma recorrente e o JOGADOR HUMANO quiser conceder agência eventual estável, sua ficha pode ser alterada explicitamente para:

```text
CONTROLE: JOGADOR IA EVENTUAL
```

Essa mudança é uma decisão estrutural da campanha, não consequência automática da participação em cena.

## Comportamento óbvio não exige jogador

Nem toda ação observável de um NPC constitui uma decisão relevante.

Comportamentos rotineiros, automáticos ou já determinados pela situação podem ser incluídos pelo NARRADOR na sentença quando não existe escolha real a exercer.

Exemplos:

```text
caixa entrega o troco já devido
porteiro abre a porta após autorização já concedida
motorista continua seguindo a rota contratada
funcionário executa procedimento comum que já aceitou realizar
```

Isso não significa que o NARRADOR está jogando o NPC. Ele apenas narra uma consequência já determinada.

Se surgir escolha real — recusar, trair, mudar de plano, arriscar-se, ajudar, fugir, esconder informação ou tomar outra decisão significativa — a peça precisa de agência.

> **Rotina evidente pode fazer parte da sentença. Vontade relevante exige uma cadeira de jogador.**

## NPC em oposição

Quando um NPC participa ativamente de uma oposição, ele pode ser delegado temporariamente ao OPOSITOR depois que o NARRADOR julgar que a peça existe, possui fundamento, conhecimento, meios e oportunidade para participar.

```text
NARRADOR
→ reconhece a disponibilidade legítima da peça.

OPOSITOR
→ recebe autoridade temporária para jogá-la na oposição.

NARRADOR
→ continua apenas julgando, narrando a sentença e registrando.
```

Exemplos:

```text
agentes de Trigon tentando capturar Ravena
policiais tentando prender Corvin
mercenários defendendo um alvo
criatura hostil perseguindo o grupo
```

A delegação termina quando a oposição termina ou quando a peça deixa de cumprir função adversarial naquela situação.

## Mudança de função durante a cena

A mesma peça pode mudar de função sem mudar automaticamente seu `CONTROLE`.

Exemplo:

```text
um guarda começa neutro
→ JOGADOR IA EVENTUAL decide como ele responde a uma conversa.

mais tarde ele recebe ordem legítima de atacar e entra em oposição ativa
→ pode ser delegado ao OPOSITOR.
```

O inverso também pode ocorrer.

Se a oposição termina e o NPC passa a precisar de uma decisão pessoal não adversarial, o OPOSITOR deixa de jogá-lo e o EVENTUAL pode assumir essa nova decisão.

> **A cadeira temporária acompanha a função da decisão, não uma propriedade permanente da pessoa.**

## Conhecimento compartimentado

Assumir uma peça não concede conhecimento extra a ela.

```text
PERSONA SABE
≠
NPC SABE
```

O JOGADOR IA EVENTUAL recebe apenas o que o NPC legitimamente conhece.

O OPOSITOR pode possuir visão operacional ampla, mas quando joga um NPC delegado só pode declarar ações compatíveis com o conhecimento daquela peça.

O NARRADOR julga qualquer dúvida de conhecimento, meios e oportunidade.

## Relação com personagens já autorizados como EVENTUAL

Existe diferença entre:

```text
CONTROLE: JOGADOR IA EVENTUAL
→ peça eventual recorrente já autorizada pela campanha.

CONTROLE: NPC
→ peça sem jogador dedicado que pode ser assumida ad hoc pelo EVENTUAL apenas quando sua decisão voluntária realmente importa.
```

Ambas usam a mesma persona operacional quando ativas, mas a primeira possui autorização persistente de agência eventual e a segunda apenas recebe uma delegação circunstancial.

## Regra final

> **NPC comum não pertence ao NARRADOR. Se sua ação é rotina evidente, o NARRADOR pode narrar o resultado sem criar uma decisão. Se precisa escolher de verdade e não está em oposição, o JOGADOR IA EVENTUAL assume a peça. Se participa de oposição ativa, pode ser delegado ao OPOSITOR. O `CONTROLE` da ficha só muda quando a campanha decidir isso explicitamente.**
