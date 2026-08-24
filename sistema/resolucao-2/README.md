# Resolução 2

**Status: EM DESENVOLVIMENTO**

Esta pasta é o espaço de trabalho para uma nova arquitetura de resolução do sistema.

As regras desenvolvidas aqui são experimentais e **não alteram nem substituem** as regras atuais em `sistema/resolucao/` ou em qualquer outra pasta até aprovação explícita.

## Ideia inicial

A intenção é reconstruir a resolução usando **uma única linguagem mecânica** para ações, resistências, combate, Poderes e Efeitos.

A base em estudo é:

```text
VALOR = Atributo + Dados de Destino + Dados de Perícia/Poder aplicável
```

Os **Dados de Destino** atualmente considerados são 4 dados com faces equivalentes a:

```text
-1, -1, 0, 0, +1, +1
```

Cada ponto de **Perícia**, **Poder** ou outra capacidade aplicável pode acrescentar um dado próprio com faces:

```text
0, 0, 0, +1, +1, +1
```

Assim, um exemplo de ação pode ser:

```text
Golpe = FIS + 4D de Destino + dados de Esgrima
```

E uma defesa pode usar a mesma estrutura:

```text
Defesa = RES + 4D de Destino + dados de Armadura
```

Uma resistência por Vontade pode seguir a mesma linguagem:

```text
Resistência = VON + 4D de Destino + dados de Poder defensivo
```

Quando houver oposição, a ideia em estudo é comparar os dois valores:

```text
Resultado = Ação - Resistência
```

- resultado positivo: a Ação prevalece;
- resultado negativo: a Resistência prevalece;
- resultado 0: empate, sem imposição automática de mudança.

A margem positiva poderá servir como **Potencial** da ação, mas a conversão desse Potencial em Dano, Cura, Controle, Teleporte ou outros resultados ainda será desenvolvida e testada.

## Poderes e Efeitos

A direção atual é que uma capacidade diga **o que o personagem consegue fazer**, enquanto o teste seja necessário quando existir oposição, dificuldade ou resistência relevante.

Exemplo conceitual:

```text
Teleporte [1] já permite teleportar.
```

O teste aparece quando existe algo a vencer, como distância difícil, barreira ou proteção. A dificuldade entra como Resistência da ação.

A intenção futura é que capacidades específicas como `Golpe`, `Disparo`, `Magia`, `Teleporte`, `Portal`, `Banimento`, `Armadura` e outras possam possuir regras próprias, mas todas usando a mesma linguagem central de resolução.

## Objetivo do redesenho

- reduzir somas e fórmulas diferentes;
- fazer ataque e defesa usarem a mesma estrutura;
- fazer Poderes, Perícias e proteções entrarem na mesma linguagem mecânica;
- preservar leitura narrativa direta dos resultados;
- permitir que cada capacidade específica seja resolvida com o mínimo possível de consulta a outros arquivos.

## Como retomar este trabalho em outro chat

Se o usuário pedir para **abrir**, **continuar** ou **trabalhar na Resolução 2**, faça o seguinte:

1. Leia primeiro este `README.md` e trate-o como o ponto de retomada da nova arquitetura.
2. Considere tudo em `sistema/resolucao-2/` como experimental e separado do sistema atual.
3. **Não altere `sistema/resolucao/` nem outras pastas existentes** por causa da Resolução 2, salvo pedido e aprovação explícitos do usuário.
4. Antes de qualquer mudança no repositório, primeiro analise e proponha a alteração; espere a confirmação do usuário.
5. Trabalhe **um ponto mecânico por vez**, evitando criar várias dúvidas novas na mesma resposta.
6. Não presuma que ideias registradas como "em estudo" já estejam aprovadas como regra final.
7. À medida que novas regras forem aprovadas, registre-as dentro de `sistema/resolucao-2/` sem apagar ou migrar a resolução antiga até decisão explícita posterior.

> **Princípio de trabalho:** construir e testar a nova resolução em paralelo, mantendo o sistema atual intacto até que a nova arquitetura esteja suficientemente fechada para uma eventual migração.
