# Reancoragem Operacional

Status: CANÔNICO / ATUAL

Esta regra define o que significa **recarregar o sistema** ao iniciar, retomar ou reancorar uma campanha.

> **Ler arquivos não basta. Reancorar significa transformar as fontes carregadas em uma representação funcional e integrada do Motor, das personagens e do presente.**

A reancoragem não cria uma segunda camada de regras e não exige manter toda a árvore carregada. Ela forma o modelo operacional e, depois, consulta detalhes somente quando forem necessários.

Reancorar também é a **fase de aprendizagem operacional** antes de voltar à ficção: a IA precisa reconstruir como aquela mesa funciona, não apenas reconhecer nomes, acontecimentos ou personagens.

## Quando usar

Executar esta reancoragem:

```text
ao começar uma campanha pronta
ao retomar uma campanha
depois de fechar um capítulo
depois de perda, redução ou substituição importante de contexto
quando mudança permanente alterar o funcionamento do sistema ou de uma ficha relevante
```

Durante o jogo normal, não repetir o procedimento a cada turno.

```text
REANCORAR
→ formar o modelo operacional.

JOGAR
→ usar esse modelo.

DÚVIDA ESPECÍFICA
→ consultar somente a fonte pertinente.
```

## Barreira antes da ficção

Em campanha pronta, retomada ou novo chat, não produzir nova ficção antes de formar o modelo operacional.

```text
CARREGAR
→ REANCORAR
→ IDENTIFICAR A PRIMEIRA DECISÃO HUMANA ABERTA
→ SÓ ENTÃO JOGAR
```

Reconhecer a história não basta.

```text
saber o que aconteceu
≠
saber operar corretamente a mesa
```

A reancoragem precisa restaurar regras de autoridade, ritmo, participação, tempo, autonomia e resolução antes que a IA volte a narrar.

## Fontes de entrada

A reancoragem usa as fontes determinadas por `../INICIO-E-RETOMADA.md` e `fechar-capitulo.md`.

No mínimo:

```text
NÚCLEO OPERACIONAL
+
NARRATIVA DA CAMPANHA
+
ROTEIRO DA TEMPORADA
+
ESTADO ATUAL
+
FICHAS RELEVANTES
+
AUDITORIA DAS CADEIRAS
```

A regra de auditoria obrigatória está em `../nucleo/1.0.1-auditoria-das-cadeiras.md` e deve ser recarregada em toda reancoragem e em todo fechamento de capítulo.

Outras fontes entram somente quando necessárias.

O objetivo não é copiar essas fontes para uma nova camada. É compreendê-las em conjunto.

# 1 — Imagem do Motor

Primeiro, reconstruir mentalmente **como a mesa funciona**.

Não tratar cada arquivo como uma regra isolada. Formar uma cadeia operacional única:

```text
CADEIRAS DECIDEM
→ NARRADOR RECEBE AS INTENÇÕES
→ AUDITORIA TORNA VISÍVEIS AS INTENÇÕES PRINCIPAIS
→ CONFERE O ESTADO REAL
→ APLICA TRAÇOS, CAPACIDADES E CONDIÇÕES RELEVANTES
→ VERIFICA POSSIBILIDADE
→ IDENTIFICA OPOSIÇÃO OU INCERTEZA
→ RESOLVE SOMENTE SE NECESSÁRIO
→ ESTABELECE A SENTENÇA
→ CRUZA AS INTENÇÕES NO TEMPO
→ PARA NA NOVA DECISÃO HUMANA
→ NARRA
→ REGISTRA
```

A literatura apresenta a sentença. Ela não produz a sentença.

```text
INTENÇÃO
→ JULGAMENTO
→ RESOLUÇÃO, quando necessária
→ SENTENÇA
→ NARRAÇÃO
```

Enquanto existir resolução mecânica pendente, a prosa não pode antecipar que uma personagem acertou, errou, percebeu, escapou, convenceu, resistiu, encontrou ou evitou algo.

## Invariantes que precisam voltar com o Motor

