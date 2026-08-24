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

> **A ficha mostra o que o personagem possui. O arquivo de cada Poder mostra como ele funciona.**

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

## 1. Atributos

Os seis Atributos aparecem em duas linhas espelhadas:

```text
Corpo — POD [X] | HAB [X] | RES [X]
Mente — POD [X] | HAB [X] | RES [X]
```

- `POD` — intensidade, potência e capacidade de produzir efeito;
- `HAB` — precisão, controle e qualidade de execução;
- `RES` — capacidade de suportar, resistir e continuar funcionando.

O domínio define a natureza da capacidade:

```text
Corpo → capacidades físicas.
Mente → capacidades mentais, sociais, psíquicas ou mágicas quando pertinente.
```

## 2. Perícias

Perícias representam áreas amplas de conhecimento, experiência, exploração e interação com o mundo.

Elas não são uma lista de ataques. A abordagem usada pelo personagem determina qual Perícia pode ser aplicável à situação.

### Comuns

```text
Esportes [X] | Exploração [X] | Expressão [X] | Sociedade [X]
Investigação [X] | Crime [X] | Ofícios [X] | Idiomas [X]
```

### Somente treinadas

```text
Arcano [X] | Ocultismo [X] | Natureza [X] | Medicina [X]
Engenharia [X] | Ciência [X] | Tecnologia [X] | História [X]
```

## 3. Poderes

Poderes são efeitos ativos.

A ficha registra apenas o nome e o limite de Energia disponível para aquele Poder:

```text
Golpe [2]
Disparo [3]
Explosão [2]
Teleporte [5]
```

Nos Poderes ativos, `[X]` representa o máximo de Energia que pode ser investido em um único uso.

A descrição mecânica completa fica no arquivo individual do Poder em:

```text
personagem/poderes/
```

Quando o jogador declara que quer usar um Poder:

```text
1. listar os Poderes da ficha;
2. o jogador escolhe um deles;
3. consultar apenas o arquivo do Poder escolhido;
4. mostrar efeito-base e ampliações;
5. o jogador declara o uso;
6. se couber no padrão, resolver com custo 0;
7. se exigir ampliação, informar o custo;
8. aguardar confirmação;
9. somente então gastar Energia e resolver.
```

O narrador nunca escolhe automaticamente uma ampliação que consuma Energia.

## 4. Passivos

Passivos são capacidades permanentes ou estáveis que já fazem parte do personagem.

Exemplos:

```text
RD [3]
Vida Extra [30]
Proteção [2]
Sentido-Aranha
Imortalidade
Regeneração [2]
```

Passivos não usam a regra de limite de Energia dos Poderes ativos. Quando possuem `[X]`, o próprio Passivo define o significado desse valor.

Exemplos:

```text
RD [3] → reduz 3 do dano recebido.
Vida Extra [30] → +30 Vida máxima.
Proteção [2] → +2 Esquiva e +2 Percepção.
Sentido-Aranha → não pode ser pego desprevenido.
Imortalidade → não morre de velhice.
Regeneração [2] → recupera 2 de Vida por hora.
```

A lista consolidada fica em `passivos.md`.

## 5. Valores Derivados

Depois de Atributos, Perícias, Poderes e Passivos estarem definidos, a ficha consolida os valores usados constantemente durante o jogo.

```text
Vida [ ] | Energia [ ]
Esquiva [ ] | Percepção [ ] | Vontade [ ] | Fortitude [ ] | RD [ ]
Deslocamento: [ ]
```

Os Passivos que alteram esses números já entram no valor final mostrado aqui.

Exemplo:

```text
Proteção [2]
→ Esquiva +2
→ Percepção +2

Vida Extra [30]
→ Vida +30

RD [3]
→ RD final +3
```

As fórmulas-base de Vida, Energia, Esquiva, Percepção e demais derivados continuam em desenvolvimento. Não preencher valores ainda não definidos com regras inventadas.

## 6. Manifestação narrativa

O mesmo Poder ou Passivo pode ter aparências diferentes sem mudar sua mecânica.

Exemplos:

```text
Golpe → soco, espada, garra, bastão, lâmina de energia.
Disparo → arco, pistola, batarang, laser, raio.
RD → armadura, pele de aço, traje tecnológico, campo místico.
Proteção → escudo, reflexos ampliados, sentidos sobrenaturais, campo defensivo.
```

A descrição pode importar para a ficção, mas não exige uma tabela separada de arsenal.

## 7. Estado atual

A ficha guarda capacidades máximas e valores consolidados.

O estado momentâneo da cena permanece separado:

```text
Ficha
Vida [50] | Energia [20]

Estado atual
Vida [31/50] | Energia [7/20] | Barreira 10 PV
```

## 8. Recursos narrativos

`Recursos` registra infraestrutura, acesso ou meios relevantes capazes de mudar possibilidades na ficção, sem virar inventário mecânico.

Exemplos:

```text
Batcaverna
Batmóvel
Rede de contatos
```

## 9. Personalidade e Histórico

Esses blocos continuam separados da construção mecânica e existem para interpretação do personagem.

`Descrição visual` mostra o exterior.

`Personalidade` registra modo de pensar, desejos, medos e vínculos.

`Histórico relevante` registra fatos do passado que ainda importam.

`Conhecimento relevante` registra aquilo que o personagem sabe atualmente.

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
