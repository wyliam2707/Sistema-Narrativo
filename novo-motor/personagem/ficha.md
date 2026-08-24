# Ficha de Personagem

Status: EM DESENVOLVIMENTO

Esta é a ficha-base experimental do `novo-motor/`.

A construção mecânica do personagem usa somente:

```text
Atributos
+ Perícias
+ Poderes
+ Passivos
= Valores Derivados
```

Armas, armaduras, escudos, focos, equipamentos e outras manifestações não formam uma camada mecânica separada. Quando relevantes, são a descrição narrativa de um Poder ou Passivo.

> **A ficha mostra o que o personagem possui. O arquivo de cada Poder ou Passivo mostra como ele funciona.**

## Modelo-base

```text
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
- Utilidade [ ]

## Passivos
- RD [ ]
- Vida Extra [ ]
- Proteção [ ]
- Sentido-Aranha

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

## Atributos

```text
Corpo — POD [X] | HAB [X] | RES [X]
Mente — POD [X] | HAB [X] | RES [X]
```

- `POD` — intensidade, potência e capacidade de produzir efeito;
- `HAB` — precisão, controle e qualidade de execução;
- `RES` — capacidade de suportar, resistir e continuar funcionando.

Corpo e Mente definem a natureza da capacidade.

## Perícias

Perícias representam treinamento, conhecimento, exploração e interação com o mundo. Elas não são uma lista separada de ataques.

A abordagem do personagem determina qual Perícia pode ser aplicável à situação.

## Poderes

Poderes são efeitos ativos. A ficha registra nome e limite:

```text
Golpe [2]
Disparo [3]
Explosão [2]
Teleporte [5]
Utilidade [2]
```

Nos Poderes, `[X]` é o máximo de Energia que pode ser investido em um único uso.

A descrição completa fica no arquivo individual em `poderes/`.

Fluxo:

```text
listar Poderes
→ jogador escolhe
→ abrir somente o arquivo escolhido
→ mostrar base e ampliações
→ jogador declara o uso
→ se couber na base, resolver
→ se exigir ampliação, informar custo
→ aguardar confirmação
→ gastar Energia e resolver
```

O narrador não escolhe automaticamente uma ampliação que consuma Energia.

## Passivos

Passivos são capacidades permanentes ou estáveis já incorporadas ao personagem.

```text
RD [3]
Vida Extra [30]
Proteção [2]
Sentido-Aranha
Imortalidade
Regeneração [2]
```

Nos Passivos, `[X]` tem o significado definido pela própria descrição e não representa limite de Energia.

A regra completa de cada Passivo fica em `passivos/`.

## Valores Derivados

Depois de Atributos, Perícias, Poderes e Passivos estarem definidos, a ficha consolida:

```text
Vida [ ] | Energia [ ]
Esquiva [ ] | Percepção [ ] | Vontade [ ] | Fortitude [ ] | RD [ ]
Deslocamento: [ ]
```

Passivos que alteram esses números já entram no valor final.

Exemplo:

```text
Proteção [2] → Esquiva +2 e Percepção +2
Vida Extra [30] → Vida +30
RD [3] → RD final +3
```

As fórmulas-base ainda não fechadas não devem ser inventadas para preencher campos vazios.

## Manifestação narrativa

O mesmo Poder ou Passivo pode ter aparências diferentes sem mudar sua mecânica.

```text
Golpe → soco, espada, garra, bastão.
Disparo → arco, pistola, batarang, laser.
RD → armadura, pele de aço, traje tecnológico, campo místico.
Proteção → escudo, reflexos ampliados, sentidos sobrenaturais, campo defensivo.
```

A descrição pode importar para a ficção, mas não exige uma tabela separada de Arsenal.

## Estado atual

A ficha guarda capacidades máximas e valores consolidados. O estado momentâneo permanece separado.

```text
Ficha
Vida [50] | Energia [20]

Estado atual
Vida [31/50] | Energia [7/20] | Barreira 10 PV
```

## Recursos narrativos

`Recursos` registra infraestrutura, acesso ou meios relevantes capazes de mudar possibilidades na ficção, sem virar inventário mecânico.

Exemplos: Batcaverna, Batmóvel, rede de contatos.

## Personalidade e Histórico

Esses blocos existem para interpretação e contexto e não formam uma camada mecânica adicional.

## Campo ainda não definido

Campo desconhecido permanece vazio.

```text
POD [ ]
```

não é igual a:

```text
POD [0]
```

> **Zero é valor real, nunca marcador de pendência.**
