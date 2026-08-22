# Personagem

Status: APROVADO

Esta pasta reúne as regras que respondem à pergunta:

> **Como uma entidade do jogo é concebida, definida mecanicamente e registrada em ficha?**

Ela existe para separar a definição do personagem da resolução de suas ações e de seu estado momentâneo.

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
- regras para representação compacta de personagens quando poucos dados forem necessários;
- regras de NPCs e de persistência de NPCs no mundo da campanha.

Todos os personagens usam as mesmas mecânicas de ATRIBUTOS, PERÍCIAS, PODERES, TRAÇOS, REL e RECURSOS.

NPC não possui uma mecânica própria. O que muda é quem controla o personagem, sua função estrutural e quanto vale a pena registrar para continuidade.

## O que não pertence aqui

Esta área não define:

- como uma intenção vira resultado — `../resolucao/`;
- quem possui autoridade operacional de decisão sobre cada personagem — `../personas/`;
- agência e vida fora da câmera — `../agencia/`;
- apresentação literária da ficção — `../narracao/`;
- STATUS, cronologia e atualização persistente de fichas — `../persistencia/`;
- ordem operacional de consulta do sistema — `../operacao/`.

Vida atual, Mana ou Energia atual, ferimentos, condições temporárias, efeitos ativos, localização e outras informações que mudam rapidamente pertencem ao STATUS ou à resolução, não à definição consolidada do personagem.

Uma capacidade máxima ou estrutural pode ser definida por outras regras do sistema, mas seu valor atual continua sendo estado momentâneo.

## Princípio estrutural

> **Personagem define quem a entidade é e do que ela é capaz. Resolução consulta essa definição. STATUS registra como ela está agora. Persistência altera a ficha quando a ficção altera de forma estável o personagem.**

## Organização dentro da campanha

Personagens jogáveis persistentes ficam normalmente em:

```text
aventuras/<campanha>/personagens/
```

Essa pasta é preparada para os personagens efetivamente jogáveis, como `JOGADOR HUMANO` e `JOGADOR IA`.

NPCs pertencem ao mundo administrado pelo NARRADOR.

Um NPC não precisa de arquivo só por existir ou aparecer várias vezes. Quando houver informação que precise sobreviver entre cenas, o NARRADOR pode criar sua ficha persistente em:

```text
aventuras/<campanha>/mundo/npcs/
```

A pasta `mundo/npcs/` não precisa existir no início da campanha. Ela pode ser criada pelo NARRADOR apenas quando surgir a necessidade real de persistência.

## Importância e CONTROLE

`Importância` e `CONTROLE` são informações diferentes.

`Importância` descreve a função estrutural do personagem na campanha.

`CONTROLE` registra como ele participa normalmente do ciclo de decisão.

Um personagem Relevante pode, por exemplo, continuar sendo:

```text
Importância: Relevante
CONTROLE: NPC
```

ou pode usar `JOGADOR IA EVENTUAL` quando essa forma de agência tiver sido definida para ele.

Central pertence ao núcleo jogável. Relevante não significa automaticamente jogável. Figurante não significa mecanicamente fraco.

As regras detalhadas estão em `ficha.md` e `npcs.md`.

## Estado da migração

Os arquivos desta pasta foram construídos a partir das regras antigas encontradas diretamente em `sistema/`.

Os arquivos antigos NÃO foram apagados ou movidos durante a migração.

`MAPA-DE-ORIGEM.md` registra de onde veio cada bloco de regra e quais conteúdos permaneceram em outras áreas, como resolução, STATUS, agência e operação.

## Arquivos

- `criacao.md` — criação conceitual, conversão para ficha e organização dos personagens na campanha;
- `calibracao.md` — calibração independente, conservadora e raridade dos graus altos;
- `escala.md` — escalas numéricas e lógica não linear de PATAMAR;
- `atributos.md` — FIS, RES, MEN e VON;
- `pericias.md` — conhecimento, treinamento, prática e especializações;
- `poderes.md` — arsenais, fontes, repertórios, usos e especializações;
- `tracos.md` — verdades qualitativas estáveis;
- `relacoes.md` — relações recorrentes registradas em ficha;
- `ficha.md` — estrutura consolidada, Importância, CONTROLE, RECURSOS e informação reservada;
- `npcs.md` — controle normal de NPCs, ficha compacta, persistência em `mundo/npcs/` e relação com o OPOSITOR;
- `MAPA-DE-ORIGEM.md` — classificação dos arquivos e seções antigas usadas na migração.

> **A ficha descreve quem o personagem é e o que precisa ser lembrado para interpretá-lo. Ela não é STATUS, inventário, diário de campanha nem mecanismo de resolução.**
