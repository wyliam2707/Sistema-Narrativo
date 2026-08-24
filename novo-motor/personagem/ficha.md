# Ficha de Personagem

Status: EM DESENVOLVIMENTO

Esta é a ficha-base experimental do `novo-motor/`.

Ela foi organizada para consulta rápida por jogador, narrador e jogador IA. Cada bloco responde a uma função específica e evita misturar descrição, interpretação e resolução.

> **A ficha registra quem o personagem é e suas referências estáveis. O estado atual da cena permanece separado.**

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

## 1. Descrição

O primeiro bloco identifica o personagem e registra apenas aquilo que deve estar disponível imediatamente para reconhecê-lo e enquadrá-lo na estrutura da campanha.

`Nome:` pode reunir codinome e identidade pessoal na mesma linha:

```text
Nome: Ravena — Rachel Roth
Nome: Batman — Bruce Wayne
```

`Importância:` registra o peso estrutural do personagem na campanha.

`Controle:` registra quem normalmente possui agência sobre suas decisões.

`Descrição visual:` contém apenas aquilo que pode ser percebido ao olhar o personagem: corpo, rosto, cabelo, pele, marcas, roupas, acessórios, postura observável e outros elementos visuais relevantes.

Não colocar nesse campo personalidade, intenção, desejo, medo ou explicação psicológica.

> **Descrição visual mostra o que se vê.**

## 2. Atributos

Os seis Atributos aparecem em duas linhas espelhadas, uma para Corpo e outra para Mente:

```text
Corpo — POD [X] | HAB [X] | RES [X]
Mente — POD [X] | HAB [X] | RES [X]
```

As três funções são as mesmas nos dois domínios:

- `POD` — Poder: intensidade, potência e capacidade de impor ou produzir efeito;
- `HAB` — Habilidade: precisão, controle e qualidade de execução;
- `RES` — Resistência: capacidade de suportar, resistir e continuar funcionando.

O domínio define a natureza da capacidade:

```text
Corpo → capacidades físicas.
Mente → capacidades mentais, sociais, psíquicas ou mágicas quando pertinente.
```

Assim, `POD`, `HAB` e `RES` não representam ações específicas. Eles representam funções gerais que podem ser aplicadas a situações diferentes conforme o mecanismo da cena.

Exemplos de leitura:

```text
POD Corpo → força e potência física.
HAB Corpo → precisão, coordenação, mobilidade e técnica física.
RES Corpo → resistência a dano, fadiga e efeitos físicos.

POD Mente → força de imposição, presença ou potência mental/mágica.
HAB Mente → percepção, raciocínio, análise e controle mental/mágico.
RES Mente → resistência a medo, pressão, dominação e outros efeitos mentais.
```

As fórmulas definitivas de resolução ainda pertencem ao desenvolvimento de `../resolucao/`.

> **Poder determina intensidade. Habilidade determina execução. Resistência determina oposição. Corpo e Mente determinam a natureza da capacidade.**

## 3. Perícias

Perícias representam áreas amplas de conhecimento, experiência, exploração e interação com o mundo.

Elas **não representam combate**.

Uma ação não pertence obrigatoriamente a uma única Perícia. A abordagem utilizada determina quais Perícias podem fazer sentido.

Exemplo:

```text
Seguir rastros
→ Exploração, pela leitura do terreno e deslocamento.
→ Investigação, pela análise de pistas e padrões.
→ Natureza, pela leitura de sinais naturais e animais.
```

### Comuns

```text
Esportes [X] | Exploração [X] | Expressão [X] | Sociedade [X]
Investigação [X] | Crime [X] | Ofícios [X] | Idiomas [X]
```

Podem ser tentadas sem treinamento quando a ação estiver dentro de conhecimento ou experiência comum plausível.

### Somente treinadas

```text
Arcano [X] | Ocultismo [X] | Natureza [X] | Medicina [X]
Engenharia [X] | Ciência [X] | Tecnologia [X] | História [X]
```

Quando uma tarefa realmente depende desses campos especializados, é necessário treinamento correspondente.

`Arcano` cobre magia, feitiços, runas, encantamentos, itens mágicos, artefatos, alquimia e funcionamento de efeitos mágicos.

`Ocultismo` cobre demônios, espíritos, mortos-vivos, cultos, possessões, entidades ocultas, maldições e seres ou fenômenos sobrenaturais relacionados.

> **A ação define o problema. A abordagem define a Perícia aplicável.**

## 4. Referências

Este bloco reúne valores estáveis de consulta rápida. Ele não representa o estado momentâneo da cena.

Padrão:

```text
Vida [ ] | Energia [ ] | Deslocamento: Curto | Visão: Comum longa / Escuro curta
Defesas - Esquiva [ ] | Vontade [ ] | Fortitude [ ] | RD: Geral [2] | Fogo [10]
```

`Visão:` pode registrar mais de um modo e o alcance de cada um.

Exemplos:

