# Personagem

Status: APROVADO

Esta pasta reúne as regras que respondem à pergunta:

> **Como uma entidade do jogo é concebida, definida mecanicamente e registrada em ficha?**

Ela separa a definição estável do personagem da resolução de suas ações e de seu estado momentâneo.

## Responsabilidades desta área

Esta pasta concentra:

- criação conceitual de personagens;
- conversão do conceito para a linguagem mecânica do sistema;
- calibração independente e conservadora;
- escala numérica;
- atributos;
- perícias;
- poderes, fontes, repertórios e especializações;
- TRAÇOS;
- RECURSOS;
- relações recorrentes registradas em `REL`;
- pareamento de informações entre fichas relacionadas;
- estrutura de ficha;
- organização visual das fichas em Markdown;
- relevância do que merece ou não ser persistido na ficha;
- Importância;
- `CONTROLE` como metadado estrutural da ficha;
- representação compacta quando poucos dados forem necessários;
- regras mecânicas e estruturais de NPCs.

Todos os personagens usam as mesmas mecânicas de ATRIBUTOS, PERÍCIAS, PODERES, TRAÇOS, REL e RECURSOS.

NPC não possui uma mecânica própria. O que muda é quem controla a personagem, sua função estrutural e quanto precisa ser persistido para continuidade.

## O que não pertence aqui

Esta área não define:

- o processo completo de criação de campanha — `../criacao/`;
- como uma intenção vira resultado — `../resolucao/`;
- quem possui autoridade operacional sobre cada personagem — `../personas/`;
- agência e vida fora da câmera — `../agencia/`;
- apresentação literária da ficção — `../narracao/`;
- estado atual e atualização persistente — `../persistencia/`;
- ordem operacional de consulta — `../operacao/`.

Vida atual, Energia atual, ferimentos, condições temporárias, efeitos ativos, localização e outras informações circunstanciais pertencem ao estado da campanha, não à definição consolidada da ficha.

## Princípio estrutural

> **Personagem define quem a entidade é e do que ela é capaz. Resolução consulta essa definição. Estado registra como ela está agora. Persistência altera a ficha quando a ficção altera de forma estável o personagem.**

## Relação com a criação de campanha

O processo canônico para criar uma campanha está em:

```text
sistema/criacao/README.md
```

Esta pasta fornece o modelo e as regras de personagem usados quando `criacao/` manda construir ou revisar uma ficha.

Depois que todas as fichas iniciais são aprovadas, `pareamento.md` orienta a comparação cruzada entre personagens antes da definição da situação inicial.

A apresentação visual padrão das fichas pertence a:

```text
sistema/personagem/organizacao-visual.md
```

A regra sobre o que realmente merece entrar na ficha pertence a:

```text
sistema/personagem/relevancia-da-ficha.md
```

## Organização dentro da campanha

Personagens com agência de jogador ficam em:

```text
campanhas/<nome>/personagens/
```

Isso inclui:

- `CONTROLE: JOGADOR HUMANO`;
- `CONTROLE: JOGADOR IA`;
- `CONTROLE: JOGADOR IA EVENTUAL`.

Cada personagem com agência possui seu próprio arquivo, mesmo quando vários personagens usam a mesma persona `JOGADOR IA EVENTUAL`.

NPCs comuns não pertencem por padrão a `personagens/`. Quando precisarem de persistência reservada para continuidade, ficam em:

```text
campanhas/<nome>/mestre/
```

Quando houver quantidade suficiente, pode existir:

```text
campanhas/<nome>/mestre/npcs/
```

Não criar `mundo/npcs/` como destino padrão. `mundo/` guarda fatos estáveis do cenário; `mestre/` guarda NPCs e material reservado.

Se um NPC receber agência formal de jogador, sua ficha canônica passa a pertencer a `personagens/`.

## Importância e CONTROLE

`Importância` e `CONTROLE` são informações diferentes.

`Importância` descreve função estrutural.

`CONTROLE` registra quem normalmente toma as decisões voluntárias da peça.

Exemplo:

```text
Importância: Relevante
CONTROLE: NPC
```

ou:

```text
Importância: Relevante
CONTROLE: JOGADOR IA EVENTUAL
```

Ser Relevante não transforma automaticamente o personagem em jogador eventual. Figurante não significa mecanicamente fraco.

As regras detalhadas estão em `ficha.md` e `npcs.md`.

## Arquivos

- `criacao.md` — criação conceitual e conversão de personagem;
- `calibracao.md` — calibração independente e conservadora;
- `escala.md` — escalas numéricas e lógica não linear de PATAMAR;
- `atributos.md` — FIS, RES, MEN e VON;
- `pericias.md` — conhecimento, treinamento, prática e especializações;
- `poderes.md` — arsenais, fontes, repertórios, usos e especializações;
- `tracos.md` — verdades qualitativas estáveis;
- `relacoes.md` — relações recorrentes registradas em ficha;
- `pareamento.md` — comparação cruzada entre fichas, perguntas ao jogador e ajuste das informações relacionais;
- `ficha.md` — estrutura consolidada, Importância, CONTROLE, RECURSOS e interpretação;
- `organizacao-visual.md` — padrão de apresentação por tópicos para manter a ficha legível no Markdown/GitHub;
- `relevancia-da-ficha.md` — regra para persistir somente informação útil à interpretação e continuidade, evitando meta-comparações desnecessárias com obras-base;
- `npcs.md` — controle normal de NPCs, ficha compacta e persistência reservada.

> **A ficha descreve quem o personagem é e o que precisa ser lembrado para interpretá-lo. Ela não é estado atual, inventário, diário de campanha nem mecanismo de resolução.**
