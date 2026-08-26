# Ficha de Personagem

Status: APROVADO

A ficha é o **dossiê consolidado do personagem**: registra quem ele é, o que consegue fazer e as informações que precisam permanecer disponíveis para interpretação e continuidade.

Ela não precisa ser curta. Precisa ser organizada e conter informação útil para decisão, interpretação, capacidade ou continuidade.

---

## Ficha não é STATUS

A ficha pode guardar, quando relevantes:

- identidade;
- nome real;
- Importância;
- `CONTROLE`;
- idade;
- aparência;
- estilo;
- Conceito;
- descrição;
- Patamar;
- TRAÇOS;
- Atributos permanentes;
- Vida Máxima;
- Mana Máxima;
- Perícias;
- Poderes;
- RECURSOS;
- relações recorrentes;
- personalidade e tendências;
- desejos e objetivos atuais relevantes;
- medos e limites;
- conhecimento atual relevante;
- história consolidada necessária à interpretação.

Não pertencem à ficha apenas por estarem ativos agora:

- Vida atual;
- Mana atual;
- Dano sofrido no momento;
- condições temporárias;
- Status e efeitos ativos;
- alterações temporárias de Atributo;
- Barreiras atuais;
- localização atual;
- ferimentos transitórios;
- favores circunstanciais;
- consequências latentes ainda não incorporadas ao personagem;
- demais informações puramente operacionais do momento.

Esses elementos pertencem ao STATUS ou a outras camadas de persistência.

> **Ficha = dossiê consolidado do personagem. STATUS = como ele está agora.**

A diferença principal não é entre “permanente” e “atual”, mas entre **informação consolidada necessária para interpretar o personagem** e **estado circunstancial da cena ou campanha**.

Vida Máxima e Mana Máxima podem aparecer diretamente na ficha para acelerar consulta. Os valores atuais pertencem ao STATUS.

---

## Organização visual

A ficha apresenta primeiro identidade e informações mecânicas de consulta rápida.

Informações extensas de interpretação e continuidade ficam abaixo, em seções próprias.

Ordem recomendada:

```text
# Nome

Status:
Importância:
CONTROLE:
Patamar: [ ]

Nome real:
Idade:
Aparência:
Estilo:
Conceito:
Descrição:

TRAÇOS:
ATR:
  Corpo  → Potência [ ] | Controle [ ] | Resistência [ ]
  Mente  → Intelecto [ ] | Presença [ ] | Vontade [ ]
Vida Máxima [ ] | Mana Máxima [ ]
PERÍCIAS:
PODERES:
RECURSOS:
REL:

## Personalidade e tendências
## Desejos / objetivos atuais
## Medos / limites relevantes
## Conhecimento atual relevante
## História consolidada relevante
```

Essa ordem é uma referência estética. **Qualquer personagem pode ter uma ficha de qualquer tamanho ou formato**, independentemente de sua Importância.

Um Figurante pode possuir uma ficha extensa se isso for útil. Um Relevante pode ter poucas linhas se isso for suficiente.

---

## Identidade visual padrão

O modelo-base separa informações que não devem ser confundidas:

```text
Nome real → identidade pessoal/civil quando diferente do nome de uso
Aparência → como o personagem é fisicamente reconhecido
Estilo → como costuma se apresentar visualmente
Conceito → síntese do que o personagem é
Descrição → presença e impressão geral útil à interpretação
```

`Aparência:` registra elementos físicos que ajudam a reconhecer a pessoa em cena.

`Estilo:` registra sua apresentação habitual, como roupas, cores, acessórios, uniforme, armadura, maquiagem ou símbolos recorrentes.

A ficha não precisa virar catálogo de medidas. O objetivo é permitir que o personagem seja **reconhecível e descrito de forma consistente quando entrar em cena**.

---

## Nascimento da ficha

Ao criar uma nova ficha apresentável ao jogador, usar desde o início o modelo-base completo definido neste arquivo.

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

Todos os demais campos já devem existir no arquivo, mas permanecem vazios até serem tratados no bloco correspondente da revisão.

Não preencher antecipadamente Patamar, Atributos, Vida, Mana, Perícias, Poderes, Traços, recursos, relações ou informações narrativas apenas para completar a ficha.

```text
NOME + IMPORTÂNCIA + CONTROLE
→ criar modelo-base completo
→ deixar demais campos vazios
→ iniciar revisão
```

