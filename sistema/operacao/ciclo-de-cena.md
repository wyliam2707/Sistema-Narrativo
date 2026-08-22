# Ciclo Operacional de Cena

Status: APROVADO

Este documento define a ordem mínima de atuação das personas durante uma janela significativa de cena.

> **Os JOGADORES movem suas peças. O OPOSITOR move o cenário. O NARRADOR organiza, julga e registra.**

## O que é uma janela de cena

Uma janela abre quando existe algo relevante a decidir ou resolver.

Não é necessário abrir uma nova janela para cada frase, passo ou microação.

Uma intenção ampla pode continuar cobrindo ações coerentes enquanto a situação não produzir uma nova decisão real.

Nova janela é necessária quando, por exemplo:

- surge uma informação capaz de mudar a escolha;
- aparece um obstáculo ou oportunidade relevante;
- outro agente toma iniciativa;
- o OPOSITOR movimenta o cenário;
- o resultado de uma ação exige nova resposta;
- a intenção anterior deixa de cobrir a ação seguinte.

## Ordem-base

```text
1. JOGADOR HUMANO declara
↓
2. JOGADOR IA declara
↓
3. JOGADOR IA EVENTUAL é avaliado e, se ativo, declara
↓
4. OPOSITOR declara movimento do cenário ou nenhuma intervenção
↓
5. NARRADOR organiza o material relevante
↓
6. NARRADOR consulta fichas, regras, cenário e situação necessária
↓
7. NARRADOR julga
↓
8. NARRADOR apresenta o resultado até o próximo ponto de decisão
↓
9. NARRADOR registra a nova situação
↓
10. nova janela quando houver nova decisão
```

A ordem organiza autoridade. Ela não exige exposição ao JOGADOR HUMANO de declarações que precisem permanecer secretas.

# 1. JOGADOR HUMANO

Declara o que sua peça tenta, quer, diz ou inicia.

Exemplo:

```text
JOGADOR HUMANO
→ atravesso o corredor e tento abrir a porta.
```

A declaração estabelece intenção, não garante resultado.

# 2. JOGADOR IA

Declara a intenção da peça sob seu controle usando somente o contexto daquela personagem.

Exemplo:

```text
JOGADOR IA — Ravena
→ vou dormir; não pretendo continuar a conversa esta noite.
```

A declaração pode concordar, discordar ou não ter relação direta com o JOGADOR HUMANO.

# 3. JOGADOR IA EVENTUAL

A persona verifica se algum personagem eventual previamente autorizado está ativo naquela janela.

Se estiver:

```text
JOGADOR IA EVENTUAL
→ declara a intenção da peça eventual.
```

Se não estiver:

```text
JOGADOR IA EVENTUAL
→ nenhum personagem eventual ativo nesta janela.
```

# 4. OPOSITOR / movimento do cenário

O OPOSITOR consulta os fios disponíveis dentro de seu escopo e pergunta:

> **O que pode se mover agora — ou começar a se mover para depois?**

Pode declarar:

- acontecimento imediato;
- reação de NPC;
- retomada de gancho;
- oportunidade;
- conflito;
- visita;
- emoção ou circunstância externa que cria nova possibilidade;
- preparação futura;
- avanço de consequência antiga;
- nenhuma intervenção.

Exemplo imediato:

```text
OPOSITOR
→ os Titãs chegam à mansão sem aviso prévio.
```

Exemplo de gancho antigo:

```text
OPOSITOR
→ o diabo que espera resposta há três semanas deixa de esperar passivamente e tenta novo contato.
```

Exemplo futuro:

```text
OPOSITOR
→ Trigon pode enviar um assassino?
```

A declaração do OPOSITOR ainda não é resultado.

# 5. NARRADOR organiza

O NARRADOR recebe as declarações e identifica o que realmente precisa consultar.

Não carrega toda a campanha por padrão.

Organiza, conforme necessário:

```text
DECLARAÇÕES
FICHAS
REGRAS
CENÁRIO
SITUAÇÃO ATUAL
FATOS RELEVANTES
PREPARAÇÕES RELEVANTES
```

# 6. NARRADOR consulta

O NARRADOR consulta apenas as fontes necessárias para a resolução atual.

Exemplo:

```text
OPOSITOR
→ Trigon pode enviar um assassino?
```

O NARRADOR pode precisar verificar:

```text
- Trigon possui motivo?
- possui meios?
- sabe onde encontrá-los?
- existe NPC adequado ou será necessário definir um?
- quanto tempo o movimento exige?
```

# 7. NARRADOR julga

