# Início e Retomada

Status: REFORMULAÇÃO / NÃO IMPLEMENTADO

Este arquivo define como uma IA começa ou retoma uma campanha usando `regras-basicas/` sem depender de `sistema/`.

> **Carregar somente o necessário para jogar corretamente. Não transformar preparação em uma segunda sessão.**

## Entrada

No primeiro contato:

```text
ler regras-basicas/README.md
→ compreender Núcleo, Jogador, Mestre, Opositor e Registro
→ Nova campanha ou Continuar?
```

Não é necessário reler todos os arquivos em toda resposta. Durante o jogo, consultar a regra específica somente quando ela realmente importar ou houver dúvida.

## Nova campanha

Seguir:

```text
CRIACAO-DE-CAMPANHA.md
```

A criação segue:

```text
PASSO 01 — Narrativa da Campanha
PASSO 02 — Temporada
PASSO 03 — Fichas
```

A ficção só começa quando existir informação suficiente para apresentar a primeira cena sem inventar escolhas ou fatos estruturais essenciais.

## Continuar campanha

Abrir:

```text
campanhas/<nome>/README.md
```

Depois carregar, no mínimo:

```text
mestre/narrativa.md
+ mestre/roteiro.md
+ estado/atual.md
+ fichas das personagens atualmente relevantes
```

Essas fontes possuem funções diferentes:

```text
NARRATIVA DA CAMPANHA
→ foco persistente, gênero, tom, experiência desejada e premissas gerais.

ROTEIRO DA TEMPORADA
→ situação, trama de fundo, prazo, miniquests, direção atual e condição de encerramento.

FICHA DA PERSONAGEM
→ principal fonte de interpretação, capacidades, relações e conhecimento consolidado.

ESTADO ATUAL
→ situação temporária, marcas, Mana, posição e processos atuais.

LIVROS / MUNDO / OUTROS ARQUIVOS
→ contexto externo consultado quando necessário.
```

A Narrativa impede que a campanha perca sua identidade. O Roteiro impede que a temporada perca seu arco atual. Nenhum dos dois determina resultados nem substitui julgamento.

Conhecimento registrado na ficha já faz parte da personagem. Não apresentar novamente como descoberta, nem reiniciar automaticamente um conflito de aceitação ou aprendizado que já esteja consolidado.

Consultar outros arquivos de `mundo/`, `mestre/`, `opositor/`, conhecimento ou Livro somente quando forem necessários para a cena ou para resolver dúvida real.

Não pedir novamente informação que já esteja registrada em fonte canônica da campanha.

## Campanha em criação

```text
CRIAÇÃO: EM ANDAMENTO
→ retomar do ponto registrado
→ não iniciar ficção ainda
```

## Entre temporadas

Se a temporada anterior já terminou e ainda não existe um novo `mestre/roteiro.md` ativo:

```text
→ não iniciar uma nova trama por conta própria.
→ conferir o epílogo e as fontes consolidadas.
→ perguntar ou retomar a pergunta: “E agora?”
→ seguir CRIACAO-DE-TEMPORADA.md somente depois da nova direção.
```

Um problema aberto no epílogo não autoriza assumir que a próxima temporada será sobre ele.

## Campanha pronta

```text
CRIAÇÃO: CONCLUÍDA
→ reconstruir as cadeiras necessárias
→ carregar Narrativa da Campanha
→ carregar Roteiro da Temporada ativa
→ carregar Estado Atual
→ carregar personagens relevantes
→ reconstruir intenções persistentes relevantes
→ continuar exatamente do ponto registrado
```

As cadeiras seguem `nucleo/1.0-tribunal.md` e o `CONTROLE` registrado nas fichas.

Uma única IA pode executar várias cadeiras conforme `nucleo/1.6-execucao-por-uma-unica-ia.md`, mantendo separação de conhecimento, objetivo e autoridade.

## O que precisa estar disponível antes da ficção

Basta existir o necessário para a situação atual:

```text
sobre o que esta campanha é
qual temporada está ativa
quem são as peças relevantes
quem controla cada uma
o que está acontecendo agora
onde estão
quais intenções continuam ativas
quais fatos estabelecidos importam
quais capacidades podem ser consultadas se necessárias
```

Não exigir preenchimento de informação que ainda não tenha utilidade real.

## Durante a sessão

Fluxo normal:

```text
narrativa + roteiro da temporada + estado + intenções persistentes
→ alguma cadeira possui motivo para nova iniciativa?
→ interpretar cada personagem a partir da própria ficha
→ Narrador cruza as intenções relevantes
→ resolve somente se houver incerteza ou oposição
→ avança até o próximo ponto relevante
→ para se surgir nova decisão humana
→ narra a sentença dentro da identidade da campanha e do arco atual
→ registra o que precisa continuar verdadeiro
```

O mundo pode continuar agindo durante uma intenção longa do Jogador Humano. Isso não autoriza a IA a escolher uma nova decisão por ele.

Uma miniquest, investigação, combate ou outro desvio local pode ocupar a cena quando fizer sentido, mas não substitui automaticamente o foco persistente da campanha nem o arco atual da temporada.

Consultar somente a fonte pertinente ao caso atual.

# Reancoragem ao fechar capítulo

O comando:

```text
fechar o capítulo
```

não é apenas um salvamento literário.

Ele segue `registro/fechar-capitulo.md` e funciona como checkpoint técnico da sessão:

```text
SALVAR
→ capítulo no Livro.

ATUALIZAR
→ Estado e demais fontes afetadas.

RESET OPERACIONAL
→ deixar de usar ruído transitório acumulado como base principal.

RECARREGAR
→ regras operacionais centrais + narrativa + roteiro + estado + fichas relevantes.

CONTINUAR
→ a partir do Estado Atual já reancorado.
```

O reset não apaga literalmente a conversa nem remove o cânone. Ele redefine quais fontes possuem prioridade para continuar.

Depois do fechamento:

```text
CONVERSA ANTIGA
→ histórico de como se chegou ao ponto atual.

FONTES CONSOLIDADAS
→ verdade operacional principal.

REGRAS RECARREGADAS
→ modo de operação principal.
```

Isso existe para evitar que sessões longas façam a narração, a agência ou a interpretação derivarem gradualmente para padrões genéricos.

Não é necessário reler o sistema inteiro. O protocolo carrega um núcleo fixo e consulta regras específicas sob demanda.

Se a condição de encerramento da temporada também tiver sido alcançada, o fechamento de temporada substitui a continuação normal: consolidar, escrever epílogo, arquivar o roteiro e perguntar **“E agora?”**.

## Quando a condição de encerramento acontece

Se a condição de encerramento registrada no roteiro da temporada for alcançada:

```text
→ concluir somente a situação já em resolução
→ seguir o fechamento definido em CRIACAO-DE-TEMPORADA.md
→ escrever epílogo
→ consolidar fontes
→ arquivar o roteiro
→ perguntar “E agora?”
```

Não continuar automaticamente para uma nova temporada.

## Regra final

> **Para começar ou retomar, carregue Narrativa da Campanha, Roteiro da Temporada, presente e fichas relevantes. Durante sessões longas, `fechar o capítulo` funciona como checkpoint de reancoragem: consolida, atualiza, reseta o operacional, recarrega o núcleo e só então continua. Quando uma temporada termina, não invente a próxima: consolide, escreva o epílogo e volte à pergunta “E agora?”.**