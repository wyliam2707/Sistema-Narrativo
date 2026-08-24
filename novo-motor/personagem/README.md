# Personagem — Novo Motor

Status: EM DESENVOLVIMENTO

Esta pasta contém a estrutura experimental de personagens do `novo-motor/`.

## Núcleo mecânico

A construção mecânica usa somente:

```text
Atributos
+ Perícias
+ Poderes
+ Passivos
= Valores Derivados
```

Não existe mais uma camada mecânica separada de Arsenal ou Ataques prontos por equipamento.

Armas, armaduras, escudos, focos, tecnologia, mutações e outras manifestações descrevem narrativamente um Poder ou Passivo quando necessário.

## Estrutura atual da ficha

```text
1. Descrição
2. Atributos
3. Perícias
4. Poderes
5. Passivos
6. Valores Derivados
7. Recursos narrativos
8. Personalidade
9. Histórico e conhecimento
```

Os blocos de Descrição, Recursos, Personalidade e Histórico existem para interpretação e contexto. O núcleo mecânico permanece Atributos + Perícias + Poderes + Passivos.

## Atributos

```text
Corpo — POD [ ] | HAB [ ] | RES [ ]
Mente — POD [ ] | HAB [ ] | RES [ ]
```

- `POD` — potência e intensidade;
- `HAB` — execução, precisão e controle;
- `RES` — resistência e capacidade de suportar.

## Perícias

Perícias representam áreas amplas de treinamento, conhecimento e experiência. A abordagem da ação determina qual Perícia pode ser aplicável.

## Poderes

Poderes são efeitos ativos. A ficha registra nome e limite de Energia:

```text
Golpe [2]
Disparo [3]
Explosão [2]
Teleporte [5]
```

Nos Poderes, `[X]` é o máximo de Energia que pode ser investido em um único uso.

Cada Poder tem arquivo próprio em:

```text
personagem/poderes/
```

O narrador consulta somente o Poder escolhido pelo jogador. Se uma intenção exigir gasto de Energia, informa o custo e aguarda confirmação antes de aplicar a ampliação.

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

Cada Passivo tem arquivo próprio em:

```text
personagem/passivos/
```

Nos Passivos, `[X]` tem o significado definido pela própria descrição e não representa limite de Energia.

## Valores Derivados

Depois dos quatro blocos mecânicos, a ficha consolida os valores usados constantemente:

```text
Vida [ ] | Energia [ ]
Esquiva [ ] | Percepção [ ] | Vontade [ ] | Fortitude [ ] | RD [ ]
Deslocamento: [ ]
```

Passivos que alteram esses números já entram no valor final mostrado.

## Recursos narrativos

Recursos registram infraestrutura, acesso ou meios relevantes, como base, veículo ou rede de contatos. Não formam inventário mecânico comum.

## Arquivos principais

- `ficha.md` — modelo-base atual;
- `atributos.md` — POD, HAB e RES em Corpo e Mente;
- `pericias.md` — lista e função das Perícias;
- `poderes.md` e `poderes/` — regras gerais e arquivos individuais dos Poderes;
- `passivos.md` e `passivos/` — regras gerais e arquivos individuais dos Passivos;
- `criacao.md` — fluxo de criação;
- `organizacao-visual.md` — apresentação da ficha.

## Conflitos herdados

Arquivos herdados ainda podem conter conceitos anteriores. Quando houver conflito direto, esta arquitetura consolidada e os arquivos acima têm precedência dentro do `novo-motor/`.

O conteúdo canônico em `sistema/` permanece separado e não deve ser alterado sem decisão explícita de migração.