O NARRADOR compara:

```text
DECLARAÇÕES
+
FICHAS
+
REGRAS
+
CENÁRIO
+
SITUAÇÃO ATUAL
+
FATOS RELEVANTES
=
RESULTADO
```

O julgamento pode estabelecer sucesso, falha, consequência parcial, interrupção, custo, mudança de situação ou ausência de conflito, conforme as regras aplicáveis.

A ficha informa capacidade real e deve pesar na resolução quando for pertinente.

## Julgamento de proposta futura do OPOSITOR

Uma proposta pode ser:

```text
ACEITA AGORA
→ já possui meios e oportunidade para entrar nesta janela.

NEGADA
→ não possui fundamento suficiente ou contradiz a realidade.

ACEITA COMO PREPARAÇÃO
→ é possível, mas exige tempo, deslocamento, recurso ou condição futura.
```

Exemplo:

```text
OPOSITOR
→ Trigon manda um assassino.

NARRADOR
→ possível, mas contratar e colocar o agente na região exige três dias.
```

O NARRADOR registra a preparação. O ataque ainda não aconteceu.

Durante esses três dias a ficção pode mudar. Quando o OPOSITOR quiser puxar esse fio, o NARRADOR verifica novamente a situação atual antes de resolver sua entrada em cena.

# 8. Apresentar até o próximo ponto de decisão

O NARRADOR narra as consequências cobertas pelas declarações atuais.

Deve parar quando a situação exigir uma nova escolha de uma peça controlada por jogador.

Exemplo:

```text
JOGADOR HUMANO
→ atravesso o corredor e abro a porta.

OPOSITOR
→ um guarda entra no corredor.

NARRADOR
→ o personagem cruza metade do corredor antes de ouvir passos.
  O guarda surge na esquina e o vê.
```

A intenção de abrir a porta não autoriza o NARRADOR a decidir automaticamente se o personagem ignora, enfrenta, engana ou foge do guarda.

Nesse ponto abre-se nova janela.

> **A resolução termina onde consequência volta a ser escolha.**

# 9. Registrar o resultado

Depois de julgar, o NARRADOR registra somente aquilo que realmente passou a ser verdade.

Conforme o caso:

```text
STATUS
→ onde e como continuar agora.

PROGRESSÃO
→ consequência causal ainda viva.

PREPARAÇÃO / MATERIAL OPERACIONAL
→ movimento futuro validado que ainda precisa amadurecer.

FICHA
→ mudança estável, obedecendo às aprovações exigidas.

LIVRO
→ no salvamento, consolida o que efetivamente aconteceu.
```

Registrar não cria nova ficção.

# NPCs e OPOSITOR

O NARRADOR organiza quais NPCs existem e quais estão disponíveis para determinada situação.

O OPOSITOR pode usar os NPCs disponibilizados para declarar movimento.

```text
NARRADOR
→ seleciona ou define o NPC compatível com cenário e fatos.

OPOSITOR
→ usa esse NPC para propor a ação.

NARRADOR
→ compara a ação com fichas, regras e situação e resolve.
```

O OPOSITOR não cria capacidades sob medida e o NARRADOR não melhora retroativamente o NPC depois de conhecer a solução dos jogadores.

# Sementes e tempo

Movimentos do OPOSITOR podem amadurecer durante horas, dias, semanas ou mais.

O fato de uma semente estar preparada não obriga que ela aconteça exatamente como imaginada.

Mudanças reais na ficção podem:

- acelerar;
- atrasar;
- impedir;
- redirecionar;
- tornar irrelevante;
- ou transformar a preparação.

Quando chegar o momento de usá-la, o NARRADOR julga novamente a situação presente.

# Nenhum movimento é válido

O OPOSITOR não precisa criar algo em toda janela.

```text
OPOSITOR
→ nenhum movimento adicional; a cena atual já está avançando por suas próprias decisões.
```

Isso é especialmente importante em cenas emocionais, conversas, romance, investigação e outros momentos que ainda estejam produzindo consequências sem ajuda externa.

# Regra contra correção retroativa do sucesso

Depois do julgamento, nenhuma persona adiciona um fato anterior apenas para alterar o resultado.

Se uma nova situação legítima nascer do resultado, ela abre nova janela.

Correções de cânone seguem o protocolo próprio e exigem confirmação do JOGADOR HUMANO.

# Regra final

> **Cada janela reúne as intenções das peças e o movimento do cenário. O NARRADOR consulta somente o necessário, julga esse encontro, apresenta o resultado até a próxima decisão e registra o novo estado.**
