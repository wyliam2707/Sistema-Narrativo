# Separação entre Testes e Combate

Status: RASCUNHO / NÃO IMPLEMENTADO

Este documento explora a possibilidade de separar claramente a resolução de ações gerais da resolução de combate.

## Ideia central

Atributos e Perícias representam principalmente a competência geral da personagem fora do confronto direto.

Combate, Poderes ofensivos, defesas extraordinárias e capacidades de confronto podem usar uma estrutura própria, sem depender automaticamente dos mesmos valores usados para investigação, conhecimento, interação social ou tarefas comuns.

Essa separação permite representar personagens de ficção super-heroica em que capacidade pessoal e poder destrutivo não possuem relação direta.

Exemplo conceitual:

```text
criança fisicamente frágil
+ pouca experiência prática
+ Poder capaz de destruir uma cidade
```

A fragilidade da personagem continua aparecendo em testes físicos comuns, enquanto o Poder mantém sua própria potência de combate.

## Fora de combate

Proposta simples:

```text
AÇÃO
→ verificar se o resultado é evidente, impossível ou incerto

INCERTEZA
→ uma única rolagem de Atributo
→ Perícia relevante pode modificar a rolagem
→ o resultado determina sucesso e eficiência
```

A intenção é que uma ação comum não exija consultar regras de combate, Dano, Defesas ou Poderes, salvo quando a própria capacidade extraordinária for necessária para tornar a ação possível.

## Eficiência por resultado

Possibilidade em estudo:

Uma única rolagem resolve tanto se a personagem consegue quanto quão bem consegue.

Modelo conceitual:

```text
resultado abaixo da dificuldade
→ falha

resultado suficiente
→ sucesso comum

resultado claramente acima
→ sucesso eficiente

resultado muito acima
→ sucesso excepcional
```

A escala exata ainda não está definida.

Uma opção é usar a margem sobre a Dificuldade, em vez do valor bruto, para que tarefas mais difíceis continuem exigindo desempenho proporcionalmente maior.

Exemplo provisório:

```text
margem 0–3
→ sucesso comum

margem 4–7
→ sucesso eficiente

margem 8+
→ sucesso excepcional
```

Essas faixas são apenas hipótese de trabalho e não estão aprovadas.

## Função das Perícias

As Perícias podem continuar servindo para representar treinamento, repertório e prática.

Possibilidades a comparar:

1. Perícia relevante concede +1d, mantendo 4 dados.
2. Perícia permite realizar tarefas especializadas e concede +1d quando houver incerteza.
3. Perícia não aumenta a rolagem, mas melhora a interpretação da eficiência ou permite resultados que um leigo não alcançaria.

Nenhuma dessas opções está escolhida ainda.

## Combate separado

A proposta não é fazer Atributos desaparecerem da ficha, mas impedir que eles determinem automaticamente a escala de combate.

Exemplo:

```text
Intelecto alto
→ excelente investigação, análise, ciência e estratégia

Raio de Energia [5]
→ potência ofensiva definida pelo próprio Poder
```

O Poder não precisa causar mais Dano só porque o Intelecto da personagem é alto, a menos que isso esteja explicitamente escrito no Poder.

Da mesma forma:

```text
Potência física baixa
≠ Poder físico fraco automaticamente
```

Uma personagem pode possuir corpo comum ou frágil e ainda controlar uma força externa extraordinária.

## Benefício esperado

A separação pretende produzir dois fluxos fáceis de entender:

```text
FORA DE COMBATE
Atributo + Perícia
→ uma rolagem
→ resultado define sucesso e eficiência

COMBATE
Poder / capacidade de confronto
→ usa valores próprios escritos na ficha
→ resolve ataque, defesa e efeito
```

Isso reduz a necessidade de fazer uma única estatística representar simultaneamente competência cotidiana, perícia, força narrativa e escala sobre-humana.

## Questões em aberto

Ainda é necessário decidir:

- se ataques mundanos usam o motor de combate ou o motor de Atributos;
- se Atributos influenciam iniciativa, defesa ou apenas ações não ofensivas;
- se Poderes podem opcionalmente usar Atributos quando isso fizer parte de sua construção;
- como representar personagens como lutadores altamente treinados sem Poderes;
- como Perícias interagem com ações de combate específicas;
- quais faixas de eficiência são mais intuitivas;
- se a eficiência deve usar margem sobre a Dificuldade ou outra leitura.

## Princípio de trabalho

> **Competência pessoal e potência de combate não precisam ser a mesma coisa.**

> **Uma única rolagem fora de combate deve, sempre que possível, dizer tanto se a ação funcionou quanto a qualidade do resultado.**