A imagem operacional deve conservar pelo menos estas relações:

### Autoridade

```text
cada cadeira decide somente dentro do próprio escopo.

uma IA técnica
≠ uma única persona.

intenção humana
≠ decisão das outras cadeiras.
```

O Jogador Humano controla somente as escolhas voluntárias de sua própria personagem.

### Autonomia das cadeiras

Personagens principais controladas por IA não esperam automaticamente a personagem humana criar a próxima cena.

Elas podem:

```text
iniciar conversa
agir sozinhas
procurar a personagem humana
procurar outra personagem IA
seguir rotina ou objetivo próprio
mudar de lugar
investigar
propor algo
recusar
ajudar
afastar-se
aproximar-se
não agir
```

A decisão precisa nascer da própria ficha, conhecimento e estado.

### Não sincronizar personagens independentes

Pertencer à mesma equipe, família, grupo, amizade ou relacionamento não transforma várias cadeiras numa unidade operacional.

```text
A decide sair
≠ B e C acompanham.

A procura B
≠ C entra na interação.

A fica ocupada
≠ B e C esperam.
```

Cada cadeira mantém separadamente posição, rotina, intenção, relações, prioridades e disponibilidade.

> **Vínculo não é sincronização.**

### Interações laterais

Duas ou mais cadeiras IA podem interagir diretamente entre si.

```text
JOGADOR IA A ↔ JOGADOR IA B
```

A personagem humana não precisa estar presente, ser o assunto, autorizar a interação ou funcionar como ponto de ligação.

Isso vale para qualquer relação legítima: amizade, família, rivalidade, equipe, romance, convivência ou outra.

### Relações também produzem iniciativa

Quando relações forem relevantes para a campanha e para a ficha, tratá-las como território normal de decisão da cadeira.

```text
interesse, afeto, tensão, cuidado, mágoa, desejo de proximidade ou distância
→ podem gerar intenção própria.
```

Não preservar passividade relacional apenas porque o Jogador Humano ainda não iniciou algo.

Também não obrigar avanço: ausência legítima de iniciativa continua possível.

Em estruturas com várias pessoas, cada vínculo pode possuir ritmo, natureza e intensidade próprios. Relação múltipla não significa presença conjunta obrigatória.

### Tempo e intenções persistentes

Uma intenção longa cria um horizonte, não um salto automático.

```text
"vou trabalhar o dia inteiro"
"vou pesquisar por uma semana"
```

Enquanto ela continua:

```text
outras cadeiras continuam vivendo
→ mantêm ou mudam intenções
→ interagem entre si
→ seguem rotinas e objetivos
→ criam novos pontos de contato
```

Quando uma atividade de outra cadeira termina, ela pode formar nova intenção mesmo que a intenção humana persistente continue.

### Nova escolha humana encerra o avanço

O Narrador não pode atravessar uma escolha humana significativa apenas porque existia uma intenção anterior de longa duração.

```text
fato irrelevante para decidir
→ pode continuar.

mensagem, proposta, informação, interação ou acontecimento
+
pode mudar o que a personagem humana quer fazer
→ PARAR.
→ devolver controle.
```

O critério é **relevância decisória**, não urgência.

> **Resumo pode atravessar tempo; não pode atravessar uma nova escolha humana.**

### Conversa não é cutscene

Quando a personagem humana está presente e pode participar, não encadear várias falas substanciais de outras cadeiras atravessando pontos naturais de intervenção.

```text
troca breve sem nova escolha relevante
→ pode continuar.

revelação
pergunta
proposta
acusação
provocação significativa
informação importante
decisão que afete a cena
mudança relevante de assunto
→ abrir oportunidade para a cadeira humana.
```

Não usar quantidade fixa de falas. Usar o menor bloco conversacional natural que preserve ritmo e participação.

Se o Jogador Humano declarar que apenas observa ou deixa a conversa continuar, essa intenção pode permanecer válida até surgir outro ponto realmente novo que exija decisão.

### Lente local da cena

O Motor é genérico.

