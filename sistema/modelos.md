# Modelos de Arquivos

Estes modelos existem para tornar a criação de aventuras consistente e rápida.

## 1. Ficha — personagem Central

```text
# Nome

Importância: Central
Idade: ...
Conceito: ...
Descrição: aparência breve | personalidade em palavras-chave

ATR: FOR [ ] | AGI [ ] | RES [ ] | MEN [ ] | VON [ ]
PER: Perícia [+ ] / Perícia [+ ] / ...
Poder [Fonte opcional] [ ] => uso / uso / especialização [ ]
Poder [ ] => ...
EQP: somente equipamentos recorrentes/relevantes
REL: Pessoa [+/- ] / Pessoa [+/- ]

## Personalidade e tendências
- ...

## Desejos/objetivos atuais
- ...

## Medos/limites relevantes
- ...

## História consolidada relevante
- somente fatos necessários para interpretar o personagem; detalhes completos ficam no livro/cronologia
```

A ficha Central pode ser mais descritiva porque precisa sustentar agência e continuidade por muito tempo.

## 2. Ficha — personagem Relevante

```text
# Nome

Importância: Relevante
Idade: ...
Conceito: ...
Descrição: aparência breve | personalidade breve

ATR: FOR [ ] | AGI [ ] | RES [ ] | MEN [ ] | VON [ ]
PER: ...
Poder [ ] => ...
EQP: ...
REL: ...

Objetivo/Tendência: uma ou poucas linhas quando necessário.
```

Adicionar detalhes apenas quando passarem a importar.

## 3. Figurante

Figurantes não precisam de arquivo individual na maioria dos casos.

Exemplos:

```text
Guarda — Humano [1] | Soldado [+2] | rifle / colete
```

```text
Invocação — Demônio [3] | FOR [4] | VON [1]
```

O modelo-base define todos os atributos. Só registrar exceções.

## 4. STATUS atual

```text
# Estado Atual

Momento: fim/início do capítulo ...
Local principal: ...
Situação imediata: ...

## Personagem Central/Relevante
VIDA: Ileso | Ferido | Grave | Crítico | Incapacitado
ENERGIA: Pleno | Metade | Limite | Crítico
COND: Nenhuma / condição 1 / condição 2
EQP temporário: dano, falta ou alteração circunstancial relevante
Efeitos ativos: ...
Local: ...

## Outro personagem
...

## Pontas imediatas
- ameaças em andamento;
- decisões pendentes;
- prazos imediatos;
- fatos que precisam ser lembrados ao retomar.
```

`Crítico` em ENERGIA significa: resta aproximadamente **uma última ação relevante** antes de esgotamento, falta de recurso ou colapso coerente com o personagem.

## 5. Relação complexa

```text
# Personagem A & Personagem B

Status: canônico / planejado / rascunho

## Situação atual
- A → B: [+ ]
- B → A: [+ ]

## Natureza do vínculo
- ...

## Dinâmica
- como A tende a agir com B;
- como B tende a agir com A;
- conflitos e compatibilidades relevantes.

## Evolução consolidada
- fatos que realmente aconteceram.

## Possibilidades/rumos planejados
- ideias futuras que ainda NÃO são fatos canônicos.
```

Nunca tratar trajetória planejada como acontecimento já ocorrido.

## 6. Cronologia

```text
## Capítulo / período
Local: ...
Presentes: ...
Acontecimento: ...
Consequência: ...
Conhecimento adquirido:
- Personagem A passou a saber ...
- Personagem B ainda não sabe ...
```

O campo de conhecimento é importante para impedir metaconhecimento acidental.

## 7. README de uma aventura

```text
# Nome da Aventura

## Premissa
...

## Personagens centrais
- ...

## Como narrar
Ler antes:
- diretrizes/...

## Hierarquia de cânone
1. correção explícita mais recente;
2. livro/capítulos consolidados;
3. diretrizes;
4. personagens/mundo/relacionamento;
5. cronologia;
6. estado atual;
7. rascunhos antigos.

## Ponto atual
Consultar: `estado/atual.md`

## Regra de continuidade
Nunca continuar apenas pela memória de outro chat; consultar as fontes desta aventura.
```

## 8. Princípio de economia

Não preencher campos apenas porque o modelo existe.

> **Registrar somente o que ajuda o narrador a decidir, lembrar ou manter continuidade.**

Central recebe detalhe alto; Relevante recebe detalhe proporcional ao papel; Figurante recebe apenas o necessário para a cena.
