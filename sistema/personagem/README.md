# Personagem

Status: APROVADO

Esta pasta reúne as regras que respondem à pergunta:

> **Como uma entidade do jogo é concebida, definida mecanicamente e registrada em ficha?**

Ela separa a definição estável do personagem da resolução de suas ações e de seu estado momentâneo.

## Responsabilidades desta área

Esta pasta concentra:

- criação conceitual de personagens;
- conversão do conceito para a linguagem mecânica;
- calibração independente;
- Patamar;
- Atributos;
- Perícias;
- Poderes;
- Traços;
- RECURSOS;
- relações recorrentes;
- estrutura e organização visual de ficha;
- representação compacta de NPCs;
- Importância;
- `CONTROLE` como metadado estrutural da ficha.

Todos os personagens usam as mesmas mecânicas.

NPC não possui uma mecânica própria. O que muda é quem controla a personagem, sua função estrutural e quanto precisa ser persistido para continuidade.

## Base mecânica atual

```text
Patamar
→ [1] a [7]

Atributos permanentes
→ Potência
→ Controle
→ Resistência
→ Intelecto
→ Presença
→ Vontade
→ escala normal [-2] a [7]

Perícias
→ sem graduação
→ relevante = +1d

Poderes
→ arsenal funcional
→ sem grau genérico [1–5]
→ configurados por Hub

Vida Máxima
→ derivada dos Atributos

Mana Máxima
→ derivada dos Atributos
```

A resolução dessas capacidades pertence a `../resolucao/`.

## Ficha não é estado atual

Vida atual, Mana atual, Status, efeitos temporários, localização, Barreiras e demais condições momentâneas pertencem ao estado da campanha.

A ficha registra capacidades consolidadas e valores máximos de referência.

> **Personagem define quem a entidade é e do que ela é capaz. Estado registra como ela está agora.**

## O que não pertence aqui

Esta área não define:

- processo completo de criação de campanha — `../criacao/`;
- como uma intenção vira resultado — `../resolucao/`;
- quem possui autoridade operacional — `../personas/`;
- agência e vida fora da câmera — `../agencia/`;
- apresentação literária — `../narracao/`;
- estado atual e atualização persistente — `../persistencia/`;
- ordem operacional de consulta — `../operacao/`.

## Relação com criação de campanha

O processo canônico para criar uma campanha está em:

```text
sistema/criacao/README.md
```

Esta pasta fornece o modelo e as regras usados quando `criacao/` manda construir ou revisar uma ficha.

A criação de personagem pertence a `criacao.md`.

## Organização dentro da campanha

Personagens com agência de jogador ficam em:

```text
campanhas/<nome>/personagens/
```

Isso inclui:

- `CONTROLE: JOGADOR HUMANO`;
- `CONTROLE: JOGADOR IA`;
- `CONTROLE: JOGADOR IA EVENTUAL`.

NPCs persistentes sem agência de jogador ficam em:

```text
campanhas/<nome>/mestre/
```

ou, quando útil:

```text
campanhas/<nome>/mestre/npcs/
```

`mundo/` guarda fatos estáveis do cenário e não é o destino padrão de fichas de NPC.

## Importância e CONTROLE

`Importância` e `CONTROLE` são informações diferentes.

`Importância` descreve função estrutural.

`CONTROLE` registra quem normalmente toma as decisões voluntárias da peça.

Exemplo:

```text
Importância: Relevante
CONTROLE: NPC
```

Ser Relevante não transforma automaticamente o personagem em jogador eventual. Figurante não significa mecanicamente fraco.

As regras detalhadas estão em `ficha.md`, `npcs.md` e `../personas/`.

## Arquivos principais

- `criacao.md` — criação e revisão de personagem;
- `calibracao.md` — calibração independente;
- `escala.md` — resumo das escalas atuais;
- `patamar.md` — Patamar, pontos e limites de criação;
- `atributos.md` — seis Atributos atuais;
- `pericias.md` — lista canônica e regra de `+1d`;
- `poderes.md` — conceito de arsenal funcional e Hub;
- `tracos.md` — verdades passivas, grupos e valores de aquisição;
- `ficha.md` — estrutura consolidada, Importância, CONTROLE, Vida e Mana máximas;
- `npcs.md` — mesma mecânica com representação rápida ou mínima;
- `organizacao-visual.md` — padrão visual de ficha;
- `relacoes.md` — relações recorrentes;
- `pareamento.md` — comparação cruzada de informações relacionais;
- `relevancia-da-ficha.md` — o que merece ser persistido.

## Compatibilidade

Não usar em novas fichas:

```text
FIS / RES / MEN / VON
Perícia [+0..+5]
Poder [1..5]
ENERGIA como reserva universal
Vida escolhida por função narrativa
```

Referências antigas ainda existentes em outras áreas devem ser tratadas como resíduos de migração até serem revisadas.

## Regra final

> **A ficha descreve quem o personagem é e o que precisa ser lembrado para interpretá-lo. A mecânica atual usa Patamar, seis Atributos, Perícias sem graduação, Poderes por Hub, Traços, Vida e Mana derivadas. Estado momentâneo continua fora da ficha consolidada.**
