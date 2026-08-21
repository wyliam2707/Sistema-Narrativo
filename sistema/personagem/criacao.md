# Criação e Revisão de Personagens

Status: APROVADO

Este arquivo define a criação de um personagem como entidade do sistema.

Ele não substitui o protocolo completo de criação de campanha. A campanha decide **quando** criar seus personagens; este arquivo define **como** um personagem deve ser concebido e convertido para ficha.

## Princípio central

> **Conceito primeiro. Mecânica depois.**

A criação deve começar por quem o personagem é, não por distribuir números.

## Etapa conceitual

Antes de calibrar a ficha mecânica, definir apenas o que for realmente necessário para compreender o personagem.

Podem importar:

- nome;
- natureza ou origem;
- aparência;
- idade real e aparente, quando diferentes;
- conceito;
- personalidade;
- comportamento social;
- história essencial;
- ocupações ou trajetória importante;
- situação atual;
- desejos e objetivos;
- medos e limites;
- TRAÇOS permanentes;
- `CONTROLE`, quando já definido pela estrutura da campanha.

Não é obrigatório preencher todos esses campos.

> **Perguntar e registrar apenas aquilo que realmente ajuda a definir o personagem.**

## Estrutura de ficha desde o começo

O arquivo do personagem pode usar desde a criação a estrutura final descrita em `ficha.md`.

Preencher apenas os campos já conhecidos.

Campos ainda desconhecidos ficam vazios.

> **Nunca usar `[0]` ou `[+0]` para representar pendência. Zero é um valor mecânico real.**

## O que não calibrar na etapa conceitual

Enquanto o conceito ainda está sendo construído, não atribuir automaticamente:

- FOR;
- AGI;
- RES;
- MEN;
- VON;
- graus de perícia;
- graus de poderes;
- especializações numéricas;
- relações numéricas ainda não estabelecidas.

Esses elementos entram na etapa de conversão mecânica.

## Criação mínima

Qualquer personagem pode nascer com uma ficha mínima.

Em uma campanha, pode ser suficiente inicialmente registrar:

- nome;
- importância, quando já definida;
- `CONTROLE`, quando já decidido;
- qualquer conceito realmente estabelecido.

Importância não determina tamanho, formato ou quantidade de detalhe da ficha.

Um personagem Central, Relevante, Figurante ou NPC pode ter apenas poucas linhas ou um dossiê extenso, conforme a necessidade real de interpretação e continuidade.

Não inventar aparência, personalidade, história, capacidades ou recursos apenas para completar visualmente a ficha.

Se o jogador delegar explicitamente a criação, uma proposta pode ser construída, mas continua sujeita à revisão normal quando for apresentável ao jogador.

## Conversão mecânica

Quando o conceito estiver suficientemente claro:

1. reconstruir as capacidades do personagem em linguagem natural;
2. identificar o que é atributo natural;
3. identificar perícias reais;
4. identificar poderes e repertórios;
5. identificar TRAÇOS qualitativos;
6. identificar RECURSOS recorrentes importantes;
7. identificar relações recorrentes que realmente pertencem à ficha;
8. converter para a sintaxe do sistema;
9. aplicar `calibracao.md`;
10. normalizar a ficha sem acrescentar conteúdo inexistente.

Todos os personagens usam as mesmas mecânicas e as mesmas escalas. NPC não possui sistema próprio de atributos, perícias, poderes, traços, relações ou recursos.

## Ordem das fichas iniciais de uma campanha

Durante criação conceitual, o protagonista pode ser definido antes dos demais.

Durante a revisão mecânica das fichas apresentáveis ao jogador, a ordem recomendada é:

```text
Personagens relevantes / NPCs visíveis
↓
Protagonista por último
```

A finalidade é evitar que os valores do protagonista sejam usados como régua inconsciente para calibrar o restante do elenco.

Essa ordem é uma proteção de processo. Ela **não autoriza comparação mecânica nem balanceamento entre fichas**.

