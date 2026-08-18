# Protocolo de Fechamento e Salvamento de Capítulo

Este documento define **o que acontece quando o jogador decide encerrar e salvar um capítulo jogado**.

Ele transforma o material da sessão em registro literário canônico e atualiza a continuidade da aventura sem depender da memória da conversa.

> **Jogar produz acontecimentos. Salvar capítulo consolida o que realmente aconteceu.**

---

## 1. Comandos equivalentes

Os comandos abaixo são aliases e executam o mesmo protocolo:

- `Salvar capítulo`
- `Fechar capítulo`
- `Fechar o capítulo`
- `Concluir capítulo`
- `Concluir o capítulo`

Variações claras de maiúsculas, acentos ou artigo podem ser entendidas normalmente.

Quando qualquer um desses comandos for usado, **não avançar a história para um capítulo novo antes de concluir o salvamento do capítulo atual**.

`Salvar estado` continua sendo um comando diferente: ele atualiza apenas o savegame operacional e não exige transformar a sessão em capítulo literário.

---

## 2. Parar exatamente onde a história está

Ao receber o comando:

1. interromper qualquer avanço narrativo novo;
2. considerar como limite do capítulo o último acontecimento ficcional já resolvido;
3. não criar uma cena extra apenas para produzir um encerramento dramático;
4. não decidir pelo personagem do jogador algo que ele ainda não decidiu.

O capítulo pode terminar em silêncio, conversa, deslocamento, combate, descoberta, descanso ou qualquer outro ponto em que o jogador tenha escolhido encerrá-lo.

> **O comando fecha o capítulo onde ele está; não força a história até um final conveniente.**

---

## 3. Consultar as fontes antes de consolidar

Antes de escrever o capítulo, consultar o que for necessário para evitar contradições.

Normalmente isso inclui:

- material jogado desde o último capítulo fechado;
- último capítulo canônico, quando necessário;
- `README.md` da aventura;
- diretrizes narrativas específicas;
- fichas dos personagens envolvidos;
- material reservado em `mestre/`, **somente quando for relevante para os acontecimentos consolidados**;
- mundo e regras específicas relevantes;
- relacionamentos relevantes;
- `progressao/`;
- `cronologia/`;
- `estado/atual.md`.

Não é necessário reler arquivos sem relação com o capítulo apenas por formalidade.

Ao consultar `mestre/`, separar o que o narrador sabe daquilo que os personagens realmente descobriram. Informação oculta não entra no capítulo apenas porque existe na ficha reservada.

Quando existir conflito, seguir a hierarquia de cânone da aventura e a correção explícita mais recente do jogador.

---

## 4. Consolidar somente o cânone válido

O material jogado é matéria-prima. O capítulo salvo deve conter **somente a versão válida dos acontecimentos**.

Remover da versão literária:

- comandos de sistema;
- mensagens ao narrador;
- discussão de regras;
- correções fora da ficção;
- tentativas descartadas;
- versões substituídas de uma mesma ação;
- repetições produzidas pela dinâmica do RPG;
- STATUS e mecânica visível, salvo quando sua consequência existir naturalmente na narrativa;
- informação reservada do narrador que nenhum personagem tenha descoberto ou que não pertença legitimamente ao ponto de vista literário adotado.

Preservar:

- decisões efetivamente tomadas;
- falas válidas;
- ações e reações que realmente ocorreram;
- consequências;
- informações descobertas;
- conhecimento e desconhecimento plausível de cada personagem;
- mudanças reais de relação;
- ferimentos, perdas, ganhos e alterações do mundo;
- ordem causal dos acontecimentos.

> **Correção fora da história altera o cânone; não vira cena dentro do livro.**

---

## 5. Reconstruir como capítulo literário

O capítulo não deve parecer uma transcrição de chat.

Reconstruir os acontecimentos usando:

1. as diretrizes específicas da aventura, se existirem;
2. `sistema/narracao-e-escrita-padrao.md` para tudo que a aventura não substituir;
3. o estilo e formato dos capítulos canônicos anteriores, quando houver.

É permitido:

- melhorar transições;
- condensar ações repetitivas;
- transformar descrição mecânica em prosa natural;
- organizar diálogos para leitura;
- resumir passagem de tempo sem importância dramática;
- dramatizar acontecimentos cuja fala, reação ou subtexto realmente importam.

Não é permitido:

- inventar acontecimentos para preencher lacunas;
- alterar a decisão do jogador;
- criar pensamentos decisivos não estabelecidos para o personagem do jogador;
- mudar resultado mecânico ou causal já resolvido;
- antecipar acontecimentos do capítulo seguinte;
- introduzir retroativamente poderes, relações ou regras para tornar a cena mais elegante.

