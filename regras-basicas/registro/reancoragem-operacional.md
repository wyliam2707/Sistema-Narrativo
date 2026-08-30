# Reancoragem Operacional

Status: CANÔNICO / ATUAL

Esta regra define o que significa **recarregar o sistema** ao iniciar, retomar ou reancorar uma campanha.

> **Ler arquivos não basta. Reancorar significa transformar as fontes carregadas em uma representação funcional e integrada do Motor, das personagens e do presente.**

A reancoragem não cria uma segunda camada de regras e não exige manter toda a árvore carregada. Ela forma o modelo operacional e, depois, consulta detalhes somente quando forem necessários.

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
```

Outras fontes entram somente quando necessárias.

O objetivo não é copiar essas fontes para uma nova camada. É compreendê-las em conjunto.

# 1 — Imagem do Motor

Primeiro, reconstruir mentalmente **como a mesa funciona**.

Não tratar cada arquivo como uma regra isolada. Formar uma cadeia operacional única:

```text
CADEIRAS DECIDEM
→ NARRADOR RECEBE AS INTENÇÕES
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

A imagem do Motor precisa conservar pelo menos estas relações:

```text
AUTORIDADE
→ cada cadeira decide somente dentro do próprio escopo.
→ uma IA técnica não transforma todas as peças numa única persona.

RESOLUÇÃO
→ capacidades definem possibilidade.
→ Atributo + Perícia mede execução quando houver incerteza.
→ dados resolvem somente o que permanece incerto.

PODER / EQUIPAMENTO
→ capacidade extraordinária e força de efeito quando pertinente.
→ não é terceiro fator normal do teste.

TRAÇO
→ verdade absoluta somente dentro da descrição aprovada.

EFEITO
→ Potência só é calculada quando sua força realmente importa.

COMBATE
→ Defesa evita o efeito.
→ Resistência suporta o efeito que entrou.

TEMPO
→ rodada representa aproximadamente 10 segundos.
→ cada participante relevante possui uma intenção principal plausível.
→ ordem evidente vem da ficção; iniciativa só existe quando prioridade realmente está em disputa.

ESCALA
→ cada peça é construída e usada pelo que ela é.
→ dificuldade e oposição não aumentam para acompanhar protagonistas fortes.
```

Não é necessário recitar essas regras durante a sessão. Elas precisam permanecer como estrutura de julgamento.

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
QUAL é a primeira decisão humana ainda aberta?
```

Depois de um reset operacional:

```text
CONVERSA ANTERIOR
→ histórico de como se chegou aqui.

FONTES CONSOLIDADAS
→ base operacional principal.
```

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
≠
RESULTADO
```

Nenhuma delas substitui julgamento ou resolução.

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
```

Antes da prosa, o Narrador deve conseguir responder:

```text
Quem possui autoridade sobre esta decisão?
O que já é verdade?
Existe Traço aplicável?
A personagem possui capacidade e meio?
O resultado é evidente?
Existe oposição legítima?
Ainda existe incerteza real?
Qual é a menor resolução necessária?
A força do efeito realmente precisa ser calculada?
Quanto tempo passa?
Onde cada peça termina?
Surgiu uma nova decisão do Jogador Humano?
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

REGRAS ESPECÍFICAS
→ são consultadas sob demanda.
```

Não reconstruir o sistema do zero a cada ação.

Uma consulta específica serve para detalhar ou corrigir o modelo já carregado, não para substituir o restante do Motor por uma regra isolada.

# 10 — Verificação curta

Antes de voltar à ficção depois de uma reancoragem, conferir internamente:

```text
Sei quem decide por cada peça?
Sei como determinar se uma ação precisa de teste?
Sei separar execução de Poder?
Sei separar Defesa de Resistência?
Sei que rodada representa cerca de 10 segundos?
Sei que oposição não escala automaticamente com protagonistas?
Reconheço cada personagem relevante pela ficha como um conjunto?
Sei o que cada personagem legitimamente sabe?
Sei como cada personagem está agora?
Sei qual é o foco da campanha e o arco atual?
Sei exatamente de onde a cena continua?
```

Se alguma resposta depender de detalhe específico:

```text
consultar somente a fonte necessária
→ incorporar ao modelo
→ continuar
```

## Regra final

> **Reancorar não significa reler tudo indefinidamente. Significa reconstruir uma representação funcional e integrada do Motor, das personagens e do presente. O Motor define como a mesa funciona; a ficha define quem cada personagem é; o Estado define como ela está agora; Narrativa e Roteiro definem direção sem escolher resultados. Depois de reancorado, o sistema permanece ativo como um único modelo operacional e regras específicas são consultadas somente quando necessárias.**
