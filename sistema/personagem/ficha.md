# Ficha de Personagem

Status: APROVADO

A ficha é o **dossiê consolidado do personagem**: registra quem ele é, o que consegue fazer e as informações que precisam permanecer disponíveis para interpretação e continuidade.

Ela não precisa ser curta. Precisa ser organizada e conter informação útil para decisão, interpretação, capacidade ou continuidade.

## Ficha não é STATUS

A ficha pode guardar, quando relevantes:

- identidade;
- importância;
- `CONTROLE`;
- idade;
- conceito;
- descrição;
- TRAÇOS;
- atributos;
- perícias;
- poderes;
- RECURSOS;
- relações recorrentes;
- personalidade e tendências;
- desejos e objetivos atuais relevantes;
- medos e limites;
- conhecimento atual relevante;
- história consolidada necessária à interpretação.

Não pertencem à ficha apenas por estarem ativos agora:

- VIDA atual;
- ENERGIA atual;
- condições temporárias;
- efeitos ativos;
- localização atual;
- ferimentos transitórios;
- favores circunstanciais;
- consequências latentes ainda não incorporadas ao personagem;
- demais informações puramente operacionais do momento.

Esses elementos pertencem ao STATUS ou a outras camadas de persistência.

> **Ficha = dossiê consolidado do personagem. STATUS = como ele está agora.**

A diferença principal não é entre “permanente” e “atual”, mas entre **informação consolidada necessária para interpretar o personagem** e **estado circunstancial da cena ou campanha**.

## Organização visual

A ficha apresenta primeiro identidade e informações mecânicas de consulta rápida.

Informações extensas de interpretação e continuidade ficam abaixo, em seções próprias.

Ordem recomendada:

```text
# Nome

Status:
Importância:
CONTROLE:

Idade:
Conceito:
Descrição:

TRAÇOS:
ATR:
PER:
PODERES:
RECURSOS:
REL:

## Personalidade e tendências
## Desejos / objetivos atuais
## Medos / limites relevantes
## Conhecimento atual relevante
## História consolidada relevante
```

Essa ordem é apenas uma referência estética. **Qualquer personagem pode ter uma ficha de qualquer tamanho ou formato**, independentemente de sua Importância.

Um Figurante pode possuir dez páginas de informação se isso for útil. Um Relevante pode ter apenas três linhas se isso for suficiente.

## Campo desconhecido fica em branco

Durante criação ou revisão, não usar zero para significar “ainda não definido”.

```text
ATR: FOR [ ] | AGI [ ] | RES [ ] | MEN [ ] | VON [ ]
```

é diferente de:

```text
ATR: FOR [0] | AGI [0] | RES [0] | MEN [0] | VON [0]
```

No segundo caso, todos os valores já foram mecanicamente definidos.

> **Zero é valor real, nunca marcador de pendência.**

## IMPORTÂNCIA

`IMPORTÂNCIA` indica o peso estrutural do personagem para a história e ajuda a organizar como sua agência pode ser tratada na campanha.

Ela **não** determina:

- tamanho da ficha;
- quantidade obrigatória de informações;
- atributos;
- perícias;
- poderes;
- dificuldade;
- proteção narrativa;
- `CONTROLE` automático para personagens não Centrais.

As categorias são:

```text
Importância: Central
Importância: Relevante
Importância: Figurante
```

### Central

É parte do núcleo jogável da campanha.

Normalmente a campanha possui no máximo dois personagens Centrais:

```text
1 JOGADOR HUMANO
1 JOGADOR IA dedicado
```

O JOGADOR IA dedicado existe exclusivamente para seu personagem Central.

Personagens Centrais possuem agência própria de jogador e não ficam sob controle normal do NARRADOR.

### Relevante

É um personagem estruturalmente importante para a campanha, mas que não pertence ao núcleo central.

Um personagem Relevante pode permanecer:

```text
CONTROLE: NPC
```

sob uso normal do NARRADOR, ou pode usar:

```text
CONTROLE: JOGADOR IA EVENTUAL
```

quando essa função tiver sido definida para ele.

> **Ser Relevante não transforma automaticamente o personagem em JOGADOR IA EVENTUAL.**

A Importância descreve seu peso estrutural. O `CONTROLE` registra quem possui normalmente sua autoridade de decisão.

Quando houver personagens sob `JOGADOR IA EVENTUAL`, uma única IA EVENTUAL pode assumir todos os personagens ativos dessa categoria ao mesmo tempo.

### Figurante

É um personagem sem papel estrutural central ou relevante para a campanha naquele momento.

