# Agência

Esta pasta reúne as regras que respondem à pergunta:

> **Quem decide o quê, e como personagens continuam sendo agentes próprios mesmo fora da câmera?**

## Estado da migração

A estrutura nova está sendo construída progressivamente.

Alguns arquivos antigos em `sistema/` ainda permanecem como fontes históricas nos pontos não substituídos por regras aprovadas da arquitetura nova. Arquivos já removidos após substituição completa não devem ser procurados nem usados como fonte operacional.

## Responsabilidades desta área

Esta pasta deverá concentrar, progressivamente:

- agência de personagens;
- ciclo autônomo;
- vida fora da câmera;
- conhecimento separado;
- continuidade de objetivos e relações;
- ativação e desativação de `JOGADOR IA EVENTUAL`;
- relações entre personagens como agentes independentes;
- limites contra meta-jogo e vazamento de informação.

## Arquivos aprovados nesta área

- `continuidade-de-npcs.md` — define quando NPCs precisam de acompanhamento, como preservar retornos e pendências futuras sem simular suas vidas dia a dia e como esses fios voltam a mover a história.
- `continuidade-de-jogadores-ia.md` — define como JOGADORES IA mantêm continuidade fora da câmera e como suas declarações compartilham o mesmo intervalo temporal, podendo interromper uma ação longa quando criam nova decisão.

## Relação com outras áreas

`../personas/` define **as funções operacionais e autoridades de decisão**.

`../personagem/` define **quem a entidade é e do que é capaz**.

`agencia/` define **como essa entidade continua exercendo vontade própria ao longo da ficção**, inclusive fora da cena principal.

Exemplo:

- `personas/jogador-ia/` define o papel `JOGADOR IA`;
- `personagem/` guarda a definição estável da peça;
- `agencia/` define como essa peça mantém rotina, objetivos, relações e decisões fora da câmera.

## Fonte antiga ainda útil

- `../agencia-de-personagens.md` — fonte histórica para regras de agência e ciclo autônomo ainda não reescritas nesta pasta.

A ordem operacional atual do ciclo está em `../operacao/ciclo-de-cena.md`.

## Regra de migração

Novos arquivos devem separar conceitos que hoje ainda estejam reunidos em documentos antigos, sem perder comportamento já validado em campanha.

Quando uma formulação antiga contradiz uma regra nova explicitamente aprovada, prevalece a regra nova.

> **Agência não é reação conveniente ao protagonista; é continuidade de vontade própria.**
