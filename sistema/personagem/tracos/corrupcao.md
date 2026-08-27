# Corrupção

Status: APROVADO

Corrupções são **Traços negativos sobrenaturais**. Elas representam fraquezas, vulnerabilidades, necessidades e regras extraordinárias que fazem parte da natureza da personagem.

Uma Corrupção não precisa ser ativada. Ela já é verdadeira e passa a importar quando sua condição aparece na ficção.

> **Corrupção estabelece uma limitação sobrenatural real. Ela pode modificar uma resolução, causar consequência automática ou tornar uma ação impossível quando sua própria descrição disser isso.**

O OPOSITOR pode explorar uma Corrupção quando possuir oportunidade e conhecimento legítimos, mas não recebe autoridade para decidir escolhas voluntárias da personagem.

---

## Valor

Toda Corrupção vale:

> **[-1]**

Cada Corrupção fornece **1 ponto negativo de criação**, que pode ser convertido conforme `../patamar.md` em apenas uma destas opções:

- `+1` Traço positivo;
- `+1` Poder.

O mesmo ponto nunca compra as duas coisas.

Não existem Corrupções comuns de `[-2]` no catálogo atual.

O equilíbrio vem da própria definição:

```text
limitação pequena demais
→ ampliar ou unir

limitação ampla demais
→ restringir fonte, gatilho ou consequência

limitação impossível de entrar em jogo
→ não concede ponto negativo
```

> **Uma Corrupção só vale [-1] quando puder realmente complicar a existência da personagem.**

---

## Critério mínimo de validade

Uma Corrupção precisa possuir:

1. **gatilho concreto** — a condição que a coloca em funcionamento;
2. **consequência objetiva** — o que muda quando o gatilho ocorre;
3. **possibilidade plausível de aparecer** — a condição pode realmente surgir na campanha.

Não comprar a mesma limitação várias vezes sob nomes diferentes.

Fontes extremamente amplas como `Físico`, `Mental`, `Magia`, `Elementos` ou `Status` não são válidas como `[X]` em Corrupções que exigem uma fonte específica, salvo regra que diga explicitamente o contrário.

---

## Corrupções e Trama

Quando uma Corrupção oferece uma escolha real e a personagem elegível **aceita voluntariamente** uma complicação evitável causada por ela, pode receber `+1 Trama` conforme `../trama.md`.

Consequência automática, por si só, não significa que houve escolha voluntária.

```text
fonte aparece e causa Dano automaticamente
→ aplicar a Corrupção
→ não pressupõe ganho de Trama

personagem poderia evitar a fonte
mas decide enfrentá-la e aceita a complicação
→ pode existir complicação válida de Trama
```

Pontos de Trama podem reduzir penalidades ou Dano quando sua própria regra permitir, mas não anulam uma impossibilidade absoluta de **Restrição**.

---

# Corrupções

## Fraqueza [X] [-1]

A personagem é especialmente suscetível a uma **fonte específica** registrada em `[X]`.

Exemplos válidos:

```text
Fraqueza [Prata]
Fraqueza [Ferro Frio]
Fraqueza [Água Sagrada]
Fraqueza [Fogo]
Fraqueza [Som Ultrassônico]
```

Quando `[X]` participa diretamente de uma resolução contra a personagem, aplica-se **1 dado de desvantagem ao lado da personagem**:

- se outra peça fizer a rolagem contra ela, essa peça recebe `+1d`;
- se somente a personagem fizer uma rolagem para resistir ou suportar `[X]`, recebe `-1d`;
- nunca aplicar os dois na mesma resolução.

Fraqueza não causa Dano por existir e não dobra consequências.

Categorias excessivamente amplas não são válidas:

```text
Fraqueza [Físico] → inválida
Fraqueza [Mental] → inválida
Fraqueza [Magia]  → inválida
```

### Fraqueza e Imunidade

Se a personagem possuir **Imunidade [X]** e **Fraqueza [X]** exatamente para a mesma fonte, a combinação é inválida.

Uma Fraqueza específica também não transforma automaticamente uma Imunidade diferente em proteção inútil; aplicar literalmente as fontes registradas.

---

## Vulnerabilidade [X] [-1]

A personagem sofre consequência física muito maior quando recebe **Dano de uma fonte específica** registrada em `[X]`.

Exemplos:

```text
Vulnerabilidade [Prata]
Vulnerabilidade [Fogo]
Vulnerabilidade [Eletricidade]
Vulnerabilidade [Sagrado]
Vulnerabilidade [Ácido]
```

Quando Dano de `[X]` alcançaria a personagem, resolver normalmente:

```text
Defesa
→ redução da Defesa
→ RD
→ mínimo aplicável
→ Escudo
```

Depois do Escudo e **antes da janela de Trama**, dobrar o Dano restante.

```text
Dano restante 3
→ Vulnerabilidade aplicável
→ 6 Dano
→ abrir Trama, quando elegível
→ Vida
```

Vulnerabilidade não dobra duração de Status, número de alvos, penalidades ou efeitos narrativos que não sejam Dano, salvo regra específica.

A fonte precisa ser específica. `Vulnerabilidade [Físico]`, `[Magia]`, `[Elementos]`, `[Mental]` ou `[Status]` não é válida como Corrupção padrão.

Não possuir Imunidade e Vulnerabilidade exatamente para a mesma fonte.

---

## Exposição [X] [-1]

A simples exposição direta a uma condição específica causa Dano contínuo.

Exemplos:

```text
Exposição [Luz Solar]
Exposição [Água Sagrada]
Exposição [Ferro Frio]
Exposição [Solo Consagrado]
Exposição [Água Corrente]
```

Em combate, enquanto a exposição direta permanecer:

> **1 Dano por Turno pessoal da personagem afetada**

O primeiro Dano ocorre quando a exposição direta é estabelecida. Se ela continuar, aplica-se novamente no início das VEZES seguintes da personagem enquanto a condição persistir.

Esse Dano é automático e não exige rolagem. Não é reduzido por Defesa, Resistência ou RD comum, salvo regra específica que diga o contrário. Trama ainda pode reduzir Dano quando a janela normal for aplicável.

Fora de combate, não criar Turnos artificiais. Resolver pela duração ficcional da exposição. Quando for realmente necessário acompanhar numericamente uma exposição curta, usar como referência **1 Dano por aproximadamente 10 segundos** de contato contínuo.

A mesma Corrupção não acumula múltiplas instâncias simultâneas da mesma fonte.

---

## Dieta Especial [X] [-1]

A personagem possui uma necessidade sobrenatural de alimentação que comida comum não satisfaz.

Exemplos:

```text
Dieta Especial [Sangue]
Dieta Especial [Energia Vital]
Dieta Especial [Emoções]
Dieta Especial [Carne Crua]
```

Enquanto a necessidade não tiver sido satisfeita desde o último descanso válido:

> **a personagem não recebe a recuperação natural diária de Vida por descanso**

Consumir uma quantidade adequada de `[X]`, conforme a ficção, torna a personagem apta a receber a recuperação no próximo descanso válido. Depois dessa recuperação, a necessidade volta a precisar ser satisfeita para a próxima recuperação natural.

Dieta Especial não causa Dano automaticamente e não obriga consumo.

Para valer `[-1]`, `[X]` precisa criar dificuldade real de obtenção, risco, conflito ou limitação. Uma fonte trivialmente disponível em qualquer lugar não sustenta esta Corrupção.

Se `[X]` for desejo ou hábito, não necessidade sobrenatural, usar **Dependência** em `vicios.md`.

---

## Repulsa [X] [-1]

A presença direta de uma fonte sobrenatural específica enfraquece ou desorganiza a personagem.

Enquanto `[X]` estiver diretamente presente e relevante:

> **-2d nas resoluções diretamente afetadas pela Repulsa**

Exemplos:

```text
Repulsa [Símbolo Sagrado]
Repulsa [Alho]
Repulsa [Sal Ritual]
Repulsa [Luz Solar]
Repulsa [Fogo Aberto]
```

A penalidade não se aplica a ações sem relação real com a presença da fonte.

Repulsa não obriga fuga e não torna uma ação automaticamente impossível.

> **Repulsa dificulta. Restrição proíbe.**

Como `-2d` já alcança o limite universal de penalidade de dados, outras penalidades de dados continuam sujeitas ao teto final do motor.

---

## Restrição [X] [-1]

A personagem está sujeita a uma **regra sobrenatural absoluta e específica** que não consegue violar enquanto a condição registrada for válida.