Figurantes permanecem normalmente como `NPC`, sob uso do NARRADOR.

A frequência de aparição não altera essa classificação. Um entregador, guarda, comerciante ou outro NPC pode aparecer repetidamente durante toda a campanha e continuar Figurante.

### Importância é quase fixa

IMPORTÂNCIA representa função estrutural na campanha e não deve subir ou descer apenas porque um personagem apareceu mais vezes ou ganhou momentaneamente destaque.

Se o `JOGADOR IA EVENTUAL` entender que um Figurante deveria se tornar Relevante, ou que um Relevante deveria se tornar Central, ele **deve perguntar ao JOGADOR HUMANO antes da promoção**.

Sem aprovação, a classificação permanece como está.

Uma promoção aprovada não altera automaticamente nenhuma outra parte da ficha. Atributos, perícias, poderes, recursos e demais informações continuam iguais. Novos campos de descrição podem ser acrescentados depois apenas se forem úteis para continuidade.

> **Na dúvida, manter a classificação atual.**

## CONTROLE

A ficha pode registrar:

```text
CONTROLE: JOGADOR HUMANO
CONTROLE: JOGADOR IA
CONTROLE: JOGADOR IA EVENTUAL
CONTROLE: NPC
```

`CONTROLE` é metadado estrutural e não atributo mecânico.

Ele informa como o personagem participa normalmente do ciclo e quem possui autoridade usual sobre suas decisões.

### JOGADOR HUMANO

É o personagem Central do jogador humano.

### JOGADOR IA

É o personagem Central com uma IA dedicada exclusivamente a ele. É apropriado para coprotagonista, parceiro romântico ou outro personagem cuja agência individual precisa ser preservada continuamente.

### JOGADOR IA EVENTUAL

É uma categoria de controle possível para personagens não Centrais quando essa agência própria tiver sido definida para eles.

Uma mesma IA EVENTUAL pode assumir simultaneamente todos os personagens dessa categoria que precisarem de agência própria naquela situação.

Um personagem não recebe esse `CONTROLE` apenas por ser Relevante. A classificação precisa estar registrada na ficha conforme as regras operacionais da campanha.

### NPC

É personagem de uso normal do NARRADOR. Inclui figurantes, civis, monstros, inimigos, criaturas, aliados, antagonistas recorrentes e também personagens Relevantes que permaneçam sob autoridade normal do NARRADOR.

## OPOSITOR não é um tipo de CONTROLE

O OPOSITOR não possui uma categoria permanente de personagem.

Sua função é **gerar problemas e apresentar oposição**.

Ele pode propor a entrada de NPCs, forças, ameaças, interrupções ou outros elementos capazes de produzir oposição. O NARRADOR julga se a proposta é válida e coerente com a ficção.

Exemplo:

```text
OPOSITOR:
Trigon envia dois assassinos.

NARRADOR:
Julga se Trigon pode fazer isso e se a entrada desses assassinos é coerente.
```

Se a proposta for aceita, os assassinos continuam sendo `NPC`, mas o NARRADOR pode **delegá-los temporariamente ao OPOSITOR** para que ele jogue com eles durante aquela oposição.

Quando a delegação termina, eles continuam sendo NPCs. Não existe `CONTROLE: OPOSITOR` na ficha.

O mesmo vale para qualquer NPC já existente. O OPOSITOR pode propor usar um entregador para interromper uma cena, um guarda para bloquear uma passagem ou um monstro para atacar; o NARRADOR julga a validade e, quando apropriado, executa o NPC ou o delega temporariamente ao OPOSITOR.

> **O OPOSITOR provoca e argumenta pela oposição. O NARRADOR julga e pode disponibilizar NPCs para executá-la.**

As regras operacionais detalhadas dessas categorias pertencem a `../personas/` e ao ciclo do sistema. Esta área apenas registra a estrutura da ficha.

## RECURSOS

`RECURSOS` registra o mínimo necessário sobre meios, infraestrutura, instalações, organizações, objetos únicos ou preparações específicas que já foram estabelecidos e podem alterar possibilidades na ficção.

Não é inventário e não é catálogo de patrimônio.

Um recurso só precisa ser registrado quando sua existência, ausência ou estado puder efetivamente ser útil para decisões futuras.

Exemplo:

```text
RECURSOS:
Castelo dos Corvos => Forja antiga, Biblioteca imensa, Laboratório de alquimia, Sala de tango, Solar, 5 quartos
Chave do Cofre de Balaladom [perdida]
Fórmula anti-Charada [uso único]
```

O objetivo é estabelecer fatos simples.

