# Criação e Revisão de Personagens

Status: EM DESENVOLVIMENTO

Este arquivo descreve o fluxo atual de criação e revisão de personagens dentro do `novo-motor/`.

> **Proposta não é fato. Só salvar depois da aprovação explícita do jogador.**

## Núcleo mecânico

A construção mecânica segue esta ordem:

```text
1. Atributos
2. Perícias
3. Poderes
4. Passivos
5. Valores Derivados
```

Descrição, Recursos narrativos, Personalidade e Histórico podem ser preenchidos antes ou depois conforme a criação exigir, mas não formam uma camada mecânica adicional.

## 1. Atributos

Usar:

```text
Corpo — POD [ ] | HAB [ ] | RES [ ]
Mente — POD [ ] | HAB [ ] | RES [ ]
```

As funções são:

```text
POD → potência e intensidade
HAB → execução, precisão e controle
RES → resistência e sustentação
```

## 2. Perícias

Usar a lista atual de Perícias em `pericias.md`.

Perícias representam treinamento, conhecimento e experiência. Elas não formam uma lista separada de ataques.

A abordagem usada pelo personagem determina qual Perícia pode ser aplicável.

## 3. Poderes

Escolher os efeitos ativos que definem o que o personagem pode fazer.

A ficha registra:

```text
Golpe [2]
Disparo [3]
Explosão [2]
Teleporte [5]
```

Nos Poderes ativos, `[X]` é o máximo de Energia que pode ser investido em um único uso.

Cada Poder possui arquivo próprio em `poderes/` com efeito-base, alcance, alvo, duração, dano, ampliações e demais parâmetros necessários.

O objeto ou manifestação narrativa não cria outra regra mecânica. Uma espada pode representar Golpe; um batarang pode representar Disparo; uma granada pode representar Explosão.

## 4. Passivos

Escolher as capacidades permanentes ou estáveis do personagem.

Exemplos:

```text
RD [3]
Vida Extra [30]
Proteção [2]
Sentido-Aranha
Imortalidade
Regeneração [2]
```

Cada Passivo possui arquivo próprio em `passivos/`.

Nos Passivos, `[X]` tem o significado definido pela própria descrição e não representa gasto máximo de Energia.

## 5. Valores Derivados

Depois que Atributos, Perícias, Poderes e Passivos estiverem definidos, consolidar os valores de consulta rápida:

```text
Vida [ ] | Energia [ ]
Esquiva [ ] | Percepção [ ] | Vontade [ ] | Fortitude [ ] | RD [ ]
Deslocamento: [ ]
```

Passivos que alteram esses valores já entram no total final.

Não inventar fórmulas ainda não fechadas apenas para preencher campos vazios.

## Poderes durante o jogo

O fluxo de consulta é:

```text
jogador declara que quer usar um Poder
→ listar os Poderes disponíveis
→ jogador escolhe um
→ abrir somente o arquivo escolhido
→ mostrar efeito-base e ampliações
→ jogador declara a intenção
→ se couber no padrão, resolver
→ se exigir ampliação, informar o custo
→ aguardar confirmação
→ gastar Energia e resolver
```

O narrador não escolhe automaticamente uma ampliação que consuma Energia.

## Sem Arsenal mecânico

Não criar uma etapa de compra de armas, armaduras ou itens de combate.

A função mecânica desses elementos deve estar representada por Poderes ou Passivos. Objetos comuns continuam existindo na ficção quando fizer sentido.

## Conteúdo narrativo

A ficha ainda pode registrar:

```text
Descrição
Recursos narrativos
Personalidade
Histórico relevante
Conhecimento relevante
```

Esses campos existem para interpretação, contexto e possibilidades ficcionais, não para criar uma quinta camada mecânica.

## Salvamento

Durante criação assistida:

```text
base disponível
→ proposta
→ discussão
→ correção
→ aprovação explícita
→ salvamento
```

Conteúdo ainda em discussão não deve ser persistido como regra definitiva.

## Campo indefinido

Campo não definido permanece vazio.

```text
POD [ ] → ainda não definido
POD [0] → valor real igual a zero
```

> **Zero é valor real, nunca marcador de pendência.**
