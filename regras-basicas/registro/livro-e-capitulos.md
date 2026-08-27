# Livro e Capítulos

Status: REFORMULAÇÃO / NÃO IMPLEMENTADO

Este arquivo define como preservar **o histórico canônico do que realmente aconteceu**.

Destino padrão:

```text
campanhas/<nome>/livro/
```

O Livro é diferente do Estado Atual.

```text
LIVRO
→ passado consolidado.

ESTADO ATUAL
→ presente necessário para continuar.
```

## O que o Livro registra

Registrar no Livro:

- ações realmente realizadas;
- decisões exercidas;
- falas relevantes;
- conflitos resolvidos;
- consequências;
- descobertas;
- mudanças de relação que realmente ocorreram;
- acontecimentos secretos que de fato aconteceram;
- mudanças de situação;
- passagem de tempo relevante;
- ordem causal necessária para entender a história.

## O que o Livro não registra como fato

Não transformar em acontecimento:

- intenção não executada;
- plano futuro;
- hipótese;
- possibilidade discutida;
- resultado ainda não julgado;
- metaconversa;
- discussão de regras;
- comando administrativo;
- versão corrigida ou anulada.

## Livro não é log de sessão

O capítulo pode ser escrito como narrativa consolidada.

Ele não precisa copiar literalmente:

```text
JOGADOR declarou...
OPOSITOR declarou...
Teste 1d20...
Narrador julgou...
```

Essas estruturas explicam como o jogo funcionou, mas o Livro registra a ficção resultante.

Exemplo:

```text
MESA
Jogador → tento abrir a porta sem fazer barulho.
Resultado → sucesso.

LIVRO
Corvin girou a maçaneta devagar e abriu a porta sem produzir mais que um leve roce das dobradiças.
```

## Preservar agência

A consolidação pode melhorar a forma literária, mas não pode mudar quem decidiu ou o que aconteceu.

Não pode:

- trocar o autor de uma ação;
- transformar recusa em aceitação;
- inventar uma decisão importante;
- inventar motivação decisiva não estabelecida;
- apagar uma decisão real porque atrapalha a prosa;
- transformar falha em sucesso ou sucesso em falha.

> **A forma pode melhorar. O cânone não pode mudar.**

## Interpretação literária

O Livro pode usar as regras de narração do Mestre para:

- ajustar ritmo;
- condensar repetição;
- organizar parágrafos;
- preservar voz das personagens;
- transformar declarações curtas em atuação coerente;
- completar nomes e detalhes que a personagem legitimamente conhecia;
- mostrar causa e consequência com clareza.

Isso continua sujeito à agência e ao conhecimento legítimo.

## Ações secretas

Se uma ação do Opositor realmente aconteceu fora da percepção dos protagonistas, ela pode fazer parte do cânone mesmo sem ser conhecida por eles.

A campanha pode optar por:

- registrar no Livro quando a estrutura literária permitir;
- manter primeiro no registro do Opositor e incorporá-la ao Livro depois;
- preservar a revelação para momento posterior.

A escolha de apresentação não muda a verdade do acontecimento.

## Fechar capítulo

Fechar capítulo significa:

```text
PARAR no último fato estabelecido
→ consolidar o trecho no Livro
→ atualizar Estado Atual
→ atualizar conhecimentos afetados
→ atualizar processos e prazos
→ atualizar Mundo somente se uma verdade estável mudou
→ atualizar Mestre/Opositor somente se seus dados mudaram
→ encerrar sem iniciar nova ficção
```

## Não fabricar um final

Ao fechar capítulo:

- não criar despedida que não aconteceu;
- não acrescentar cliffhanger artificial;
- não avançar até a próxima manhã;
- não executar evento futuro só para encerrar bem;
- não decidir reação ainda pendente.

O capítulo termina onde a ficção realmente parou.

## Numeração

Usar a convenção já existente na campanha.

Se não houver uma, pode-se adotar uma sequência simples:

```text
001.md
002.md
003.md
```

Antes de criar novo capítulo, verificar os arquivos existentes em `livro/` para não duplicar numeração.

## Correção de cânone

Se um capítulo salvo contiver erro e a correção for aprovada, substituir a versão incorreta e alinhar somente as fontes afetadas.

Não manter duas versões contraditórias como igualmente verdadeiras.

Exemplo:

```text
VERSÃO ERRADA
→ Ravena saiu às 22h.

CORREÇÃO CANÔNICA
→ Ravena saiu às 23h.
```

Depois da correção, qualquer Estado, prazo ou referência que dependa desse horário deve ser ajustado.

## Capítulo x conhecimento

O fato de algo aparecer no Livro não significa que todas as personagens sabem disso.

```text
LIVRO SABE
≠
PERSONAGEM SABE
```

Conhecimento continua sendo controlado por suas fontes próprias.

## Capítulo x estado atual

Depois do fechamento, o Estado Atual deve representar somente o ponto final do capítulo.

Exemplo:

```text
LIVRO
→ registra toda a noite.

ESTADO ATUAL
→ manhã seguinte, local, presentes, condições e processos ainda vivos.
```

## Regra final

> **O Livro é a memória histórica da campanha: registra o que realmente aconteceu, em forma narrativa consolidada, sem copiar o chat nem alterar agência. Fechar capítulo preserva esse passado e atualiza as fontes que precisam continuar válidas, sem jogar nenhum acontecimento novo durante o salvamento.**