> **A consolidação melhora a forma, não reescreve os fatos.**

---

## 6. Número e arquivo do capítulo

Determinar o próximo capítulo consultando `livro/`, nunca apenas pela memória da conversa.

Se a aventura possuir convenção própria de nomes, segui-la.

Caso contrário, usar um formato consistente, por exemplo:

```text
livro/capitulo-01.md
livro/capitulo-02.md
livro/capitulo-03.md
```

O formato literário padrão recomendado é:

```text
# CAPÍTULO N
## TÍTULO

[texto do capítulo]
```

Não criar um novo número se o jogador estiver apenas corrigindo um capítulo que acabou de ser salvo.

---

## 7. Atualizações obrigatórias de continuidade

Salvar o capítulo não termina apenas em `livro/`.

Depois de consolidá-lo, verificar e atualizar o que realmente mudou.

### `cronologia/`
Registrar fatos importantes e mudanças de conhecimento necessárias para consulta rápida.

### `progressao/`
Registrar somente consequências que continuam com potencial causal futuro.

Não transformar qualquer acontecimento do capítulo em Progressão.

### `personagens/`
Alterar ficha somente se a própria ficção mudou de forma estável o personagem.

Não conceder XP, aumento automático ou recompensa mecânica por ter concluído o capítulo.

### `mestre/`
Atualizar somente quando acontecimentos reais alterarem informação que o narrador precisa acompanhar em segredo.

Exemplos:
- um antagonista reservado foi ferido de forma duradoura;
- perdeu ou ganhou um recurso de forma estabelecida na ficção;
- mudou de objetivo por causa de um acontecimento real;
- uma capacidade antes oculta foi revelada e precisa ter seu estado de conhecimento atualizado.

Não adicionar retroativamente nova capacidade ou proteção apenas porque o protagonista encontrou uma solução eficaz.

### `relacionamento/`
Atualizar quando um vínculo recorrente e complexo realmente mudou de forma relevante.

Relações circunstanciais com futuro possível podem ficar em `progressao/` em vez de poluir a ficha.

### `estado/atual.md`
Sobrescrever com o ponto exato em que o capítulo terminou:

- Vida;
- Energia;
- Condições;
- efeitos ativos;
- localização;
- situação imediata;
- decisões ou riscos ainda em andamento.

Remover do STATUS aquilo que já terminou.

Se alguma informação operacional precisa permanecer oculta do jogador, não a exponha apenas para completar `estado/atual.md`; mantenha-a na área reservada adequada.

> **Livro guarda o que aconteceu. Cronologia facilita consulta. Progressão guarda o que ainda pode voltar. Estado atual guarda exatamente onde continuar. Material do mestre preserva o que precisa continuar verdadeiro sem ser revelado antes da hora.**

---

## 8. Revisão depois do salvamento

Após salvar, informar de forma curta:

- qual capítulo foi consolidado;
- onde foi salvo;
- quais arquivos de continuidade foram atualizados;
- se existe algum ponto que precise de revisão do jogador.

Ao informar os arquivos atualizados, não revelar conteúdo reservado do narrador. Se `mestre/` tiver sido atualizado, basta registrar que a continuidade reservada foi mantida quando isso puder ser dito sem entregar segredo.

O jogador pode então corrigir o capítulo.

Se houver correção:

1. alterar o mesmo capítulo;
2. atualizar também cronologia, Progressão, ficha, relacionamento, material reservado ou estado quando a correção afetar esses arquivos;
3. não manter simultaneamente duas versões contraditórias como canônicas.

Não iniciar automaticamente um novo capítulo na mesma resposta do comando de salvamento. O jogador continua quando desejar.

---

## 9. Comando repetido

Se `Salvar capítulo` for usado novamente sem que tenha ocorrido nova ficção desde o último fechamento:

- não criar outro capítulo vazio;
- verificar se o jogador pretende revisar o capítulo já salvo;
- se não houver correção, apenas informar que o capítulo atual já está fechado.

Se houve nova ficção depois do fechamento anterior, ela pertence ao capítulo seguinte.

---

## 10. Quando a aventura não usa capítulos

Se a aventura declarar explicitamente que não usa capítulos literários, não impor esse formato.

Nesse caso, interpretar o comando como pedido para executar o **método equivalente de consolidação definido pela própria aventura**, mantendo as mesmas regras de cânone e continuidade.

---

## 11. Regra final

> **Salvar capítulo = parar a ficção, consultar as fontes, consolidar somente o que realmente aconteceu, escrever na forma literária correta, atualizar continuidade e deixar um ponto exato para retomar.**

> **`Salvar capítulo`, `Fechar capítulo` e `Concluir capítulo` significam a mesma coisa.**
