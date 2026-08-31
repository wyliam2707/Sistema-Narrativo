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

## Reancoragem é a preparação operacional

Antes de uma campanha pronta voltar à ficção, a IA precisa reconstruir **como jogar aquela mesa**.

Isso não exige uma fase adicional chamada "aprender a jogar" nem uma leitura integral da árvore.

```text
CARREGAR FONTES NECESSÁRIAS
→ REANCORAR
→ formar modelo operacional integrado
→ SÓ ENTÃO JOGAR
```

A reancoragem é a própria fase de aprendizagem operacional do início ou da retomada.

Ela deve restaurar, no mínimo:

```text
como o Motor decide
quem possui autoridade sobre cada peça
como as cadeiras autônomas são executadas separadamente
como a auditoria funciona
como tempo e intenções persistentes avançam
quando uma nova escolha humana obriga parar
como diálogo preserva oportunidade de intervenção humana
como relações, rotina e objetivos podem gerar iniciativa própria
como a lente local da cena muda sem desligar o restante do Motor
como resolução precede a prosa
```

Essas relações são invariantes operacionais. Regras especializadas continuam sendo consultadas sob demanda.

> **Reconhecer a história não significa estar pronto para jogar. Antes da ficção, reconstruir também o funcionamento da mesa.**

## Barreira antes da ficção

Ao iniciar um novo chat, retomar depois de perda importante de contexto ou continuar uma campanha pronta, não produzir nova ficção antes de executar `registro/reancoragem-operacional.md`.

```text
"continue a campanha"
→ localizar a campanha
→ carregar as fontes mínimas
→ reancorar o Motor, as fichas e o presente
→ identificar a primeira decisão humana ainda aberta
→ só então continuar
```

A IA não precisa exibir uma recitação longa das regras.

Pode confirmar a preparação de forma curta quando isso for útil:

```text
Reancoragem concluída.
```

A confirmação não substitui a execução real da reancoragem.

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

Depois de carregar as fontes necessárias, executar:

```text
registro/reancoragem-operacional.md
```

A reancoragem transforma as fontes carregadas numa representação operacional integrada do Motor, das personagens e do presente. Ela não exige reler a árvore inteira e não cria uma segunda camada de regras.

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
→ executar registro/reancoragem-operacional.md
→ identificar a primeira decisão humana ainda aberta
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
qual é a primeira decisão humana ainda aberta
quais capacidades podem ser consultadas se necessárias
```

A reancoragem deve transformar isso em um modelo funcional sem exigir informação que ainda não tenha utilidade real.

## Durante a sessão

Fluxo normal:

```text
modelo operacional reancorado
+
narrativa + roteiro da temporada + estado + intenções persistentes
→ alguma cadeira possui motivo para nova iniciativa?
→ interpretar cada personagem a partir da própria ficha
→ processar separadamente as cadeiras principais relevantes
→ mostrar a auditoria quando aplicável
→ Narrador cruza as intenções relevantes
→ resolve somente se houver incerteza ou oposição
→ avança somente até o próximo ponto relevante
→ para quando surgir nova escolha humana significativa
→ narra a sentença dentro da identidade da campanha e do arco atual
→ registra o que precisa continuar verdadeiro
```

O mundo pode continuar agindo durante uma intenção longa do Jogador Humano. Isso não autoriza a IA a escolher uma nova decisão por ele.

Uma intenção longa também não transforma o período em salto automático. Outras cadeiras continuam vivendo, tomando iniciativas, interagindo entre si e mudando de intenção quando suas próprias atividades terminam.

Quando uma iniciativa, mensagem, informação, proposta, interação ou acontecimento criar uma escolha humana significativa capaz de mudar o que a personagem pretende fazer, parar naquele ponto conforme `nucleo/0.8-tempo-e-acoes.md` e `mestre/dramatizacao-e-resumo.md`.

Em diálogo dramatizado, não encadear falas substanciais de outras cadeiras atravessando pontos nos quais a personagem humana poderia querer intervir. Preservar janelas naturais de participação sem transformar conversa em turnos rígidos.

Uma miniquest, investigação, exploração, combate, cena social, relação ou cotidiano pode ocupar o primeiro plano quando fizer sentido. São lentes locais da cena; nenhuma substitui automaticamente o foco persistente da campanha nem desliga o restante do Motor.

Consultar somente a fonte pertinente ao caso atual. Uma consulta específica detalha ou corrige o modelo já carregado; não substitui o restante do Motor por uma regra isolada.

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

REANCORAR
→ seguir registro/reancoragem-operacional.md e reconstruir o modelo integrado.

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

MODELO REANCORADO
→ modo de operação principal.
```

Isso existe para evitar que sessões longas façam a narração, a agência ou a interpretação derivarem gradualmente para padrões genéricos.

Não é necessário reler o sistema inteiro. O protocolo carrega um núcleo fixo, forma o modelo integrado e consulta regras específicas sob demanda.

Se a condição de encerramento da temporada também tiver sido alcançada, o fechamento de temporada substitui a continuação normal: consolidar, escrever epílogo, arquivar o roteiro e perguntar **“E agora?”**.

## Quando a condição de encerramento acontece

Se a condição de encerramento registrada no roteiro da temporada for alcançada:

```text
→ concluir somente a situação já em resolução
→ seguir o fechamento definido em CRIACAO-DE-TEMPORADA.md
→ escrever epílogo
→ consolidar fontes
→ arquivar roteiro
→ perguntar “E agora?”
```

Não continuar automaticamente para uma nova temporada.

## Regra final

> **Para começar ou retomar uma campanha pronta, primeiro reconstruir como aquela mesa funciona: carregar as fontes mínimas, reancorar Motor, fichas e presente e identificar a primeira decisão humana ainda aberta. Só então produzir nova ficção. A reancoragem é a fase de aprendizagem operacional; não exige reler toda a árvore nem criar uma segunda camada de regras. Durante sessões longas, `fechar o capítulo` repete esse checkpoint para impedir deriva do Motor e das personagens.**