# Narração

Status: EM MIGRAÇÃO

Esta pasta reúne as regras que respondem à pergunta:

> **Como os acontecimentos resolvidos são apresentados ao jogador e transformados em cena?**

## Estado da migração

A estrutura nova está sendo construída sem apagar os arquivos antigos.

Enquanto uma regra de apresentação ainda não tiver sido reescrita e aprovada nesta pasta, o arquivo antigo correspondente pode continuar sendo consultado apenas nos pontos ainda não substituídos.

## Responsabilidades desta área

Esta pasta deverá concentrar, progressivamente:

- narração e escrita padrão;
- ritmo de cena;
- ponto de parada;
- quantidade de avanço por declaração;
- diferença entre jogo ao vivo e texto literário consolidado;
- apresentação de fala, pensamento e informação perceptível;
- controle de foco e clareza espacial;
- limites para não narrar decisões voluntárias do jogador humano.

## Relação com outras áreas

- `../personas/` define quem decide;
- `../resolucao/` define o que acontece;
- `../operacao/` define quando apresentar e quando devolver controle;
- `narracao/` define como o acontecimento estabelecido é mostrado.

O NARRADOR não deve usar estilo narrativo para alterar resultado, criar oposição retroativa ou assumir decisões que pertencem aos jogadores.

## Direção narrativa da campanha

Toda campanha atual registra sua direção narrativa nas fontes definidas por `../criacao/README.md`.

O resumo canônico da direção narrativa fica no `README.md` da própria campanha. Detalhes adicionais só devem existir em outro arquivo quando houver necessidade concreta e uma fonte principal claramente definida.

A direção específica da campanha pode complementar ou alterar aspectos do padrão geral de escrita.

> **A campanha define o estilo local; o sistema fornece o padrão herdado.**

## Fonte antiga ainda útil

Enquanto esta pasta não possuir uma substituição completa aprovada para o estilo geral, pode ser consultado:

```text
../narracao-e-escrita-padrao.md
```

Esse arquivo é fonte histórica ainda útil somente nos pontos de estilo não substituídos. Ele não pode reintroduzir estrutura antiga de campanha, controle, resolução ou persistência.

## Livro e jogo ao vivo

A apresentação durante a sessão e a consolidação literária cumprem funções diferentes.

```text
JOGO AO VIVO
→ apresenta somente o necessário para a situação atual e devolve agência aos jogadores

LIVRO
→ consolida depois aquilo que realmente aconteceu
```

As regras de consolidação pertencem a `../persistencia/livro.md` e `../persistencia/fechamento-de-capitulo.md`.

> **Forma melhora a experiência; não reescreve o acontecimento.**