> **A ficha nasce completa em estrutura e mínima em conteúdo.**

---

## Campo desconhecido fica em branco

Durante criação ou revisão, não usar zero para significar “ainda não definido”.

```text
Potência [ ]
Controle [ ]
Resistência [ ]
Intelecto [ ]
Presença [ ]
Vontade [ ]
```

é diferente de:

```text
Potência [0]
Controle [0]
Resistência [0]
Intelecto [0]
Presença [0]
Vontade [0]
```

No segundo caso, os valores já foram mecanicamente definidos.

> **Zero é valor real, nunca marcador de pendência.**

O mesmo princípio vale para informação omitida em fichas rápidas: ausência de campo não significa valor zero.

---

## Patamar

A ficha registra:

```text
Patamar: [X]
```

Patamar varia de `[1]` a `[7]` e representa desenvolvimento mecânico geral.

Sua regra completa pertence a `patamar.md`.

Patamar organiza limites e quantidades de criação e fornece o valor `[X]` usado pelos Poderes.

> **Patamar não mede Importância narrativa e não altera a Dificuldade do cenário.**

---

## Atributos

A ficha completa registra os seis Atributos:

```text
CORPO
Potência [ ]
Controle [ ]
Resistência [ ]

MENTE
Intelecto [ ]
Presença [ ]
Vontade [ ]
```

A escala permanente normal é `[-2]` a `[7]`.

A regra completa pertence a `atributos.md`.

`Controle` como Atributo corporal não deve ser confundido com `CONTROLE`, o metadado estrutural de agência.

---

## Perícias

Perícias são registradas apenas pelo nome.

Exemplo:

```text
PERÍCIAS:
- Medicina
- Investigar
- Ocultismo
```

Perícias não possuem graduação `[+0]` a `[+5]`.

Quando uma Perícia for realmente relevante para uma resolução, concede `+1d` conforme `pericias.md` e `../resolucao/`.

Várias Perícias aplicáveis ao mesmo teste continuam concedendo no máximo `+1d` por Perícias.

---

## Poderes

Poderes representam partes do arsenal funcional do personagem.

Eles não usam uma escala genérica `[1]` a `[5]`.

A ficha registra quais Poderes o personagem possui; funcionamento, Hub, custo, alcance, Dano, Efeito e outras opções pertencem às regras específicas dos Poderes.

Exemplo estrutural:

```text
PODERES:
- Teleporte
- Proteção
- Ilusão
```

Quando uma regra de Poder usar `[X]`:

> **[X] = Patamar do personagem**

---

## Vida Máxima e Mana Máxima

Para consulta rápida, a ficha registra:

```text
Vida Máxima [X] | Mana Máxima [Y]
```

Os valores são derivados dos Atributos permanentes.

### Vida Máxima

A fórmula canônica pertence a `../resolucao/vida.md`:

> **Vida = 10 + (Resistência ×4) + (Potência ×2) + (Controle ×2) + Intelecto + Presença + Vontade**

Para Vida, Atributos negativos contam como `0`.

Vida não é escolhida de acordo com protagonismo, Importância ou duração desejada de confronto.

Uma mudança permanente nos Atributos recalcula a Vida Máxima. Alterações temporárias não recalculam.

### Mana Máxima

A fórmula canônica pertence a `../resolucao/mana.md`:

> **Mana = 10 + 2 × (Potência + Controle + Resistência + Intelecto + Presença + Vontade)**

Para Mana, Atributos negativos contam normalmente.

Uma mudança permanente nos Atributos recalcula a Mana Máxima. Alterações temporárias não recalculam.

### Valores atuais

A ficha registra os máximos; o STATUS registra os atuais.

Exemplo:

```text
FICHA
Vida Máxima [29] | Mana Máxima [24]

STATUS
Vida [18/29] | Mana [9/24]
```

> **A ficha mostra a capacidade de referência. O STATUS mostra a condição atual.**

---

## IMPORTÂNCIA

`IMPORTÂNCIA` indica o peso estrutural do personagem para a história.

Ela **não determina `CONTROLE`** e não impõe quantidade máxima universal de personagens em nenhuma categoria.

Ela também não determina automaticamente:

- tamanho da ficha;
- Patamar;
- Atributos;
- Perícias;
- Poderes;
- Traços;
- Vida;
- Mana;
- Dificuldade;
- proteção narrativa.