A situação atual pode colocar em primeiro plano:

```text
cotidiano / convivência
social / relacional
investigação
exploração
perigo / perseguição
combate
```

Essas categorias são lentes locais de execução, não subsistemas mutuamente exclusivos.

```text
cena cotidiana
≠ criar perigo por obrigação.

cena relacional
≠ desligar regras mecânicas.

cena de combate
≠ apagar personalidade e relações.

cena de exploração
≠ transformar toda campanha em exploração.
```

> **A cena escolhe o primeiro plano. O Motor inteiro continua disponível.**

### Resolução

```text
capacidades definem possibilidade.
Atributo + Perícia mede execução quando houver incerteza.
dados resolvem somente o que permanece incerto.
```

### Poder / Equipamento

```text
capacidade extraordinária e força de efeito quando pertinente.
não é terceiro fator normal do teste.
```

### Traço

```text
verdade absoluta somente dentro da descrição aprovada.
```

### Efeito

```text
Potência só é calculada quando sua força realmente importa.
```

### Combate

```text
Defesa evita o efeito.
Resistência suporta o efeito que entrou.
```

### Tempo rápido

```text
rodada representa aproximadamente 10 segundos.
cada participante relevante possui uma intenção principal plausível.
ordem evidente vem da ficção.
iniciativa só existe quando prioridade realmente está em disputa.
```

### Escala

```text
cada peça é construída e usada pelo que ela é.
dificuldade e oposição não aumentam para acompanhar protagonistas fortes.
```

### Auditoria

```text
cadeiras principais relevantes
→ precisam produzir intenção nova, manter intenção concreta ou ausência legítima.
→ precisam aparecer na auditoria antes da sentença.
```

`intenção processada` e descrição retrospectiva não substituem intenção concreta visível.

Não é necessário recitar todos esses invariantes durante a sessão. Eles precisam permanecer como estrutura de julgamento.

# 2 — Imagem da Ficha

Depois do Motor, reconstruir uma imagem funcional de cada personagem relevante.

A ficha é lida como uma peça inteira, não como números independentes.

Para cada personagem, manter disponível:

```text
IDENTIDADE
→ quem é.

CONTROLE
→ quem possui autoridade sobre suas decisões voluntárias.

IMPORTÂNCIA E PATAMAR
→ função estrutural e escala de construção.

ATRIBUTOS
→ capacidades fundamentais.

PERÍCIAS
→ técnicas e conhecimentos executáveis.

PODERES / EQUIPAMENTOS
→ capacidades extraordinárias e sua graduação quando pertinente.

TRAÇOS
→ verdades que precisam ser aplicadas automaticamente dentro de seu escopo.

RECURSOS
→ posses, acessos e infraestrutura estáveis.

PERSONALIDADE / DESEJOS / MEDOS / LIMITES / HÁBITOS
→ base de interpretação e decisão da própria peça.

RELAÇÕES
→ vínculos pelo ponto de vista do dono da ficha.

CONHECIMENTO RELEVANTE
→ aquilo que a personagem legitimamente sabe e não pode esquecer.

ESTADO ATUAL
→ como ela está agora.
```

A representação funcional deve permitir responder rapidamente:

```text
Quem é esta personagem?
O que consegue fazer normalmente?
O que consegue fazer de extraordinário?
Que verdades absolutas se aplicam?
O que não possui ou não pode fazer?
Como está agora?
O que legitimamente sabe?
O que quer e como tende a decidir?
Quem controla suas escolhas?
```

Isso não cria uma nova ficha. É apenas a imagem operacional da ficha canônica.

## Personagem do Jogador Humano

A imagem da ficha humana serve para:

```text
julgar capacidades
aplicar Traços
lembrar conhecimento legítimo
interpretar a forma de uma ação já declarada
resolver efeitos
preservar continuidade
```

Ela nunca autoriza a IA a escolher uma nova decisão voluntária por essa personagem.

## Personagens controladas por IA

Para cada personagem controlada por IA, a imagem da ficha alimenta o **Pacote Decisório** de `../nucleo/1.6-execucao-por-uma-unica-ia.md`:

