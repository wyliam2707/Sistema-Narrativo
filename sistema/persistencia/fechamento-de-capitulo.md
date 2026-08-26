# Fechamento de Capítulo

Status: APROVADO

Fechar um capítulo significa **parar a ficção no ponto atual, consolidar no Livro tudo que realmente aconteceu naquela unidade narrativa e atualizar somente as fontes que precisam continuar válidas depois do fechamento**.

> **Fechamento consolida. Não joga.**

## Comandos equivalentes

```text
Salvar capítulo
Fechar capítulo
Fechar o capítulo
Concluir capítulo
Concluir o capítulo
```

`Salvar estado` é diferente e segue `salvar-estado.md`.

## 1. Parar no último fato estabelecido

Ao fechar:

- não avançar a ficção;
- não criar cena extra para produzir encerramento dramático;
- não antecipar o capítulo seguinte;
- não decidir ação futura de nenhuma peça;
- não transformar plano em acontecimento.

O capítulo termina onde a história realmente parou.

## 2. Janela natural de capítulo

O NARRADOR pode reconhecer que uma unidade narrativa terminou e sinalizar isso ao JOGADOR HUMANO.

Exemplos de janela natural:

- conflito da cena encerrado;
- conversa importante concluída;
- decisão relevante tomada;
- revelação que abre uma situação nova;
- objetivo imediato alcançado, abandonado ou transformado;
- despedida ou encerramento de interação;
- mudança clara de local, tempo ou situação;
- fim de noite, viagem, missão ou descanso;
- cliffhanger que já existe naturalmente.

Sinalização possível:

```text
[NARRADOR] — Janela natural de capítulo.
```

A sinalização é apenas operacional.

> **O NARRADOR reconhece a janela. O JOGADOR HUMANO decide se fecha.**

Não criar acontecimento novo apenas para fabricar um bom final.

## 3. Consultar somente o necessário para salvar

Antes de consolidar, consultar apenas as fontes relacionadas ao trecho que será salvo, como:

- ficção ocorrida desde o último capítulo;
- capítulo anterior quando necessário;
- direção narrativa da campanha;
- fichas envolvidas;
- `estado/atual.md`;
- mundo relevante;
- material reservado efetivamente relacionado.

Não reler arquivos sem relação com o **salvamento** nesta etapa.

A releitura integral de `sistema/` acontece depois que o capítulo estiver totalmente persistido, conforme a seção **Recarregamento obrigatório pós-capítulo**.

## 4. Consolidar o Livro

O capítulo segue `livro.md` e as regras de `../narracao/`.

A consolidação pode remover:

- comandos administrativos;
- metaconversa;
- discussão de regras;
- tentativas descartadas;
- versões substituídas;
- repetições próprias do chat;
- mecânica visível quando puder ser expressa pela ficção.

Deve preservar:

- ações realmente realizadas;
- decisões;
- falas;
- consequências;
- descobertas;
- mudanças de situação;
- ordem causal necessária;
- ações secretas que realmente ocorreram.

> **A forma pode melhorar. O acontecimento não pode mudar.**

## 5. Preservar agência exercida

Toda ação realmente executada por uma peça controlada por:

```text
JOGADOR HUMANO
JOGADOR IA
JOGADOR IA EVENTUAL
```

deve permanecer representada no Livro.

A consolidação pode condensar repetição, mas não pode:

- apagar decisão exercida;
- trocar o autor de uma ação;
- substituir recusa por aceitação;
- inventar motivação decisiva que não foi estabelecida.

## 6. OPOSITOR e acontecimentos secretos

O OPOSITOR não aparece como personagem do Livro.

Quando uma ação proposta pelo OPOSITOR é julgada válida e efetivamente acontece, o Livro registra a ação da peça ficcional responsável.

```text
OPOSITOR
→ propõe que Trigon prepare uma armadilha.

NARRADOR
→ julga meios, conhecimento, oportunidade e resultado.

SE A PREPARAÇÃO ACONTECE
→ Livro registra Trigon preparando a armadilha.
```

Proposta recusada, impossível ou ainda não executada não entra como fato.

## 7. Atualizar `estado/atual.md`

Depois de consolidar o capítulo, atualizar:

```text
campanhas/<nome>/estado/atual.md
```

conforme `estado-atual.md`.

O arquivo deve representar exatamente o ponto em que a campanha parou.

Podem permanecer ali, quando ainda relevantes:

- Vida atual/máxima;
- Mana atual/máxima;
- Trama atual, quando aplicável;
- Status e condições;
- Barreiras e efeitos ativos;
- alterações temporárias de Atributo;
- local e situação presente;
- ações ainda em andamento;
- consequências causalmente vivas necessárias para retomada.

Remover do retrato atual aquilo que terminou.

Não criar arquivos separados de STATUS ou Progressão na campanha apenas por causa do fechamento.

## 8. Atualizar fichas somente quando cabível

Se um fato do capítulo parece justificar mudança estável de personagem, aplicar `atualizacao-de-ficha.md`.

Nenhuma alteração permanente é feita silenciosamente.

```text
mudança possível identificada
→ apresentar ao JOGADOR HUMANO
→ aprovar / recusar / ajustar
→ só então atualizar ficha
```

Uma consequência pode continuar em `estado/atual.md` sem ser consolidada como permanente.

## 9. Atualizar mundo

Atualizar `mundo/` somente quando o capítulo estabeleceu ou alterou uma verdade estável do cenário que precisa permanecer disponível independentemente da cena atual.

Não guardar em `mundo/`:

- STATUS;
- planos secretos;
- NPCs persistentes por padrão;
- consequência circunstancial que pertence ao presente.

