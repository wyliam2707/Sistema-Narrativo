# Organização Visual das Fichas

Status: EM DESENVOLVIMENTO

A prioridade é permitir leitura rápida por jogador humano, narrador e jogador IA.

> **Cada bloco deve responder a uma função clara e evitar repetir regra já definida em Poderes ou Passivos.**

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
Corpo — POD [ ] | HAB [ ] | RES [ ]
Mente — POD [ ] | HAB [ ] | RES [ ]

## Perícias
Comuns
Esportes [ ] | Exploração [ ] | Expressão [ ] | Sociedade [ ]
Investigação [ ] | Crime [ ] | Ofícios [ ] | Idiomas [ ]

Somente treinadas
Arcano [ ] | Ocultismo [ ] | Natureza [ ] | Medicina [ ]
Engenharia [ ] | Ciência [ ] | Tecnologia [ ] | História [ ]

## Poderes
- Golpe [ ]
- Disparo [ ]
- Teleporte [ ]

## Passivos
- RD [ ]
- Vida Extra [ ]
- Proteção [ ]

## Derivados
Vida [ ] | Energia [ ]
Esquiva [ ] | Percepção [ ] | Vontade [ ] | Fortitude [ ] | RD [ ]
Deslocamento: [ ]

## Recursos
- Recurso narrativo relevante

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

- manter Atributos em duas linhas espelhadas;
- manter as Perícias nos grupos definidos em `pericias.md`;
- listar Poderes apenas pelo nome e `[X]` registrado na ficha;
- listar Passivos apenas pelo nome e valor quando houver;
- mostrar Derivados já consolidados depois de Poderes e Passivos;
- não criar bloco separado de Ataques;
- não criar bloco separado de Arsenal;
- não repetir dano, alcance, ampliações ou regras completas dos Poderes na ficha;
- manter textos longos apenas nos blocos narrativos quando necessário.

## Poderes sob demanda

Quando um Poder for escolhido, o narrador abre apenas o arquivo correspondente em `poderes/` e mostra ao jogador sua descrição operacional.

A ficha não carrega todos os detalhes dos Poderes ao mesmo tempo.

## Passivos

Passivos ficam visíveis na ficha porque são capacidades permanentes ou estáveis. Quando alteram Vida, Esquiva, Percepção, RD ou outro Derivado, o valor final já aparece consolidado em `Derivados`.

## Derivados não são estado atual

`Derivados` registra capacidades máximas ou consolidadas.

Exemplo:

```text
Ficha
Vida [50] | Energia [20]

Estado atual
Vida [31/50] | Energia [7/20] | Barreira 10 PV
```

## Exterior e interior

`Descrição visual` registra o que pode ser percebido olhando o personagem.

`Personalidade` e `Histórico` orientam interpretação e contexto, sem criar regras mecânicas adicionais.

## Flexibilidade

A ficha pode crescer quando um personagem realmente exigir informação narrativa adicional, mas o núcleo mecânico deve continuar reconhecível:

```text
Atributos → Perícias → Poderes → Passivos → Derivados
```