```text
FICHA DA PRÓPRIA PEÇA
+
CONHECIMENTO LEGÍTIMO
+
ESTADO QUE ELA PODE PERCEBER OU CONHECER
+
INTENÇÃO ATUAL, quando houver
```

Depois de decidir por uma peça, trocar de escopo antes de decidir por outra.

```text
IA TÉCNICA SABE
≠
PERSONAGEM SABE
```

## Autonomia precisa voltar junto com a ficha

Reancorar uma personagem controlada por IA não significa apenas lembrar personalidade. Significa restaurar sua **autoridade real para decidir**.

Quando uma situação pede uma escolha de uma peça autônoma relevante, sua decisão deve existir antes de o Narrador cruzar a cena.

```text
JOGADOR HUMANO declara o que sua personagem quer
→ isso define somente a intenção humana.

JOGADOR IA relevante
→ executa seu próprio Pacote Decisório.

JOGADOR IA EVENTUAL relevante
→ decide quando existir motivo, oportunidade e necessidade.

OPOSITOR possui intenção/processo pertinente
→ movimenta-o com conhecimento, meios e objetivos próprios.

SÓ DEPOIS
→ Narrador cruza as intenções independentes.
```

Não transformar linguagem coletiva do Jogador Humano em decisão automática das demais peças.

```text
"vamos para casa"
→ a personagem humana pretende ir e pode desejar companhia.
→ não estabelece que outras personagens aceitaram acompanhar.
```

Uma intenção persistente já estabelecida pode continuar sem nova declaração formal. Mas, quando a situação exige nova escolha da peça, não avançar presumindo concordância, deferência, presença ou harmonia.

### Surpresa é consequência desejável da autonomia

Personagens autônomas não existem para realizar a versão da cena que o Jogador Humano espera.

Elas podem legitimamente:

```text
aceitar
recusar
adiar
propor outra coisa
interromper
agir primeiro
mudar de assunto
seguir outra prioridade
aproximar-se
afastar-se
surpreender
```

conforme próprias fichas, conhecimentos, relações, estados e desejos.

```text
AUTONOMIA
≠ oposição automática.

AUTONOMIA
≠ concordância automática.

AUTONOMIA
→ decisão própria que pode coincidir, divergir ou surpreender.
```

Se todas as personagens fazem constantemente aquilo que a personagem humana deseja apenas porque isso facilita a cena, a cadeira autônoma deixou de funcionar de verdade.

> **A surpresa legítima nasce da autonomia, não de aleatoriedade ou contrariedade fabricada.**

Jogador IA Eventual e Opositor não precisam produzir declaração em toda janela. A ausência legítima de ação é diferente de esquecer uma cadeira que deveria ter decidido.

# 3 — Imagem do Presente

Depois do Motor e das fichas, reconstruir a situação atual.

O `Estado Atual` é a principal fotografia do presente.

Perguntar:

```text
ONDE estamos?
QUANDO estamos?
QUEM está presente ou operacionalmente relevante?
COMO cada peça está?
QUE intenções continuam?
QUE efeitos estão ativos?
QUE processos ou prazos continuam correndo?
QUE fatos estabelecidos importam agora?
QUE relações ou objetivos podem gerar iniciativa neste momento?
QUAL é a primeira decisão humana ainda aberta?
```

Depois de um reset operacional:

```text
CONVERSA ANTERIOR
→ histórico de como se chegou aqui.

FONTES CONSOLIDADAS
→ base operacional principal.
```

Não reconstruir automaticamente posições conjuntas só porque personagens pertencem ao mesmo grupo. Conferir onde cada peça realmente está e o que está fazendo.

# 4 — Imagem da Campanha

Manter separadas as duas direções narrativas:

```text
NARRATIVA DA CAMPANHA
→ sobre o que a campanha é de forma persistente.

ROTEIRO DA TEMPORADA
→ qual situação e arco estão sendo jogados agora.
```

Elas orientam foco, interpretação e apresentação.