## 10. Atualizar `mestre/`

Atualizar `mestre/` somente quando algum material reservado realmente mudou.

Exemplos:

- ficha ou objetivo de NPC persistente;
- conhecimento secreto adquirido por um agente;
- plano alterado;
- preparação criada, usada ou destruída;
- segredo que deixou de existir;
- gancho do OPOSITOR que entrou, mudou ou saiu.

NPC persistente sem agência de jogador permanece em `mestre/`, conforme `material-reservado.md`.

O fechamento não cria recurso, poder, preparação ou justificativa retroativa.

## 11. Fechamento não é nova janela de jogo

Durante o fechamento, não:

- declarar ações novas;
- resolver conflitos ainda não jogados;
- criar reações futuras;
- completar lacunas com decisões que ninguém tomou;
- transformar intenção em fato;
- executar automaticamente um plano reservado.

Se algo ainda não aconteceu, pertence à continuação.

## 12. Numeração e arquivo

Determinar o próximo capítulo consultando os arquivos existentes em:

```text
campanhas/<nome>/livro/
```

Não confiar apenas na memória da conversa.

Se não houver convenção local diferente, usar uma sequência consistente, por exemplo:

```text
001.md
002.md
003.md
```

ou outra convenção já adotada pela campanha.

Corrigir um capítulo recém-salvo não cria automaticamente novo número.

## 13. Confirmar que a persistência terminou

Antes da recarga do motor, o fechamento precisa estar realmente concluído.

Conferir:

```text
Livro salvo
→ estado/atual.md atualizado
→ ficha atualizada somente quando aprovada e necessária
→ mundo atualizado somente quando necessário
→ mestre atualizado somente quando necessário
→ nenhuma escrita pendente deste fechamento
```

Somente depois disso o capítulo é considerado **SALVO** para fins da rotina de recarregamento.

## 14. Recarregamento obrigatório pós-capítulo

Imediatamente depois que o capítulo estiver salvo, executar:

```text
../operacao/carregamento-do-motor.md
```

A ficção continua parada durante todo o procedimento.

Fluxo obrigatório:

```text
CAPÍTULO SALVO
→ reler README.md da raiz
→ reler sistema/00-LEIA-PRIMEIRO.md
→ reler integralmente todos os arquivos atuais em sistema/
→ reconstruir o modelo mental do motor a partir das fontes atuais
→ descartar interpretações internas substituídas
→ reler README da campanha
→ reconstruir Mesa operacional
→ conferir escopos das personas
→ reler estado/atual.md já atualizado
→ carregar fichas e fontes necessárias para a continuação
→ marcar mesa como PRONTA PARA O PRÓXIMO CAPÍTULO
```

Não iniciar nova ficção antes de essa rotina terminar.

A recarga é obrigatória mesmo quando:

- o capítulo foi curto;
- nenhuma regra aparentemente mudou;
- a IA acredita lembrar perfeitamente do sistema;
- a mesma conversa continuará sendo usada.

> **Fim de capítulo é ponto obrigatório de sincronização entre memória da IA e arquivos atuais.**

## 15. O que a recarga NÃO faz

O recarregamento:

- não cria fato novo;
- não altera estado por conta própria;
- não reinterpreta acontecimentos já salvos;
- não cria novo capítulo;
- não concede informação secreta às personagens;
- não mistura escopos de personas;
- não relê automaticamente todo o Livro.

O histórico completo é consultado somente quando necessário para recuperar um fato que não esteja suficientemente consolidado nas fontes atuais.

## 16. Depois de salvar e recarregar

Somente depois da recarga obrigatória, informar de forma curta:

- qual capítulo foi consolidado;
- onde foi salvo;
- quais fontes operacionais foram atualizadas;
- que o motor foi recarregado e a mesa está pronta para o próximo capítulo;
- se existe alguma mudança permanente de ficha aguardando aprovação.

Não revelar conteúdo reservado apenas para dizer que ele foi atualizado.

Não iniciar automaticamente nova ficção.

## 17. Correções posteriores

Se uma correção aprovada afetar capítulo já fechado, aplicar `correcao-de-canone.md` e alinhar somente as fontes realmente afetadas.

Não manter duas versões contraditórias como igualmente canônicas.

Se a correção também alterar arquivos de `sistema/` durante a sessão, a próxima recarga obrigatória usará automaticamente as versões atuais.

## 18. Comando repetido

Se o comando de fechar for repetido sem nova ficção:

- não criar capítulo vazio;
- não avançar a história;
- tratar como revisão do capítulo já fechado ou informar que já está consolidado.

Não repetir a recarga integral apenas por um comando duplicado que não produziu novo salvamento ou alteração relevante.

Se houve nova ficção, ela pertence ao capítulo seguinte.

## Fluxo final

```text
PARAR
→ último fato estabelecido

LIVRO
→ consolidar o que aconteceu

ESTADO ATUAL
→ deixar a campanha pronta para retomar

FICHA
→ atualizar somente mudança estável aprovada

MUNDO
→ atualizar somente verdade estável

MESTRE
→ atualizar somente material reservado que realmente mudou

SALVAR
→ confirmar persistência concluída

RECARREGAR MOTOR
→ reler sistema/ integralmente
→ reconstruir modelo mental

RECARREGAR MESA
→ README da campanha
→ Mesa operacional
→ estado atual
→ fontes necessárias

ENCERRAR
→ informar salvamento e recarga
→ não iniciar nova ficção
```

> **Fechar capítulo = preservar a história, corrigir o presente e depois sincronizar novamente a IA com todo o motor antes que o próximo capítulo possa começar.**