As categorias são:

```text
Importância: Central
Importância: Relevante
Importância: Figurante
```

### Central

É parte do núcleo estrutural da campanha.

Uma campanha pode possuir quantos personagens Centrais forem realmente definidos como parte desse núcleo.

### Relevante

É um personagem estruturalmente importante para a campanha, mas que não pertence ao núcleo central.

> **Ser Relevante não determina quem controla o personagem.**

### Figurante

É um personagem sem papel estrutural central ou relevante para a campanha naquele momento.

A frequência de aparição não altera automaticamente essa classificação.

### Importância é quase fixa

IMPORTÂNCIA representa função estrutural na campanha e não deve subir ou descer apenas porque um personagem apareceu mais vezes ou ganhou momentaneamente destaque.

Se surgir proposta de mudar a Importância, ela deve ser apresentada ao JOGADOR HUMANO antes da alteração.

Sem aprovação, a classificação permanece como está.

Uma mudança aprovada de Importância não altera automaticamente `CONTROLE`, Patamar, Atributos, Perícias, Poderes, Traços, Vida, Mana ou recursos.

> **Na dúvida, manter a classificação atual.**

---

## CONTROLE

A ficha pode registrar:

```text
CONTROLE: JOGADOR HUMANO
CONTROLE: JOGADOR IA
CONTROLE: JOGADOR IA EVENTUAL
CONTROLE: NPC
```

`CONTROLE` é metadado estrutural e não Atributo mecânico.

Ele informa como a personagem participa normalmente do ciclo. Nas peças com jogador dedicado, também indica quem possui autoridade usual sobre suas decisões.

`CONTROLE` é independente de `IMPORTÂNCIA` e de Patamar.

> **IMPORTÂNCIA diz qual é o peso estrutural da peça. CONTROLE diz como sua agência é atribuída. Uma informação não determina automaticamente a outra.**

### JOGADOR HUMANO

As decisões voluntárias pertencem ao jogador humano.

### JOGADOR IA

A personagem possui uma IA dedicada à sua agência contínua.

### JOGADOR IA EVENTUAL

A personagem pode receber agência da persona eventual conforme as regras de `../personas/`.

### NPC

É uma personagem sem jogador dedicado.

```text
ROTINA EVIDENTE
→ NARRADOR pode narrar como consequência já determinada

DECISÃO VOLUNTÁRIA RELEVANTE, NÃO ADVERSARIAL
→ JOGADOR IA EVENTUAL assume temporariamente

OPOSIÇÃO ATIVA
→ NPC pode ser delegado ao OPOSITOR depois do julgamento de disponibilidade
```

A assunção temporária não muda o `CONTROLE` da ficha.

As regras completas pertencem a `../personas/`.

---

## OPOSITOR não é tipo de CONTROLE

O OPOSITOR não possui categoria permanente de personagem.

Sua função é gerar problemas e apresentar oposição legítima conforme `../personas/`.

NPCs podem ser delegados temporariamente ao OPOSITOR quando a ficção e a disponibilidade permitirem, sem alterar o `CONTROLE` registrado na ficha.

> **O OPOSITOR joga a oposição legitimamente delegada. O NARRADOR julga.**

---

## RECURSOS

`RECURSOS` registra o mínimo necessário sobre meios, infraestrutura, instalações, organizações, objetos únicos ou preparações específicas já estabelecidas e capazes de alterar possibilidades na ficção.

Não é inventário e não é catálogo de patrimônio.

Um recurso só precisa ser registrado quando sua existência, ausência ou estado puder ser útil para decisões futuras.

Exemplo:

```text
RECURSOS:
Castelo dos Corvos => Forja antiga, Biblioteca, Laboratório
Chave do Cofre [perdida]
Fórmula experimental [uso único]
```

RECURSOS não possuem Patamar por padrão e não concedem bônus automáticos.

Eles estabelecem meios, infraestrutura, acesso e possibilidades concretas.

A ausência de um meio necessário pode ser relevante para a resolução.

> **RECURSOS registram apenas o que foi efetivamente estabelecido e pode ser útil depois.**

---

## REL e relações recorrentes

`REL` registra relações que precisam permanecer disponíveis para interpretação e continuidade.

A regra detalhada pertence a `relacoes.md` e `pareamento.md`.