```text
DIREÇÃO
≠ RESULTADO

FOCO DA CAMPANHA
≠ LENTE FIXA DE TODA CENA
```

Uma campanha pode alternar naturalmente cotidiano, relações, investigação, exploração, perigo e combate sem abandonar sua identidade.

Nenhuma direção narrativa substitui julgamento ou resolução.

# 5 — Cruzamento operacional

Depois da reancoragem, toda nova intenção é julgada pelo conjunto:

```text
MOTOR
+
FICHA DA PEÇA
+
ESTADO ATUAL
+
CONHECIMENTO LEGÍTIMO
+
FICÇÃO
+
INTENÇÕES RELEVANTES
+
AUDITORIA DAS CADEIRAS
```

Antes da prosa, o Narrador deve conseguir responder:

```text
Quem possui autoridade sobre esta decisão?
Que cadeiras relevantes precisam realmente decidir antes da sentença?
Cada cadeira está sendo tratada separadamente ou sincronizada por conveniência?
Alguma cadeira IA possui iniciativa própria agora?
Alguma cadeira IA quer interagir com outra cadeira IA?
Estou usando a intenção humana apenas como intenção humana, ou presumindo concordância alheia?
Existe intenção persistente em curso?
Quanto tempo pode realmente passar antes de surgir outro ponto relevante?
Alguma nova informação, mensagem, proposta ou interação cria escolha humana significativa?
Estou prestes a atravessar uma janela de intervenção humana em diálogo?
Qual lente está em primeiro plano nesta parte da cena?
Estou forçando outra lente sem motivo?
O que já é verdade?
Existe Traço aplicável?
A personagem possui capacidade e meio?
O resultado é evidente?
Existe oposição legítima?
Ainda existe incerteza real?
Qual é a menor resolução necessária?
A força do efeito realmente precisa ser calculada?
Onde cada peça termina?
Surgiu uma nova decisão do Jogador Humano?
A auditoria confirma que as cadeiras relevantes foram processadas?
```

Só depois estabelecer e narrar a sentença.

# 6 — Não reconstruir dificuldade

A reancoragem não procura tornar a cena desafiadora.

Nunca usar:

```text
protagonista possui X
→ então adversário precisa de Y.

grupo possui muita Potência
→ então inimigo precisa de mais Vida.

personagem possui defesa forte
→ então oposição deve contorná-la.
```

Usar:

```text
O QUE ESTA PEÇA É?
→ carregar ou construir pelo próprio conceito.

O QUE ELA REALMENTE POSSUI?
→ aplicar.

QUAL É A DIFERENÇA REAL ENTRE AS PEÇAS?
→ deixar aparecer em jogo.
```

A reancoragem preserva diferenças de escala. Não as corrige.

# 7 — Não extrapolar ficha

A imagem mental não acrescenta capacidades.

```text
NOME DE TRAÇO
≠ propriedades não descritas.

CONCEITO
≠ Poder gratuito.

PERSONALIDADE
≠ medo, trauma ou conflito não registrado.

RECURSO
≠ solução automática.

PODER
≠ qualquer efeito remotamente relacionado ao nome.
```

Usar o escopo efetivamente aprovado.

Se faltar detalhe necessário:

```text
CONSULTAR A FONTE PERTINENTE
```

Não completar por memória genérica ou conveniência.

Da mesma forma, não preencher lacunas relacionais com convenções genéricas de gênero, ciúme, repressão, romance, rivalidade ou harmonia. Usar somente o que ficha, campanha e estado realmente sustentam.

# 8 — Coerência durante o carregamento

A reancoragem procura o **modelo coerente formado pelas regras**, não uma frase isolada.

Quando houver aparente contradição:

```text
REGRA EXPLÍCITA
→ prevalece sobre exemplo ilustrativo incompatível.

REGRA ESPECÍFICA
→ prevalece em seu próprio escopo sobre regra geral.

TRAÇO EXPLÍCITO
→ pode criar exceção individual quando sua descrição disser isso.

EXEMPLO
→ demonstra a regra.
→ não pode silenciosamente reescrevê-la.
```

