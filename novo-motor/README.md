# Novo Motor

**Status: EM DESENVOLVIMENTO**

Esta pasta é o espaço de trabalho para uma nova arquitetura mecânica do sistema.

Ela fica **fora de `sistema/` de propósito**. Tudo desenvolvido aqui é experimental e **não altera nem substitui** as regras atuais em `sistema/resolucao/`, `sistema/personagem/` ou em qualquer outra pasta do sistema até aprovação explícita e migração posterior.

## Ideia inicial preservada da antiga Resolução 2

A intenção é reconstruir a resolução usando **uma única linguagem mecânica** para ações, resistências, combate, Poderes e Efeitos.

A base que estava em estudo na antiga `sistema/resolucao-2/` era:

```text
VALOR = Atributo + Dados de Destino + Dados de Perícia/Poder aplicável
```

Os **Dados de Destino** então considerados eram 4 dados com faces equivalentes a:

```text
-1, -1, 0, 0, +1, +1
```

Cada ponto de **Perícia**, **Poder** ou outra capacidade aplicável poderia acrescentar um dado próprio com faces:

```text
0, 0, 0, +1, +1, +1
```

Assim, um exemplo de ação era:

```text
Golpe = FIS + 4D de Destino + dados de Esgrima
```

E uma defesa poderia usar a mesma estrutura:

```text
Defesa = RES + 4D de Destino + dados de Armadura
```

Uma resistência por Vontade poderia seguir a mesma linguagem:

```text
Resistência = VON + 4D de Destino + dados de Poder defensivo
```

Quando houvesse oposição, a ideia em estudo era comparar os dois valores:

```text
Resultado = Ação - Resistência
```

- resultado positivo: a Ação prevalece;
- resultado negativo: a Resistência prevalece;
- resultado 0: empate, sem imposição automática de mudança.

A margem positiva poderia servir como **Potencial** da ação, mas a conversão desse Potencial em Dano, Cura, Controle, Teleporte ou outros resultados ainda seria desenvolvida e testada.

## Poderes e Efeitos

A direção registrada era que uma capacidade dissesse **o que o personagem consegue fazer**, enquanto o teste fosse necessário quando existisse oposição, dificuldade ou resistência relevante.

Exemplo conceitual:

```text
Teleporte [1] já permite teleportar.
```

O teste apareceria quando existisse algo a vencer, como distância difícil, barreira ou proteção. A dificuldade entraria como Resistência da ação.

A intenção futura era que capacidades específicas como `Golpe`, `Disparo`, `Magia`, `Teleporte`, `Portal`, `Banimento`, `Armadura` e outras pudessem possuir regras próprias, mas todas usando a mesma linguagem central de resolução.

## Objetivo do redesenho

- reduzir somas e fórmulas diferentes;
- fazer ataque e defesa usarem a mesma estrutura quando isso for desejável;
- fazer Poderes, Perícias e proteções entrarem numa linguagem mecânica simples;
- preservar leitura narrativa direta dos resultados;
- permitir que cada capacidade específica seja resolvida com o mínimo possível de consulta a outros arquivos.

## Regra de isolamento

Enquanto o novo motor estiver em desenvolvimento:

1. tudo dentro de `novo-motor/` é experimental;
2. **não alterar `sistema/` por causa do novo motor**;
3. trabalhar um ponto mecânico por vez;
4. não tratar ideias em estudo como regras aprovadas;
5. registrar aqui apenas o que fizer parte do desenvolvimento do novo motor;
6. a migração para `sistema/resolucao/`, `sistema/personagem/` ou outras áreas só acontece quando o novo motor estiver suficientemente fechado e houver decisão explícita para migrar.

> **Princípio de trabalho:** construir e testar o novo motor em paralelo, mantendo o sistema atual intacto até que a nova arquitetura esteja pronta para migração.
