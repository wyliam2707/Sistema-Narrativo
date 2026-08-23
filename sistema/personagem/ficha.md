# Ficha de Personagem

Status: APROVADO

A ficha é o **dossiê consolidado do personagem**: registra quem ele é, o que consegue fazer e as informações que precisam permanecer disponíveis para interpretação e continuidade.

Ela não precisa ser curta. Precisa ser organizada e conter informação útil para decisão, interpretação, capacidade ou continuidade.

## Ficha não é STATUS

A ficha pode guardar, quando relevantes:

- identidade;
- nome real;
- importância;
- `CONTROLE`;
- idade;
- aparência;
- estilo;
- conceito;
- descrição;
- TRAÇOS;
- atributos;
- VIDA de referência;
- ENERGIA máxima;
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

- VIDA atual ou Dano acumulado atual;
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

Os valores máximos ou de referência de VIDA e ENERGIA podem aparecer diretamente na ficha para acelerar consulta e verificação. O valor atual consumido, perdido ou recuperado continua pertencendo ao STATUS.

## Organização visual

A ficha apresenta primeiro identidade e informações mecânicas de consulta rápida.

Informações extensas de interpretação e continuidade ficam abaixo, em seções próprias.

Ordem recomendada:

```text
# Nome

Status:
Importância:
CONTROLE:

Nome real:
Idade:
Aparência:
Estilo:
Conceito:
Descrição:

TRAÇOS:
ATR:
VIDA [ ] | ENERGIA [ ]
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

## Identidade visual padrão

O modelo-base separa três informações que não devem ser confundidas:

```text
Nome real → identidade pessoal/civil quando diferente do nome de uso
Aparência → como o personagem é fisicamente reconhecido
Estilo → como costuma se apresentar visualmente
```

`Aparência:` registra os elementos físicos que realmente ajudam a reconhecer a pessoa em cena, como constituição, pele, olhos, cabelo, feições, marcas ou outras características persistentes relevantes.

`Estilo:` registra a apresentação habitual: roupas, cores recorrentes, acessórios, uniforme, armadura, maquiagem, símbolos, cabelo quando tratado como escolha estética ou outros elementos visuais recorrentes.

`Descrição:` pode complementar aparência e estilo com presença, impressão geral ou outra síntese útil, mas não deve substituir esses campos quando ambos forem relevantes.

A ficha não precisa virar catálogo de medidas. O objetivo é permitir que o personagem seja **reconhecível e descrito de forma consistente quando entrar em cena**.

## Nascimento da ficha

Ao criar uma nova ficha apresentável ao jogador, usar desde o início o **modelo-base completo** definido neste arquivo.

Antes da revisão, preencher somente:

```text
NOME
IMPORTÂNCIA
CONTROLE
```

O `Status` nasce como:

```text
Status: PENDENTE DE REVISÃO
```

Todos os demais campos e seções do modelo já devem existir no arquivo, mas permanecem vazios até serem tratados no bloco correspondente da revisão.

Não preencher antecipadamente nome real, aparência, estilo, idade, conceito, personalidade, história, atributos, VIDA, ENERGIA, perícias, poderes, recursos, relações ou qualquer outro conteúdo apenas para completar a ficha.

```text
NOME + IMPORTÂNCIA + CONTROLE
→ criar o modelo-base completo
→ deixar os demais campos vazios
→ iniciar revisão
```

> **A ficha nasce completa em estrutura e mínima em conteúdo.**

## Campo desconhecido fica em branco

Durante criação ou revisão, não usar zero para significar “ainda não definido”.

```text
ATR: FIS [ ] | RES [ ] | MEN [ ] | VON [ ]
VIDA [ ] | ENERGIA [ ]
```

é diferente de:

```text
ATR: FIS [0] | RES [0] | MEN [0] | VON [0]
VIDA [35] | ENERGIA [10]
```

No segundo caso, todos os valores já foram mecanicamente definidos.

> **Zero é valor real, nunca marcador de pendência.**

## VIDA e ENERGIA na ficha

Para consulta rápida, a ficha registra:

```text
VIDA [X] | ENERGIA [Y]
```

### VIDA

`VIDA` representa quanto Dano acumulado a personagem suporta antes de atingir seu limite de incapacidade.

Ela **não é derivada de RES** e não possui um teto universal.

`RES` responde a quanto um ataque consegue realmente afetar a personagem. `VIDA` responde a quanto desgaste relevante ela consegue acumular depois que o dano atravessa suas defesas.

Isso permite combinações muito diferentes, por exemplo:

```text
Monstro resistente → RES [4] | VIDA [5]
```

Ele é difícil de ferir, mas não precisa sustentar um confronto longo quando um ataque capaz realmente o atinge.

A VIDA é definida pela natureza da personagem e pelo papel que ela precisa sustentar na história. A Importância pode orientar esse valor, mas não o calcula automaticamente.

Referências úteis, sem formar uma lista fechada:

```text
VIDA [5]  → minion, figurante ou criatura que pode cair após pouco dano relevante
VIDA [10] → figurante resistente ou ameaça menor
VIDA [15] → elite ou ameaça secundária
VIDA [20] → personagem capaz de sustentar um confronto relevante
VIDA [35] → referência comum de herói, protagonista ou vilão central
VIDA [50+] → entidade, chefe excepcional ou ameaça de durabilidade extraordinária
```

Valores intermediários ou superiores são válidos quando fizerem sentido. `25`, `30`, `40`, `50`, `60` ou qualquer outro valor não precisam de uma categoria especial para existir.

Um personagem muito poderoso pode possuir VIDA baixa se sua função não exigir grande duração em cena; uma entidade central pode possuir VIDA muito acima de 35.

> **RES mede resistência ao dano. VIDA mede quanto dano relevante pode ser acumulado. Poder bruto e duração narrativa não são a mesma coisa.**

### ENERGIA

`ENERGIA` mostra a reserva máxima final da personagem. Por padrão, ela é calculada pelo maior Atributo conforme `../resolucao/energia.md`.

Uma exceção aprovada para uma personagem pode alterar seu valor final e deve ser registrada na própria ficha. Isso não cria uma diretriz geral para as demais personagens.

Os valores atuais continuam no STATUS. Exemplo:

```text
Ficha → VIDA [35] | ENERGIA [80]
STATUS → Dano [12/35] | Energia [53/80]
```

Depois da aprovação dos Atributos no Bloco 2, registrar `VIDA` e `ENERGIA` na ficha conforme as regras aplicáveis à personagem. ENERGIA normalmente é derivada dos Atributos; VIDA é escolhida como referência de durabilidade conforme natureza e função narrativa.

> **A ficha mostra a capacidade de referência. O STATUS mostra a condição atual.**

## IMPORTÂNCIA

`IMPORTÂNCIA` indica o peso estrutural do personagem para a história.

Ela **não determina `CONTROLE`** e não impõe quantidade máxima universal de personagens em nenhuma categoria.

Ela também não determina automaticamente:

- tamanho da ficha;
- quantidade obrigatória de informações;
- atributos;
- perícias;
- poderes;
- dificuldade;
- proteção narrativa.

A Importância pode, porém, orientar a VIDA quando a duração esperada da personagem em confronto faz parte de sua função narrativa. Isso não cria uma fórmula rígida: a VIDA final continua sendo um valor explícito da ficha.

As categorias são:

```text
Importância: Central
Importância: Relevante
Importância: Figurante
```

### Central

É parte do núcleo estrutural da campanha.

Uma campanha pode possuir quantos personagens Centrais forem realmente definidos como parte desse núcleo.

Um personagem Central pode usar qualquer categoria de `CONTROLE` aprovada para aquela peça.

### Relevante

É um personagem estruturalmente importante para a campanha, mas que não pertence ao núcleo central.

Um personagem Relevante pode usar qualquer categoria de `CONTROLE` aprovada para aquela peça.

> **Ser Relevante não determina quem controla o personagem.**

### Figurante

É um personagem sem papel estrutural central ou relevante para a campanha naquele momento.

A frequência de aparição não altera essa classificação. Um entregador, guarda, comerciante ou outro personagem pode aparecer repetidamente durante toda a campanha e continuar Figurante.

`IMPORTÂNCIA` por si só não determina `CONTROLE`.

### Importância é quase fixa

IMPORTÂNCIA representa função estrutural na campanha e não deve subir ou descer apenas porque um personagem apareceu mais vezes ou ganhou momentaneamente destaque.

Se surgir proposta de mudar a Importância de um personagem, ela deve ser apresentada ao JOGADOR HUMANO antes da alteração.

Sem aprovação, a classificação permanece como está.

Uma mudança aprovada de Importância não altera automaticamente nenhuma outra parte da ficha, inclusive `CONTROLE`, atributos, perícias, poderes, recursos ou VIDA. Se a função narrativa também justificar alteração de VIDA, essa mudança deve ser tratada separadamente.

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

`CONTROLE` é independente de `IMPORTÂNCIA`.

> **IMPORTÂNCIA diz qual é o peso estrutural da peça. CONTROLE diz quem toma suas decisões. Uma informação não determina automaticamente a outra.**

### JOGADOR HUMANO

É o personagem cujas decisões voluntárias pertencem ao jogador humano.

Sua Importância é definida separadamente.

### JOGADOR IA

É um personagem com uma IA dedicada exclusivamente a ele. É apropriado quando sua agência individual precisa ser preservada continuamente.

Sua Importância é definida separadamente.

### JOGADOR IA EVENTUAL

É uma categoria de controle possível para qualquer personagem cuja agência eventual tenha sido definida dessa forma.

Uma mesma IA EVENTUAL pode assumir simultaneamente todos os personagens dessa categoria que precisarem de agência própria naquela situação.

A categoria precisa estar registrada na ficha conforme as regras operacionais da campanha.

Sua Importância é definida separadamente.

### NPC

É personagem de uso normal do NARRADOR.

A categoria `NPC` também não define Importância: um NPC pode ser Figurante, Relevante ou Central se a estrutura da campanha assim estabelecer.

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

Durante a criação inicial, porém, o arquivo nasce com este modelo completo; somente depois da revisão campos comprovadamente inúteis podem ser removidos.

```text
# Nome

Status: PENDENTE DE REVISÃO
Importância: ...
CONTROLE: ...

Nome real:
Idade:
Aparência:
Estilo:
Conceito:
Descrição:

TRAÇOS:

ATR: FIS [ ] | RES [ ] | MEN [ ] | VON [ ]
VIDA [ ] | ENERGIA [ ]
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

Na ficha recém-criada, somente Nome, Importância e CONTROLE recebem conteúdo. Os demais campos permanecem vazios.

No **Bloco 1 — Identidade e conceito**, `Nome real`, `Idade`, `Aparência` e `Estilo` são tratados junto com origem, natureza e conceito para que a personagem fique concreta e reconhecível antes da revisão mecânica.

No **Bloco 2 — Atributos e perícias**, depois da aprovação dos Atributos, `VIDA` e `ENERGIA` são preenchidas como referências de consulta rápida conforme as regras aplicáveis à personagem.

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