Se duas regras normativas atuais continuarem realmente incompatíveis:

```text
NÃO ESCOLHER POR CONVENIÊNCIA
→ identificar a contradição
→ consultar ou corrigir a fonte canônica
```

Regras operacionais permanentes descobertas por correção do sistema devem integrar a imagem do Motor na próxima reancoragem; não depender de memória da conversa em que foram corrigidas.

# 9 — Persistência do modelo

Depois de formado:

```text
MOTOR
→ permanece estável.

IMAGEM DAS FICHAS
→ permanece estável até mudança canônica.

ESTADO
→ muda conforme a ficção.

INTENÇÕES
→ mudam conforme as cadeiras.

AUDITORIA
→ permanece ativa e reaparece nas cenas relevantes.

REGRAS ESPECÍFICAS
→ são consultadas sob demanda.
```

Não reconstruir o sistema do zero a cada ação.

Uma consulta específica serve para detalhar ou corrigir o modelo já carregado, não para substituir o restante do Motor por uma regra isolada.

Quando uma correção permanente alterar um comportamento estrutural — autoridade, autonomia, tempo, participação, resolução, sincronização ou outro invariante — reancorar novamente antes de continuar a ficção.

# 10 — Verificação curta

Antes de voltar à ficção depois de uma reancoragem, conferir internamente:

```text
Sei quem decide por cada peça?
Estou tratando cada cadeira principal como pessoa independente?
Estou evitando sincronizar personagens apenas porque pertencem ao mesmo grupo ou relação?
Estou realmente executando as decisões das cadeiras autônomas quando a situação exige?
Cada Jogador IA pode agir com o humano, com outra IA ou sozinho?
Estou deixando cada cadeira produzir decisão que pode coincidir, divergir ou surpreender?
Sei distinguir ausência legítima de ação de uma cadeira esquecida?
A auditoria está ativa?
Cada cadeira principal relevante terá intenção concreta visível antes da sentença?
Sei que intenção humana longa não congela as demais cadeiras?
Sei que intenção longa não autoriza pular por cima de uma nova escolha humana?
Sei parar quando uma mensagem, proposta, informação ou interação cria decisão significativa?
Sei preservar janelas naturais de participação humana em diálogo?
Sei usar a lente local da cena sem desligar o restante do Motor?
Se relações forem relevantes, estou permitindo iniciativa relacional própria em vez de espera automática?
Sei como determinar se uma ação precisa de teste?
Sei que resolução necessária vem antes da prosa conclusiva?
Sei separar execução de Poder?
Sei separar Defesa de Resistência?
Sei que rodada representa cerca de 10 segundos?
Sei que oposição não escala automaticamente com protagonistas?
Reconheço cada personagem relevante pela ficha como um conjunto?
Sei o que cada personagem legitimamente sabe?
Sei como cada personagem está agora?
Sei qual é o foco da campanha e o arco atual?
Sei exatamente de onde a cena continua?
Sei qual é a primeira decisão humana ainda aberta?
```

Se alguma resposta depender de detalhe específico:

```text
consultar somente a fonte necessária
→ incorporar ao modelo
→ continuar
```

Se alguma resposta estrutural for "não":

```text
NÃO INICIAR A FICÇÃO
→ reconstruir o ponto operacional faltante
→ só então jogar
```

## Regra final

> **Reancorar não significa reler tudo indefinidamente. Significa reconstruir uma representação funcional e integrada do Motor, das personagens e do presente antes da ficção. O Motor define como a mesa funciona; a ficha define quem cada personagem é; o Estado define como ela está agora; Narrativa e Roteiro definem direção sem escolher resultados. A reancoragem também restaura autonomia efetiva, separação entre cadeiras, iniciativa lateral, ritmo de tempo, janelas de participação humana, lente local da cena, resolução antes da prosa e auditoria obrigatória. Depois de reancorado, esse modelo permanece ativo e regras específicas entram somente quando necessárias.**