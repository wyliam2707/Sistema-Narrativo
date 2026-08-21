# Ficha de Personagem

Status: EM REVISÃO

A ficha é o **dossiê consolidado do personagem**: registra quem ele é, o que consegue fazer e as informações que precisam permanecer disponíveis para interpretação e continuidade.

Ela não precisa ser curta. Precisa ser organizada e conter apenas informação útil para decisão, interpretação, capacidade ou continuidade.

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

Personagens Centrais ou controlados por IA podem possuir blocos narrativos extensos quando isso for necessário para manter interpretação e continuidade consistentes.

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

## CONTROLE

A ficha pode registrar:

```text
CONTROLE: JOGADOR HUMANO
CONTROLE: JOGADOR IA
CONTROLE: JOGADOR IA EVENTUAL
CONTROLE: NPC
```

`CONTROLE` é metadado estrutural e não atributo mecânico.

Ele informa como o personagem participa do ciclo e quem possui autoridade normal para suas decisões.

### JOGADOR HUMANO

É o personagem do jogador humano.

### JOGADOR IA

É um personagem com uma IA dedicada exclusivamente a ele. É apropriado para coprotagonistas, parceiros românticos ou personagens cuja agência individual precisa ser preservada de forma contínua.

### JOGADOR IA EVENTUAL

É um personagem que pode receber agência própria quando for importante para a campanha. Uma mesma IA eventual pode controlar simultaneamente todos os personagens eventuais ativos.

### NPC

É um personagem de uso normal do NARRADOR. Inclui figurantes, civis, monstros, inimigos, criaturas e demais personagens sem jogador próprio.

### OPOSITOR não é um tipo de CONTROLE

O OPOSITOR não possui uma categoria permanente de personagens.

Sua função é propor problemas e apresentar oposição.

Ele pode sugerir a entrada de NPCs, forças, ameaças ou outros elementos capazes de produzir oposição. O NARRADOR julga se essa proposta é válida e coerente com a ficção.

Se aprovada, o NARRADOR pode disponibilizar esses elementos ao OPOSITOR para uso naquela oposição.

Exemplo:

```text
OPOSITOR:
Trigon envia dois assassinos.

NARRADOR:
Julga se Trigon pode fazer isso e se a entrada desses assassinos é coerente.

Se aprovado:
Os assassinos podem ser usados pelo OPOSITOR na oposição da cena.
```

Os assassinos continuam sendo `NPC`; não passam a ter `CONTROLE: OPOSITOR`.

As regras operacionais dessas categorias pertencem a `../personas/` e ao ciclo do sistema. Esta área apenas registra o valor aprovado na ficha.

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

Exemplo:

```text
Castelo dos Corvos => Forja antiga, Biblioteca imensa, Laboratório de alquimia, Sala de tango, Sala de treino, Solar, 5 quartos
```

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

## Estrutura recomendada — personagem Central

```text
# Nome

Status: PENDENTE DE REVISÃO
Importância: Central
CONTROLE: ...

Idade:
Conceito:
Descrição:

TRAÇOS:
- ...

ATR: FOR [ ] | AGI [ ] | RES [ ] | MEN [ ] | VON [ ]
PER:
PODERES:
- Poder [Fonte opcional] [ ] => uso / uso / especialização [ ]
RECURSOS:
REL:

## Personalidade e tendências
- ...

## Desejos/objetivos atuais
- ...

## Medos/limites relevantes
- ...

## Conhecimento atual relevante
- ...

## História consolidada relevante
- somente fatos necessários para interpretar o personagem e preservar continuidade
```

Uma ficha Central pode ser extensa porque precisa sustentar agência e continuidade por muito tempo.

## Estrutura recomendada — personagem Relevante

```text
# Nome

Status: PENDENTE DE REVISÃO
Importância: Relevante
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

## Desejos/objetivos atuais
- ...

## Medos/limites relevantes
- ...

## Conhecimento atual relevante
- ...

## História consolidada relevante
- ...
```

A ficha Relevante pode ser mais curta quando menos informação for necessária para interpretá-la corretamente.

Se um campo não possui utilidade real, ele pode permanecer vazio.

## Ficha reservada de antagonista importante

Quando um antagonista importante precisa de continuidade sem revelar suas capacidades ao jogador, pode usar a mesma linguagem de ficha em área reservada da aventura.

Modelo:

```text
# Nome

Status: CANÔNICO DO MESTRE
Visibilidade: MESTRE
Importância: Relevante | Central

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

## Desejos/objetivos atuais
- ...

## Medos/limites relevantes
- ...

## Conhecimento atual relevante
- ...

## História consolidada relevante
- ...

## Segredos ainda não descobertos
- ...
```

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

Fichas reservadas do Narrador usam seu próprio estado canônico e não passam por aprovação aberta quando isso revelaria segredos.

## Alterações posteriores

A ficha não recebe XP ou melhorias automáticas por missão ou capítulo.

Se a ficção alterar de verdade o personagem — por transformação permanente, aquisição real de uma capacidade, perda estrutural, mudança estável de identidade ou equivalente — a parte mecânica da ficha pode ser atualizada para representar a nova realidade.

As partes narrativas da ficha também podem ser atualizadas quando novos objetivos, conhecimentos, relações, limites ou fatos consolidados passarem a ser necessários para interpretar corretamente o personagem.

> **A ficha acompanha quem o personagem é e o que precisa ser lembrado para interpretá-lo corretamente.**

O procedimento de atualização e persistência pertence a `../persistencia/`.
