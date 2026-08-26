# Poderes

Status: APROVADO

Um **Poder** representa parte do arsenal funcional do personagem.

Ele define ações específicas, efeitos e possibilidades que vão além das ações comuns resolvidas diretamente por Atributos, equipamentos ordinários e ficção básica.

A origem pode ser:

- mundana;
- física;
- técnica;
- tecnológica;
- sobrenatural;
- psíquica;
- biológica;
- qualquer outra coerente com o Conceito.

> **Poder representa o que o personagem consegue produzir como parte de seu arsenal especial.**

---

## 1. Poder não usa grau genérico

Poderes não usam mais uma escala universal:

```text
[1] [2] [3] [4] [5]
```

Essa graduação antiga não faz parte do motor atual.

A ficha registra apenas quais Poderes o personagem possui.

Exemplo:

```text
PODERES:
- Teleporte
- Proteção
- Ilusão
```

A ausência de um Poder significa que aquela capacidade não faz parte do arsenal funcional registrado do personagem.

Não usar `Poder [0]` como marcador.

---

## 2. Ações comuns não exigem Poder

Qualquer personagem pode tentar ações comuns que sejam ficcionalmente possíveis para ele.

Exemplos:

```text
socar
correr
escalar
empurrar
usar uma ferramenta comum
```

Essas ações não exigem um Poder chamado `Soco`, `Corrida` ou equivalente.

Poder é necessário quando a personagem pretende produzir uma capacidade especial que não existe apenas pela ação comum e pelos meios disponíveis.

Exemplos:

```text
teleportar
criar uma Barreira sobrenatural
invocar uma criatura
alterar a mente de alguém por efeito extraordinário
produzir um disparo especial de energia
```

---

## 3. Hub

Cada Poder possui sua própria regra e seu próprio **Hub**.

O Hub organiza apenas as dimensões relevantes para aquele Poder, que podem incluir:

- Alcance;
- Alvos;
- Área;
- Dano;
- Efeito;
- Defesa;
- Duração;
- Conjuração;
- Tipo;
- Modo;
- Distância;
- Escopo;
- Contra;
- Tamanho;
- Material;
- outras propriedades específicas.

Nem todo Poder usa todos esses campos.

> **O arquivo do Poder define o que ele faz. O Hub define como aquele uso é configurado.**

---

## 4. Custo e [X]

Quando uma progressão de Hub não disser outra coisa:

- a primeira posição custa `+0`;
- cada avanço seguinte custa `+1`;
- opções equivalentes no mesmo estágio possuem o mesmo custo;
- o custo final é a soma das opções escolhidas.

`[X]` representa:

> **Patamar da personagem**

E normalmente limita:

> **a quantidade máxima de Mana que pode ser gasta em um único uso do Poder**

Alguns Poderes possuem custo operacional a partir de `0+ Mana`; outros a partir de `1+ Mana`, conforme sua própria regra.

Consultar `../resolucao/mana.md` e `patamar.md`.

---

## 5. Configuração pertence ao jogador da peça

Quando um Poder possuir escolhas que alterem custo ou resultado, o controlador da personagem decide a configuração voluntária.

O NARRADOR pergunta somente o que ainda estiver faltando para resolver o uso.

Se alvo, forma, alcance, intensidade e demais escolhas já estiverem claros na declaração, não perguntar novamente.

O NARRADOR não escolhe silenciosamente uma configuração mais cara, mais fraca ou diferente da intenção declarada.

As regras de autoridade continuam pertencendo a `../personas/`.

---

## 6. Ataques comuns e Poderes ofensivos

Uma personagem sem Poder ofensivo ainda pode realizar um ataque comum.

Quando um ataque comum causa Dano sem usar fonte especial com Dano próprio:

> **Dano = Atributo utilizado no ataque**

Sem rolagem separada de Dano.

Poderes ofensivos substituem essa forma simples pelas regras próprias de seu Hub, podendo definir:

- Dano;
- alcance;
- Defesa;
- Resistência;
- Efeito;
- Área;
- Alvos;
- outras propriedades.

A resolução completa pertence a `../resolucao/combate-e-dano.md` e aos arquivos específicos de Poder.

---

## 7. Poder, Atributo e Perícia

Cada parte da ficha responde a uma pergunta diferente:

```text
ATRIBUTO
→ qual capacidade fundamental o personagem possui?

PERÍCIA
→ em quais campos possui treinamento e experiência?

PODER
→ quais funções especiais fazem parte de seu arsenal?
```

Atributos, Perícias e Poderes não são somados automaticamente.

Uma Perícia pode conceder `+1d` quando realmente for relevante para a resolução, mas não aumenta genericamente Dano ou custo de Poder.

---

## 8. Capacidade natural e Poder

Uma capacidade natural ou permanente já representada adequadamente por um Atributo não precisa ser duplicada como Poder apenas para repetir a mesma coisa.

Exemplo:

```text
Potência [5]
```

já pode representar força natural extraordinária.

Mas uma capacidade ativa, configurável ou com efeito próprio pode ser Poder.

Exemplo:

```text
Aprimoramento
→ aumenta temporariamente Atributos conforme seu Hub
```

---

## 9. Forma narrativa e função mecânica

A aparência do efeito não cria automaticamente uma categoria nova de Poder.

Um mesmo Poder ofensivo pode se manifestar como raio, projétil, golpe, onda ou outra forma quando sua própria regra e o Conceito permitirem.

Da mesma forma, Poderes diferentes podem produzir resultados visualmente parecidos sem serem mecanicamente iguais.

> **A forma vem da ficção; a função vem da regra específica do Poder.**

---

## 10. Calibração

Poderes são escolhidos pelo que realmente pertence ao personagem.

Não adicionar, retirar ou alterar Poderes apenas para:

- equilibrar grupo automaticamente;
- aproximar duas fichas sem pedido do jogador;
- garantir determinado vencedor;
- recuperar dificuldade depois de uma solução válida.

A regra completa pertence a `calibracao.md`.

---

## 11. Migração dos arquivos específicos

A posse e o registro de Poderes pertencem a `personagem/`.

As regras concretas de cada Poder e seus Hubs pertencem à camada de resolução e serão organizadas em:

```text
../resolucao/poderes/
```

Enquanto a migração desses arquivos específicos não estiver concluída, não inventar novas graduações genéricas para preencher a lacuna.

---

## Regra final

> **Poder é arsenal funcional, não uma nota de [1] a [5]. A ficha registra quais Poderes existem; cada arquivo específico define o que eles fazem e o Hub define como cada uso é configurado dentro do limite de Mana e Patamar.**
