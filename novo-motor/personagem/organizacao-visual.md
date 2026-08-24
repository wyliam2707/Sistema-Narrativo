# Organização Visual das Fichas

Status: EM DESENVOLVIMENTO

Este arquivo define a apresentação visual atual da ficha de personagem dentro do `novo-motor/`.

A prioridade é permitir leitura rápida por jogador humano, narrador e jogador IA.

> **Cada bloco deve responder a uma função clara e ser consultável sem reler a ficha inteira.**

## Estrutura visual atual

```markdown
# Nome do personagem

## Descrição
Nome: Codinome — Nome real
Importância:
Controle:
Idade:
Peso:
Altura:

Descrição visual:

## Atributos
Corpo - Força [ ] | Destreza [ ] | Agilidade [ ]
Mente - Intelecto [ ] | Percepção [ ] | Presença [ ]

## Perícias
Comuns
Esportes [ ] | Exploração [ ] | Expressão [ ] | Sociedade [ ]
Investigação [ ] | Crime [ ] | Ofícios [ ] | Idiomas [ ]

Somente treinadas
Arcano [ ] | Ocultismo [ ] | Natureza [ ] | Medicina [ ]
Engenharia [ ] | Ciência [ ] | Tecnologia [ ] | História [ ]

## Referências
Vida [ ] | Energia [ ] | Deslocamento: Curto | Visão: Comum longa
Defesas - Esquiva [ ] | Vontade [ ] | Fortitude [ ] | RD: Geral [ ]

## Ataques
Luta [ ] / arma / dano / crítico / alcance
Disparo [ ] / arma / dano / crítico / alcance
Magia [ ] / arma ou efeito / dano / crítico / alcance

## Poderes
- Nome do poder

## Recursos
- Recurso relevante

## Personalidade
Descrição mental:
Desejos:
Medos:
Vínculos:

## Histórico
Histórico relevante:
Conhecimento relevante:
```

## Regras de apresentação

- manter `Atributos` em exatamente duas linhas;
- manter as Perícias nos dois grupos de oito;
- manter `Referências` em duas linhas compactas sempre que possível;
- manter uma linha para `Luta`, uma para `Disparo` e uma para `Magia`;
- listar apenas os nomes dos Poderes na ficha principal;
- manter textos longos apenas em `Descrição visual`, `Personalidade` e `Histórico` quando necessário;
- evitar repetir a mesma informação em blocos diferentes.

## Exterior e interior

`Descrição visual` registra apenas o que pode ser percebido olhando o personagem.

`Descrição mental`, `Desejos`, `Medos` e `Vínculos` registram elementos internos usados para interpretação.

> **Descrição mostra o exterior. Personalidade orienta decisões. Histórico fornece contexto.**

## Referências não são estado atual

O nome `Referências` foi escolhido para evitar confusão com o estado momentâneo da cena.

A ficha pode registrar `Vida [35]` e `Energia [20]` como capacidades estáveis, enquanto o estado da campanha registra os valores atuais consumidos ou perdidos.

## Flexibilidade

A estrutura pode crescer quando um personagem realmente exigir informação adicional, mas o modelo-base deve permanecer reconhecível.

Detalhes extensos de Poderes ficam em arquivos próprios e não devem ser incorporados integralmente à ficha principal.
