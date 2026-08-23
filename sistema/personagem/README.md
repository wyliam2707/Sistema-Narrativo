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
- estrutura de ficha;
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

Esta pasta não cria uma segunda sequência de campanha. Ela fornece o modelo e as regras de personagem usados quando `criacao/` manda construir ou revisar uma ficha.

Durante a criação de campanha, prevalecem a ordem, os blocos de revisão, o checkpoint e as regras de salvamento definidos em `../criacao/README.md`.

## Organização dentro da campanha

Personagens com agência de jogador ficam em:

```text
campanhas/<nome>/personagens/
```

Isso inclui:

- protagonista com `CONTROLE: JOGADOR HUMANO`;
- personagens com `CONTROLE: JOGADOR IA`;
- personagens com `CONTROLE: JOGADOR IA EVENTUAL`.

Cada personagem com agência possui **seu próprio arquivo**, mesmo quando vários personagens são administrados pela mesma persona `JOGADOR IA EVENTUAL`.

Exemplo:

```text
campanhas/<nome>/personagens/
├── README.md
├── protagonista.md
├── ravena.md
├── dick-grayson.md
└── kory.md
```

> **Persona compartilhada não cria ficha compartilhada.**

NPCs comuns, aliados ocasionais, figurantes e adversários não pertencem por padrão a `personagens/`.

Um NPC pode existir somente em cena sem arquivo próprio. Quando precisar de persistência reservada para continuidade, sua ficha ou informação operacional fica em:

```text
campanhas/<nome>/mestre/
```

Quando houver quantidade suficiente para justificar subdivisão, pode existir:

```text
campanhas/<nome>/mestre/npcs/
```

Não criar `mundo/npcs/` como destino padrão. `mundo/` guarda fatos estáveis do cenário; `mestre/` guarda NPCs e material reservado de condução.

Se um personagem que era NPC passar a receber agência formal de jogador e `CONTROLE: JOGADOR IA EVENTUAL`, sua ficha canônica passa a pertencer a `personagens/`. Informação realmente reservada que não pertença à ficha aberta pode continuar em `mestre/` sem duplicar a ficha inteira.

## Importância e CONTROLE

`Importância` e `CONTROLE` são informações diferentes.

`Importância` descreve a função estrutural do personagem na campanha.

`CONTROLE` registra como ele participa normalmente do ciclo de decisão.

Exemplo:

```text
Importância: Relevante
CONTROLE: NPC
```

ou, quando a campanha tiver definido agência própria:

```text
Importância: Relevante
CONTROLE: JOGADOR IA EVENTUAL
```

Ser Relevante não transforma automaticamente o personagem em jogador eventual. Figurante não significa mecanicamente fraco.

As regras detalhadas estão em `ficha.md` e `npcs.md`.

## Estado da migração

Os arquivos desta pasta foram construídos a partir das regras antigas encontradas diretamente em `sistema/`.

Os arquivos antigos não são apagados durante a migração, mas referências antigas de organização não prevalecem contra `../criacao/estrutura-da-campanha.md`.

`MAPA-DE-ORIGEM.md` registra a origem histórica das regras.

## Arquivos

- `criacao.md` — criação conceitual e conversão de personagem; a sequência de campanha pertence a `../criacao/`;
- `calibracao.md` — calibração independente, conservadora e raridade dos graus altos;
- `escala.md` — escalas numéricas e lógica não linear de PATAMAR;
- `atributos.md` — FIS, RES, MEN e VON;
- `pericias.md` — conhecimento, treinamento, prática e especializações;
- `poderes.md` — arsenais, fontes, repertórios, usos e especializações;
- `tracos.md` — verdades qualitativas estáveis;
- `relacoes.md` — relações recorrentes registradas em ficha;
- `ficha.md` — estrutura consolidada, Importância, CONTROLE, RECURSOS e informação necessária à interpretação;
- `npcs.md` — controle normal de NPCs, ficha compacta e persistência reservada;
- `MAPA-DE-ORIGEM.md` — classificação dos arquivos e seções antigas usadas na migração.

> **A ficha descreve quem o personagem é e o que precisa ser lembrado para interpretá-lo. Ela não é estado atual, inventário, diário de campanha nem mecanismo de resolução.**
