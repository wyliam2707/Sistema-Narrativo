# Atributos

Status: APROVADO

A ficha usa quatro atributos universais.

Cada atributo descreve uma capacidade diferente do personagem. Eles não são somados automaticamente entre si, com perícias, poderes ou equipamentos.

Os atributos usam a escala universal definida em `escala.md`.

A ficha não busca equilibrar personagens entre si. O valor de um Atributo deve refletir aquilo que o personagem realmente é.

---

## 1. Atributos básicos

### FIS — Físico

**FIS mede aquilo que o corpo do personagem consegue fazer.**

Reúne potência, velocidade, coordenação, precisão corporal, equilíbrio e capacidade de reação física.

Inclui, quando pertinente:

- levantar peso;
- empurrar e puxar;
- arrombar;
- agarrar ou conter alguém fisicamente;
- correr, saltar e escalar;
- esquivar;
- manter equilíbrio;
- executar movimentos rápidos;
- reagir fisicamente a algo percebido;
- realizar movimentos delicados ou precisos;
- aplicar potência em golpes produzidos pelo próprio corpo.

FIS não mede percepção. Perceber uma ameaça, detalhe ou mudança no ambiente pertence normalmente a MEN. FIS pode determinar a qualidade, velocidade ou precisão da resposta corporal depois que a situação foi percebida.

FIS também não mede quanto dano, esforço ou impacto o corpo consegue suportar. Isso pertence a RES.

> **FIS age. RES suporta.**

---

### RES — Resistência

**RES mede quanto o corpo consegue suportar antes de falhar.**

Inclui, quando pertinente:

- dano e impacto;
- dor física;
- esforço prolongado;
- fôlego e exaustão;
- privação física;
- ambientes hostis;
- venenos;
- doenças;
- toxinas;
- capacidade de continuar funcionando apesar de desgaste físico.

FIS e RES são independentes.

Um personagem pode possuir capacidade física extrema e baixa resistência, ou grande resistência e pouca capacidade de ação corporal.

---

### MEN — Mente

**MEN mede a capacidade de perceber, compreender, analisar e processar informações.**

Inclui, quando pertinente:

- percepção;
- atenção;
- raciocínio;
- memória;
- análise;
- cálculo;
- dedução;
- leitura de situação;
- antecipação;
- aprendizado;
- interpretação de informações;
- precisão mental na execução de efeitos quando a natureza da ação depender disso.

MEN não mede força de vontade nem resistência mental. Essas funções pertencem a VON.

MEN também não representa conhecimento universal.

MEN alto pode permitir compreender, relacionar e aprender informações com grande eficiência, mas não concede automaticamente repertório nunca adquirido.

MEN não concede por si só:

- formação médica;
- conhecimento ocultista;
- idiomas nunca aprendidos;
- fatos nunca conhecidos;
- informação secreta;
- conhecimento exclusivo do Narrador.

> **MEN ajuda a construir caminhos de entendimento; não substitui repertório especializado nem cria informação inexistente.**

---

### VON — Vontade

**VON mede determinação, resistência mental e capacidade de sustentar uma ação, efeito ou intenção sob pressão.**

Inclui, quando pertinente:

- resistir a medo;
- resistir a coerção ou dominação;
- resistir a controle mental;
- permanecer funcional sob pressão psicológica;
- perseverar apesar de desgaste emocional;
- manter concentração;
- sustentar poderes ou efeitos prolongados;
- impor um efeito quando sua natureza depender diretamente de força de vontade.

Como princípio geral:

```text
MEN → perceber, compreender, calcular, conjurar, mirar ou controlar com precisão mental.
VON → resistir, sustentar, manter, perseverar ou impor pela determinação.
```

A natureza concreta da ação continua sendo mais importante do que uma associação automática.

---

## 2. Defesa não pertence a um único atributo

O sistema não possui um atributo universal de defesa.

A capacidade usada para se defender depende de como a defesa acontece na ficção.

Exemplos possíveis:

- evitar fisicamente um ataque percebido: FIS;
- antecipar um adversário por leitura, percepção ou raciocínio: MEN;
- bloquear, agarrar ou conter algo fisicamente: FIS, quando fizer sentido;
- suportar o impacto em vez de evitá-lo: RES;
- resistir a dominação, medo ou pressão mental: VON;
- perceber ou evitar algo por uma capacidade extraordinária: poder apropriado.

Mais de uma informação da ficha pode ser relevante para explicar uma defesa, mas isso não cria soma automática entre atributos.

As regras completas de defesa e resolução pertencem a `../resolucao/`.

---

## 3. Não existe atributo universal de Poder

A potência de uma capacidade sobrenatural, tecnológica ou especial é registrada no próprio poder.

Exemplo:

```text
Magia [3]
```

Não existe necessidade de um atributo separado chamado `Poder`.

---

## 4. CONTROLE não é atributo

`CONTROLE` é metadado estrutural da ficha.

Ele indica qual papel possui autoridade sobre as decisões voluntárias do personagem.

Seu significado operacional pertence a `../personas/`.

---

## 5. Potência, fonte e execução são coisas diferentes

O valor usado para produzir um efeito vem da fonte que realmente o produz.

O corpo pode ser essa fonte. Um equipamento, Poder ou outra capacidade também pode ser.

Exemplos:

```text
FIS [2] → golpe corporal usa potência física [2]
Pistola — Dano [1] → o disparo usa Dano [1]
Espada Mágica — Dano [3] → o golpe da espada usa Dano [3]
```

Esses valores não são somados automaticamente:

`FIS [2] + Pistola [1] ≠ Dano [3]`

`FIS [2] + Espada Mágica [3] ≠ Dano [5]`

FIS continua podendo ser relevante para posição, agarrões, deslocamento, velocidade, precisão corporal ou outras disputas físicas durante a mesma cena, sem aumentar automaticamente a potência do equipamento.

A Perícia aplicável descreve quão bem aquela fonte é utilizada. Ela também não se transforma automaticamente em potência adicional da arma ou do Poder.

> **FIS determina o que o corpo consegue produzir. Equipamento determina o que o equipamento consegue produzir. Perícia determina quão bem a fonte escolhida é aplicada.**

---

## 6. Capacidades naturais

Uma capacidade permanente ou natural deve aparecer diretamente no atributo sempre que fizer sentido.

Exemplo:

```text
FIS [4]
```

Isso já representa uma capacidade física natural extraordinária. Não é necessário criar separadamente `Superforça`, `Superagilidade` ou equivalentes apenas para repetir aquilo que FIS já descreve.

Em contraste, uma capacidade que precisa ser ativada deve aparecer como Poder.

Exemplo:

```text
FIS [0]
Magia [3] => Ampliação física
```

Nesse caso, o personagem possui capacidade física humana em repouso e pode usar uma capacidade ativa para alterá-la temporariamente quando o repertório permitir.

---

## 7. Princípio de leitura

Os quatro atributos respondem a perguntas diferentes:

```text
FIS → o que o corpo consegue fazer?
RES → quanto o corpo consegue suportar?
MEN → o que consegue perceber, compreender e processar?
VON → quanto consegue resistir, sustentar e perseverar?
```

Nenhum atributo substitui automaticamente outro apenas porque pode contribuir para a mesma cena.

> **A ficha descreve o personagem; não oferece justiça entre personagens.**
