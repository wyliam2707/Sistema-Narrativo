# Poderes

Status: EM DESENVOLVIMENTO

No `novo-motor/`, a ficha principal registra **somente os nomes dos Poderes que o personagem possui**.

Exemplo:

```text
## Poderes
- Teleporte
- Escudo Arcano
- Petrificação
- Cura
```

A ficha não deve carregar a descrição mecânica completa de todos os Poderes ao mesmo tempo.

> **A ficha responde quais Poderes existem. O arquivo do Poder responde como ele funciona.**

## Arquivo próprio por Poder

Cada Poder deverá possuir uma descrição própria fora da ficha do personagem.

Esse arquivo deverá concentrar as informações necessárias para usar o Poder, como, quando aplicável:

- alcance;
- alvo;
- dano;
- efeito;
- custo;
- duração;
- Defesa envolvida;
- limitações;
- propriedades especiais.

O formato definitivo desses arquivos ainda será definido durante o desenvolvimento do novo motor.

## Consulta sob demanda

Quando o jogador declarar que deseja usar um Poder, o fluxo previsto é:

```text
1. consultar a ficha do personagem;
2. mostrar a lista de Poderes disponíveis;
3. o jogador escolhe um deles;
4. consultar apenas o arquivo do Poder escolhido;
5. mostrar ao jogador o efeito e os parâmetros relevantes;
6. o jogador confirma o uso;
7. resolver a ação.
```

Isso evita carregar na ficha principal detalhes que não são necessários para a decisão atual.

## Poder não é Perícia

`Arcano` representa conhecimento sobre magia.

`Magia`, no bloco de Ataques, representa competência de combate quando um efeito mágico precisa ser imposto contra oposição.

Um Poder representa uma capacidade específica disponível ao personagem.

Exemplo:

```text
Arcano [4]     → entende profundamente magia.
Magia [+2]     → possui determinada competência para aplicar magia em conflito.
Petrificação   → é um Poder que pode ser escolhido e consultado quando usado.
```

Essas informações não são automaticamente equivalentes nem se substituem.

## Poderes e Ataques

Um Poder pode produzir dano, controle, movimento, proteção, cura ou qualquer outro efeito compatível com sua descrição.

Quando o Poder for usado como ataque, a resolução consulta a forma apropriada de ataque e a Defesa válida para aquele efeito.

As regras completas de alcance, contato, acerto, Defesas, dano e demais propriedades permanecem em desenvolvimento dentro de `../resolucao/`.