Cada personagem continua sendo avaliado isoladamente conforme `calibracao.md`.

## Organização dos arquivos na campanha

Personagens jogáveis persistentes ficam normalmente em:

```text
personagens/
```

Isso inclui personagens sob `JOGADOR HUMANO` e `JOGADOR IA`.

NPCs pertencem ao mundo administrado pelo NARRADOR.

Um NPC simples pode existir apenas durante a cena e não precisa receber arquivo persistente.

Quando um NPC acumular informação que precise sobreviver entre cenas — capacidades, relações, desavenças, objetivos, conhecimento, pactos, recursos, obrigações ou outros ganchos relevantes — sua ficha pode ser registrada no mundo da campanha, normalmente em:

```text
mundo/npcs/
```

Ter arquivo persistente não altera automaticamente a Importância nem o `CONTROLE` do personagem.

## Revisão do personagem controlado pelo jogador humano

Quando a ficha pertence ao personagem do jogador humano, revisar com controle fino.

Ordem recomendada:

1. nome/identidade, se ainda houver algo a revisar;
2. `CONTROLE`;
3. idade;
4. conceito;
5. descrição;
6. TRAÇOS;
7. ATRIBUTOS como um bloco;
8. PERÍCIAS como um bloco;
9. PODERES como um bloco;
10. RECURSOS;
11. REL;
12. personalidade e tendências;
13. desejos/objetivos;
14. medos/limites;
15. história consolidada relevante;
16. ficha completa para aprovação final.

Se um campo já estiver definido, apresentá-lo como está para confirmação em vez de recriá-lo sem necessidade.

Nos blocos de ATRIBUTOS, PERÍCIAS e PODERES, normalizar a sintaxe e reapresentar o bloco inteiro antes de considerar a revisão concluída.

## Revisão em blocos

Quando for útil revisar um personagem de forma mais compacta, usar quatro blocos.

### Bloco 1 — Identidade e conceito

- nome;
- importância;
- `CONTROLE`;
- idade;
- conceito;
- descrição;
- TRAÇOS.

### Bloco 2 — Capacidades

- atributos;
- perícias;
- poderes;
- especializações.

### Bloco 3 — Recursos e relações

- RECURSOS recorrentes;
- REL atual e recorrente.

### Bloco 4 — Interpretação

- personalidade e tendências;
- desejos/objetivos;
- medos/limites;
- conhecimento atual relevante;
- história consolidada relevante.

Não inventar campos sem utilidade apenas para completar os quatro blocos.

## Personagens canônicos

Para um personagem canônico ou licenciado:

1. definir qual versão canônica ou adaptação vale para a campanha;
2. reconstruir suas capacidades sem números;
3. preservar identidade, personalidade, poderes e relações essenciais conforme essa versão;
4. somente depois converter para a linguagem do sistema;
5. aplicar calibração conservadora;
6. não ajustar a ficha para ficar parecida com a de outro personagem.

## Antagonistas reservados

Antagonistas importantes podem receber ficha completa sem revisão aberta quando a apresentação revelaria informação que deve permanecer secreta.

Isso não altera as regras de calibração.

Sempre que for prático, capacidades ocultas relevantes devem existir antes de serem usadas diretamente contra o protagonista.

Depois de estabelecidas, não podem ser alteradas apenas para contrariar uma solução válida ou recuperar dificuldade.

## Estado de aprovação

Uma ficha apresentável ao jogador permanece:

```text
Status: PENDENTE DE REVISÃO
```

até a leitura final consolidada ser aprovada.

Depois da aprovação explícita:

```text
Status: APROVADO
```

A versão final não deve carregar tentativas descartadas, explicações de conversa ou versões intermediárias.

## Progressão não é criação repetida

Concluir missão, capítulo ou arco não concede automaticamente:

- atributo novo;
- aumento de perícia;
- aumento de poder;
- nova capacidade.

A ficha só muda posteriormente quando a própria ficção muda de forma estável o personagem.

O procedimento de atualização pertence a `../persistencia/`.