Relação não é bônus mecânico automático. Ela pode alterar possibilidades, informação, disposição e contexto quando a ficção realmente tornar isso relevante.

---

## Modelo-base de ficha

O sistema não exige modelos diferentes para Central, Relevante ou Figurante.

Durante a criação inicial, porém, a ficha apresentável ao jogador nasce com este modelo completo; somente depois da revisão campos comprovadamente inúteis podem ser removidos.

```text
# Nome

Status: PENDENTE DE REVISÃO
Importância: ...
CONTROLE: ...
Patamar: [ ]

Nome real:
Idade:
Aparência:
Estilo:
Conceito:
Descrição:

TRAÇOS:

ATR:
Corpo  → Potência [ ] | Controle [ ] | Resistência [ ]
Mente  → Intelecto [ ] | Presença [ ] | Vontade [ ]

Vida Máxima [ ] | Mana Máxima [ ]

PERÍCIAS:
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

No **Bloco 1 — Identidade e conceito**, tratar identidade, aparência e Conceito.

No **Bloco 2 — Atributos e Perícias**, definir Patamar quando necessário à construção mecânica, distribuir Atributos conforme `patamar.md` e registrar Perícias reais.

Depois dos Atributos permanentes estarem fechados, calcular Vida Máxima e Mana Máxima automaticamente pelas regras de `../resolucao/vida.md` e `../resolucao/mana.md`.

No **Bloco 3 — Poderes e capacidades**, registrar o arsenal funcional e suas capacidades realmente possuídas.

No **Bloco 4 — Traços e relações**, registrar apenas verdades estáveis e vínculos relevantes.

---

## Fichas rápidas e mínimas

Todos os personagens usam as mesmas regras, mas nem todos precisam registrar a mesma quantidade de informação.

Uma ficha rápida ou mínima pode omitir campos que ainda não sejam necessários.

> **Informação ausente não significa valor zero.**

Quando Vida Máxima ou Mana Máxima precisarem ser acompanhadas, seus valores podem ser registrados diretamente na ficha compacta como resultados derivados, mesmo que Atributos não relevantes naquele momento tenham sido omitidos visualmente.

Isso não altera as regras de construção do personagem; apenas reduz o que precisa ser exibido e persistido.

---

## Informação reservada do NARRADOR

Quando uma ficha do mundo precisar guardar uma verdade que não pode ser apresentada ao jogador, ela pode incluir:

```text
## Informação reservada do NARRADOR
- identidade oculta;
- plano ainda não descoberto;
- conhecimento secreto;
- pacto desconhecido;
- capacidade ou limitação ainda não revelada;
- outro fato consolidado que precise permanecer secreto.
```

Essa seção é opcional e só deve existir quando houver informação realmente estabelecida que precise ser preservada em sigilo.

Ela não autoriza criar fatos retroativamente para contrariar uma ação válida, restaurar dificuldade ou proteger a trama.

> **Informação pode ser secreta. A realidade da campanha não pode ser criada retroativamente apenas para impedir uma solução válida.**

---

## Ficha reservada

Quando um personagem precisa de continuidade sem revelar suas capacidades ou segredos ao jogador, pode usar a mesma linguagem de ficha em uma área reservada da campanha.

A ficha reservada preserva segredo; não autoriza alterar capacidades retroativamente.

---

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

---

## Alterações posteriores

A ficha não recebe XP ou melhorias automáticas por missão ou capítulo apenas por passagem narrativa.

Se a ficção alterar de verdade o personagem — por transformação permanente, aquisição real de capacidade, perda estrutural, mudança estável de identidade ou equivalente — a parte mecânica pode ser atualizada para representar a nova realidade conforme as regras de progressão vigentes.

Mudanças permanentes de Atributo recalculam Vida Máxima e Mana Máxima.

As partes narrativas também podem ser atualizadas quando novos objetivos, conhecimentos, relações, limites ou fatos consolidados passarem a ser necessários para interpretar corretamente o personagem.

> **A ficha acompanha quem o personagem é e o que precisa ser lembrado para interpretá-lo corretamente.**

## Regra final

> **A ficha guarda identidade, capacidade consolidada e continuidade. Patamar, seis Atributos, Perícias sem graduação, Poderes por arsenal funcional, Vida Máxima e Mana Máxima formam sua base mecânica atual; estado momentâneo continua pertencendo ao STATUS.**