Quando a Restrição se aplica, não existe teste para simplesmente contrariá-la.

Exemplos válidos:

```text
Restrição [Convite]
→ não consegue atravessar o limiar de residência privada sem convite legítimo

Restrição [Verdade]
→ não consegue afirmar deliberadamente algo que sabe ser falso

Restrição [Água Corrente]
→ não consegue atravessar água corrente por deslocamento próprio

Restrição [Solo Consagrado]
→ não consegue entrar voluntariamente em local verdadeiramente consagrado
```

A Restrição deve bloquear **uma ação ou relação específica**, não uma parte enorme da existência da personagem.

Exemplo amplo demais para uma Corrupção padrão:

```text
Restrição [Luz do Dia]
→ "não consegue fazer nada durante o dia"
→ inválida por abrangência excessiva
```

Para luz solar, usar normalmente **Exposição**, **Repulsa**, **Fraqueza** ou outra Corrupção específica conforme o efeito desejado.

Uma Restrição pode ser contornada quando a própria redação permitir outro método.

```text
não consegue atravessar água corrente por deslocamento próprio
→ Teleporte pode contornar se não existir travessia física
```

---

## Repouso Especial [X] [-1]

A personagem só consegue realizar **descanso válido** quando estiver em uma condição sobrenatural específica registrada em `[X]`.

Exemplos:

```text
Repouso Especial [Caixão]
Repouso Especial [Escuridão Total]
Repouso Especial [Círculo Ritual]
Repouso Especial [Contato com Solo Natal]
```

Fora dessa condição, dormir, permanecer imóvel ou esperar não conta como descanso válido para regras que dependam de repouso.

A condição precisa ser exigente, mas **plausivelmente alcançável ou preparável** durante a campanha.

Uma condição única, remota e praticamente impossível de acessar na maior parte da campanha é ampla demais para a Corrupção padrão de `[-1]` e exige aprovação específica da criação.

Repouso Especial não altera por si só quanto Vida ou Mana é recuperado; ele apenas determina se o descanso é válido.

---

## Âncora [X] [-1]

A estabilidade sobrenatural da personagem depende de um objeto, lugar ou vínculo externo concreto registrado em `[X]`.

Exemplos:

```text
Âncora [Amuleto]
Âncora [Arma Vinculada]
Âncora [Filactério]
Âncora [Coração Oculto]
Âncora [Território]
```

Quando a ligação com a Âncora é destruída, rompida ou perdida de maneira realmente relevante:

1. a personagem perde imediatamente **toda a Mana atual**;
2. não recupera Mana por repouso enquanto a ligação não for restaurada, substituída ou reparada de modo coerente com o Conceito.

Âncora não reduz Vida diretamente.

Para valer `[-1]`, a Âncora precisa existir concretamente, poder ser ameaçada e não estar protegida por uma impossibilidade absoluta de interação.

Perder contato momentâneo sem romper o vínculo não ativa automaticamente a Corrupção, salvo se a descrição registrada disser explicitamente que distância ou separação é o gatilho.

---

# Relação com agência e narrativa

Corrupções não entregam a personagem ao NARRADOR ou ao OPOSITOR.

```text
Dieta Especial [Sangue]
→ necessidade existe
→ a persona decide como lidar com ela

Repulsa [Símbolo Sagrado]
→ penalidade objetiva existe
→ a persona ainda decide sua ação

Restrição [Convite]
→ atravessar o limiar é impossível sem convite
→ a persona decide o que tentar em vez disso
```

O OPOSITOR só pode explorar uma Corrupção usando conhecimento e meios que realmente possua.

Uma Corrupção registrada na ficha não concede automaticamente esse conhecimento a outras personagens.

---

# Lista rápida

```text
Fraqueza [X] [-1]
Vulnerabilidade [X] [-1]
Exposição [X] [-1]
Dieta Especial [X] [-1]
Repulsa [X] [-1]
Restrição [X] [-1]
Repouso Especial [X] [-1]
Âncora [X] [-1]
```

# Regra fundamental

> **Toda Corrupção vale [-1]. Para ser justa, precisa produzir uma limitação sobrenatural real e plausível; efeitos muito amplos são restringidos a fontes ou condições específicas. Corrupções criam consequências objetivas, nunca autoridade sobre escolhas voluntárias da personagem.**
