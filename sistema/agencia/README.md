# Agência

Esta pasta reúne as regras que respondem à pergunta:

> **Quem decide o quê, e como personagens continuam sendo agentes próprios mesmo fora da câmera?**

## Estado da migração

A estrutura nova está sendo construída sem apagar os arquivos antigos.

Enquanto uma regra ainda não tiver sido reescrita e aprovada nesta pasta, o arquivo antigo correspondente em `sistema/` continua válido.

## Responsabilidades desta área

Esta pasta deverá concentrar, progressivamente:

- agência de personagens;
- ciclo autônomo;
- vida fora da câmera;
- conhecimento separado;
- controle de personagem;
- ativação e desativação de `JOGADOR IA EVENTUAL`;
- relações entre personagens como agentes independentes;
- limites contra meta-jogo e vazamento de informação.

## Relação com `personas/`

`../personas/` define **as funções operacionais**.

Esta pasta define **como a agência dos personagens funciona ao longo da ficção**.

Exemplo:

- `personas/jogador-ia/` define o papel `JOGADOR IA`;
- `agencia/` define como esse personagem mantém rotina, objetivos, relações e decisões fora da cena principal.

## Arquivos antigos ainda em uso

- `../agencia-de-personagens.md` — regra ampla de agência e ciclo autônomo atual.
- `../ciclo-de-jogadores.md` — ordem operacional atual entre declarações, Opositor e Narrador.

## Regra de migração

Novos arquivos devem separar conceitos que hoje estão reunidos no documento antigo, sem perder comportamento já validado em campanha.

> **Agência não é reação conveniente ao protagonista; é continuidade de vontade própria.**
