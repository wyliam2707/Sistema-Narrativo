# Ficha de Personagem

Status: EM REVISÃO

A ficha permanente registra **quem o personagem é e quais capacidades estáveis possui**.

Ela deve permanecer curta e conter apenas informação útil para decisão, interpretação e continuidade.

## Ficha não é STATUS

A ficha permanente guarda, quando relevantes:

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
- equipamento recorrente importante;
- relações recorrentes;
- personalidade;
- objetivos;
- medos e limites;
- história consolidada necessária à interpretação.

Não pertencem à ficha permanente apenas por estarem ativos agora:

- VIDA atual;
- ENERGIA atual;
- condições temporárias;
- efeitos ativos;
- localização;
- ferimentos transitórios;
- dano temporário de equipamento;
- favores circunstanciais;
- acessos;
- consequências latentes que não fazem parte da identidade estável.

Esses elementos pertencem ao STATUS ou a outras camadas de persistência.

> **Ficha = quem ele é. STATUS = como ele está agora.**

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

Ele informa qual papel possui autoridade de decisão sobre o personagem.

As regras operacionais dessas categorias pertencem a `../personas/` e ao ciclo do sistema. Esta área apenas registra o valor aprovado na ficha.

## Equipamento recorrente

Equipamento recorrente ou importante pode aparecer em:

```text
EQP: armadura balística / espada encantada / kit médico / lançador de teia
```

Não transformar a ficha em inventário.

> **Equipamento recorrente/importante entra na ficha. Equipamento circunstancial pode existir apenas na narrativa ou no STATUS quando precisar ser acompanhado.**

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
Poder [Fonte opcional] [ ] => uso / uso / especialização [ ]
Poder [ ] => ...
EQP:
REL:

## Personalidade e tendências
- ...

## Desejos/objetivos atuais
- ...

## Medos/limites relevantes
- ...

## História consolidada relevante
- somente fatos necessários para interpretar o personagem
```

Uma ficha Central pode ser mais descritiva porque precisa sustentar agência e continuidade por muito tempo.

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
Poder [ ] => ...
EQP:
REL:

## Personalidade e tendências
- ...

## Desejos/objetivos atuais
- ...

## Medos/limites relevantes
- ...

## História consolidada relevante
- ...
```

A ficha Relevante pode ser mais curta.

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
Poder [ ] => ...
EQP:
REL:

## Personalidade e tendências
- ...

## Desejos/objetivos atuais
- ...

## Medos/limites relevantes
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

Se a ficção alterar de verdade o personagem — por transformação permanente, aquisição real de uma capacidade, perda estrutural, mudança estável de identidade ou equivalente — a ficha pode ser atualizada para representar a nova realidade.

> **A ficha muda quando o personagem mudou.**

O procedimento de atualização e persistência pertence a `../persistencia/`.