Ter um castelo não significa automaticamente possuir toda instalação que venha a ser conveniente depois. Se a ficha registra `Forja antiga`, então existe uma forja. Se não registra uma instalação e ela nunca foi estabelecida na ficção, sua existência não deve ser presumida apenas por conveniência.

Novos RECURSOS podem ser adicionados naturalmente quando forem estabelecidos e passarem a ter utilidade real.

Não é necessário grande evento mecânico para atualizar essa linha. A ficha apenas passa a refletir o que já existe.

RECURSOS não possuem Patamar por padrão e não concedem bônus automáticos. Eles estabelecem meios, infraestrutura, acesso e possibilidades concretas.

A ausência de um meio necessário pode ser apresentada pelo OPOSITOR como fundamento de oposição.

Exemplo:

```text
JOGADOR:
“Vou forjar uma espada.”

OPOSITOR:
“Com qual forja?”
```

Se a ficha já estabelece uma `Forja antiga`, existe suporte ficcional para essa parte da ação. Se não existe forja ou meio equivalente, o NARRADOR julga a oposição apresentada.

RECURSOS também não anulam limites físicos ou ficcionais. Se novas instalações começarem a parecer incompatíveis com o espaço ou estrutura já estabelecidos, o OPOSITOR pode questionar se realmente cabem, se exigem reforma, expansão ou demolição de algo existente. O NARRADOR julga.

> **RECURSOS registram apenas o que foi efetivamente estabelecido e pode ser útil depois.**

## Modelo-base de ficha

O sistema não exige modelos diferentes para Central, Relevante ou Figurante. O mesmo formato pode ser expandido ou reduzido livremente conforme a necessidade real.

```text
# Nome

Status: PENDENTE DE REVISÃO
Importância: ...
CONTROLE: ...

Idade:
Conceito:
Descrição:

TRAÇOS:
- ...

ATR: FOR [ ] | AGI [ ] | RES [ ] | MEN [ ] | VON [ ]
PER:
PODERES:
RECURSOS:
REL:

## Personalidade e tendências
- ...

## Desejos / objetivos atuais
- ...

## Medos / limites relevantes
- ...

## Conhecimento atual relevante
- ...

## História consolidada relevante
- ...
```

Campos sem utilidade real podem ser omitidos ou permanecer vazios.

## Informação reservada do NARRADOR

Quando uma ficha pertencente ao mundo precisar guardar uma verdade que não pode ser apresentada ao jogador, ela pode incluir uma seção reservada como:

```text
## Informação reservada do NARRADOR
- identidade oculta;
- plano ainda não descoberto;
- conhecimento secreto;
- pacto desconhecido;
- capacidade ou limitação que ainda não foi revelada;
- outro fato consolidado que precise permanecer secreto.
```

Essa seção é opcional e só deve existir quando houver informação realmente estabelecida que precise ser preservada em sigilo.

Ela não autoriza criar fatos retroativamente para contrariar uma ação válida, restaurar dificuldade ou proteger a trama.

A informação pode ser secreta para os personagens e para o jogador, mas continua sendo uma verdade já estabelecida da campanha.

## Ficha reservada

Quando um personagem precisa de continuidade sem revelar suas capacidades ou segredos ao jogador, pode usar a mesma linguagem de ficha em uma área reservada da aventura.

A ficha reservada pode usar `## Informação reservada do NARRADOR` quando isso for útil.

A ficha reservada preserva segredo; não autoriza alterar capacidades retroativamente apenas para contrariar uma solução válida.

## Aprovação

Durante criação e revisão de fichas apresentáveis ao jogador, usar:

```text
Status: PENDENTE DE REVISÃO
```

Somente depois da aprovação explícita da ficha consolidada mudar para:

```text
Status: APROVADO
```

Fichas reservadas do NARRADOR podem usar estado canônico próprio quando uma aprovação aberta revelaria segredos.

## Alterações posteriores

A ficha não recebe XP ou melhorias automáticas por missão ou capítulo.

Se a ficção alterar de verdade o personagem — por transformação permanente, aquisição real de uma capacidade, perda estrutural, mudança estável de identidade ou equivalente — a parte mecânica da ficha pode ser atualizada para representar a nova realidade.

As partes narrativas também podem ser atualizadas quando novos objetivos, conhecimentos, relações, limites ou fatos consolidados passarem a ser necessários para interpretar corretamente o personagem.

> **A ficha acompanha quem o personagem é e o que precisa ser lembrado para interpretá-lo corretamente.**

O procedimento de atualização e persistência pertence a `../persistencia/`.