```text
Visão: Comum longa
Visão: Comum longa / Escuro curta
Visão: Comum longa / Térmica média / Mágica curta
```

As três Defesas são:

- `Esquiva` — evitar que um ataque ou efeito alcance o personagem;
- `Fortitude` — bloquear, suportar ou resistir fisicamente quando a ficção permitir;
- `Vontade` — resistir a efeitos que tentem dominar, alterar ou impor algo à mente.

A Defesa utilizada depende de como o personagem enfrenta o efeito e do que a ficção permite. O personagem não escolhe livremente a maior Defesa apenas porque o valor é melhor.

`RD` registra Redução de Dano geral ou específica quando existir.

Exemplo:

```text
RD: Geral [2] | Fogo [10]
```

As fórmulas exatas de cálculo das Defesas e as propriedades de ataques que restringem determinada Defesa ainda pertencem ao desenvolvimento de `resolucao/`.

## 5. Ataques

O bloco de Ataques mantém uma linha pronta para cada forma básica de ataque:

```text
Luta [bônus] / arma / dano / crítico / alcance
Disparo [bônus] / arma / dano / crítico / alcance
Magia [bônus] / arma ou efeito / dano / crítico / alcance
```

Exemplo:

```text
Luta [+6] / Espada mágica / 1d8+3 + 1d6 fogo / Crítico 20 x2 / Toque
```

`Luta` cobre ataques e manobras corporais, como golpear ou agarrar.

`Disparo` cobre ataques à distância por armas ou meios equivalentes.

`Magia` cobre a competência de impor efeitos mágicos em conflito.

`Arcano` e `Magia` não são a mesma coisa: `Arcano` é conhecimento sobre magia; `Magia` é competência de ataque quando um efeito mágico exige essa forma de resolução.

Nem todo ataque precisa causar dano. Quando um campo não se aplicar, ele pode ficar marcado como `—`.

## 6. Poderes

A ficha lista apenas os nomes dos poderes disponíveis ao personagem.

```text
## Poderes
- Teleporte
- Escudo Arcano
- Petrificação
- Cura
```

Os detalhes completos de cada poder ficam fora da ficha, em arquivo próprio, para serem consultados apenas quando necessários.

Fluxo de uso previsto:

```text
Jogador declara que quer usar um poder
→ sistema mostra a lista de Poderes da ficha
→ jogador escolhe um Poder
→ sistema consulta o arquivo desse Poder e mostra o efeito aplicável
→ jogador confirma
→ a ação é resolvida
```

O arquivo detalhado do Poder deverá registrar informações como alcance, dano, efeito, custo e demais propriedades necessárias. O formato definitivo desses arquivos será criado separadamente.

## 7. Recursos

`Recursos` registra meios, infraestrutura, acesso ou bens relevantes capazes de mudar possibilidades na ficção.

Não é inventário de objetos comuns.

Exemplos:

```text
- Batcaverna — laboratório, oficina e computadores
- Batmóvel — veículo blindado
- Rede de contatos
```

Equipamentos já consolidados em Ataques ou Poderes não precisam ser repetidos aqui apenas para formar uma lista de posses.

## 8. Personalidade

Este bloco registra quem o personagem é por dentro e serve diretamente à interpretação por jogador humano ou jogador IA.

```text
Descrição mental:
Desejos:
Medos:
Vínculos:
```

`Descrição mental:` registra temperamento, modo de pensar, valores, tendências de comportamento e formas habituais de reagir.

`Desejos:` registra aquilo que o personagem busca, quer proteger, conquistar, preservar ou experimentar.

`Medos:` registra aquilo que teme enfrentar, perder ou se tornar.

`Vínculos:` registra pessoas, grupos, lugares ou relações que realmente influenciam suas decisões.

> **Descrição visual mostra o exterior. Personalidade explica o interior.**

## 9. Histórico e conhecimento

`Histórico relevante:` não é uma biografia completa. Registra apenas fatos do passado que ainda importam para interpretar corretamente o personagem no presente.

`Conhecimento relevante:` registra informações que o personagem sabe e que podem alterar suas decisões futuras.

A separação é importante:

```text
Histórico relevante → o que aconteceu com o personagem.
Conhecimento relevante → o que o personagem sabe agora.
```

Isso ajuda a impedir que um jogador IA use informações que pertencem ao narrador, ao jogador humano ou a outro personagem.

## Estado atual não pertence a Referências

`Referências` guarda capacidades estáveis e valores máximos ou consolidados.

Informações momentâneas como Vida perdida, Energia consumida, condições, localização, ferimentos temporários e efeitos ativos devem permanecer na camada de estado/persistência da campanha.

Exemplo:

```text
Ficha / Referências
Vida [35] | Energia [20]

Estado atual
Vida [23/35] | Energia [8/20] | Imobilizado
```

> **A ficha diz quem o personagem é e do que dispõe. O estado atual diz como ele está agora.**

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
