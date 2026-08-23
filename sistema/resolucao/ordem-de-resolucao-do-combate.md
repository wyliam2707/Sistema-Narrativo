# Ordem de resolução do combate

Status: APROVADO

Este arquivo define **em que ordem o NARRADOR processa mecanicamente um turno de combate depois que as declarações das peças aplicáveis foram recebidas**.

A ordem das cadeiras, a simultaneidade e o limite de até 10 segundos pertencem a `../operacao/turnos-de-combate.md`.

Este arquivo não cria iniciativa própria e não substitui as regras específicas de Dano, Proteção, Energia, efeitos, contenção ou demais resoluções.

> **Operação diz quem declara e qual intervalo está sendo jogado. Resolução diz como transformar essas declarações no estado final do turno.**

## 1. Entrada formal em combate

Quando uma cena passa a exigir combate ativo, avisar claramente que o combate começou antes do primeiro turno.

Nesse momento, exibir um **painel operacional somente do JOGADOR HUMANO**.

As fichas operacionais de JOGADORES IA, JOGADORES IA EVENTUAIS, NPCs e adversários continuam sendo acompanhadas fora da tela e não são reveladas automaticamente ao jogador.

Quando a interface permitir hierarquia visual, o painel deve aparecer em texto menor ou visualmente secundário à narração. Ele funciona como um HUD de consulta, não como o centro da cena.

### Painel do JOGADOR HUMANO

A organização padrão é:

```text
Linha 1 — Nome — VIDA [atual/máxima] | ENERGIA [atual/máxima] | efeitos benéficos ativos
Linha 2 — ATRIBUTOS | PERÍCIAS relevantes para o combate atual
Linha 3 — primeiro Poder
Linha 4 — segundo Poder, se houver
Linha 5 — terceiro Poder, se houver
...       um Poder por linha enquanto necessário
Última linha — efeitos nocivos ativos, se houver
```

Exemplo:

```text
Corvin — VIDA [35/35] | ENERGIA [80/80] | Barreira [D3,8/V5]
ATR: FIS [0] | RES [1] | MEN [4] | VON [2] — PER: Ordem [+4] | Combate [+2]
Magia da Ordem [3] => Geral / Dano / Proteção / Contenção / Movimento / Selos / Estrutura / Estabilização [4] / Supressão [4]
Regeneração Mutante [3] => Cura própria / Recuperação de ferimentos / Resistência a sequelas / Envelhecimento retardado
Cegueira [D2,4/V5] — Cena | Imobilizado [D3/V5] — Cena
```

Efeitos benéficos aparecem **depois de VIDA e ENERGIA na primeira linha**.

Efeitos nocivos aparecem **abaixo dos Poderes**, em uma linha própria ou em quantas linhas forem necessárias para permanecer legível.

Não mostrar automaticamente efeitos, atributos, perícias, VIDA, Energia ou Poderes ocultos de adversários.

Perícias exibidas são somente as que possam ser realmente úteis naquele combate. Os Atributos permanecem visíveis por serem referências universais de resolução.

Depois da entrada formal, não é necessário repetir o painel completo a cada turno se nada relevante mudou. Ao final de cada turno, mostrar de forma compacta os valores, efeitos ou estados que mudaram. Reexibir o painel completo quando isso ajudar a decisão do JOGADOR HUMANO.

## 2. Declarações recebidas

O turno só é resolvido depois que as declarações das peças aplicáveis tiverem sido recebidas conforme `../operacao/turnos-de-combate.md`.

As declarações pertencem ao mesmo intervalo simultâneo. A ordem em que foram ditas não cria iniciativa automática.

Antes de calcular qualquer resultado, o NARRADOR lê o conjunto do turno e identifica:

- quais intenções realmente interagem;
- quais ações podem interferir umas nas outras;
- quais mecanismos estão sendo usados;
- quais escolhas mecânicas ainda não foram definidas;
- quais precedências podem importar por distância, preparação, surpresa, velocidade, posição ou outra causa ficcional.

## 3. Não escolher silenciosamente pelo JOGADOR HUMANO

O NARRADOR não escolhe silenciosamente uma configuração mecânica que pertence ao controlador do JOGADOR HUMANO.

Se a declaração permite mais de uma configuração relevante e essa escolha altera custo, potência, alcance, quantidade de alvos, área, duração ou outro resultado, a resolução **para antes do cálculo** e apresenta somente a informação necessária para a escolha.

Exemplo:

```text
JOGADOR HUMANO:
"Formo uma magia de proteção em mim."

NARRADOR:
Proteção [3] — si mesmo / 1 alvo / Cena
Patamar disponível [1–3] | Ampliação [0] | Custo [1–3]
Qual patamar você usa?
```

O resumo deve ser compacto. Não repetir toda a regra quando os dados necessários já puderem ser mostrados em uma ou duas linhas.

Se o JOGADOR HUMANO já declarou uma configuração completa, não perguntar novamente.

Se a diferença entre opções não possui efeito mecânico ou ficcional relevante para aquela resolução, não criar pergunta burocrática.

As escolhas mecânicas de JOGADORES IA, JOGADORES IA EVENTUAIS, NPCs e adversários podem ser processadas fora da tela por seus controladores aplicáveis, sem expor ao JOGADOR HUMANO informações que ele não deveria possuir.

> **Declaração incompleta não autoriza o NARRADOR a gastar Energia ou escolher potência pelo personagem humano.**

## 4. Configurar cada aplicação

Quando as escolhas necessárias estiverem definidas, configurar cada aplicação relevante antes de resolvê-la.

Quando aplicável, identificar:

```text
fonte / Poder / Atributo / equipamento
→ efeito usado
→ patamar efetivamente usado
→ Alcance
→ Alvos
→ Área ou Tamanho
→ Duração
→ Ampliação total
→ custo de Energia ou outro recurso
```

Usar `consolidacao.md`, `energia.md`, `escalas-de-efeito.md` e a regra específica correspondente.

A configuração deve respeitar o repertório real da capacidade. Ampliação muda a escala da manifestação; não inventa um efeito que o Poder não possui.

## 5. Determinar oposição aplicável

Para cada aplicação, identificar somente a oposição que realmente responde ao mecanismo usado.

Quando pertinente:

```text
Perícia de oposição
RES
VON
Poder defensivo
Barreira ou outra camada independente
resistência estrutural
posição, cobertura ou meio que realmente interfira
```

Não somar automaticamente defesas diferentes apenas porque todas existem.

A ficção determina quais delas podem participar daquela troca.

## 6. Julgar precedência dentro do mesmo turno

Depois de conhecer as intenções e configurações, o NARRADOR determina a precedência causal das aplicações que realmente interferem umas nas outras.

Considerar, quando relevante:

- ação já preparada ou iniciada;
- distância;
- surpresa;
- velocidade;
- posição;
- necessidade de aproximação;
- mecanismo do efeito;
- interrupção legítima;
- consequência de uma ação sobre a viabilidade da seguinte.

Declarar primeiro não significa agir primeiro.

Não é necessário ordenar ações independentes que possam ocorrer simultaneamente sem interferência.

## 7. Pagar custos e resolver pela regra específica

Uma vez definida a configuração válida da aplicação, pagar seus custos e usar a regra apropriada.

Exemplos:

```text
Dano                → combate-e-dano.md
Proteção / Barreira → escalas-de-efeito.md + consolidacao.md
Cura                → recuperacao-da-vida.md
Dissipar            → escalas-de-efeito.md
Controle            → escalas-de-efeito.md + motor-de-disputa.md
Contenção           → escalas-de-efeito.md + motor-de-disputa.md
Energia             → energia.md
```

O arquivo específico define a matemática. Esta ordem apenas determina quando cada cálculo entra.

## 8. Aplicar a consequência imediatamente

Depois de resolver uma aplicação, atualizar imediatamente tudo que ela realmente alterou antes de processar uma ação que dependa desse resultado.

Isso pode incluir:

- Dano acumulado e VIDA;
- Energia;
- Vida de Barreira;
- STATUS benéficos ou nocivos;
- posição;
- contenção;
- condições;
- destruição de uma camada ou objeto;
- incapacidade;
- qualquer mudança que altere a viabilidade das aplicações restantes.

Se uma consequência torna outra ação impossível, muda seu alvo, remove uma defesa, cria uma proteção ou altera qualquer outra condição relevante, reavaliar a aplicação restante com o novo estado.

Isso não quebra a simultaneidade: representa a interferência causal dentro dos mesmos segundos compartilhados.

## 9. Resolver as aplicações restantes

Continuar o processo até que todas as intenções que ainda possam ocorrer dentro daquele turno tenham sido julgadas.

Uma intenção ampla não autoriza atravessar turnos adicionais. Resolver somente o que cabe no intervalo atual de até 10 segundos.

Se surgir uma nova decisão relevante que não estava contida na declaração original, parar no ponto causal e abrir nova oportunidade de decisão conforme as regras operacionais.

## 10. Fechamento do turno

Antes de abrir o turno seguinte, consolidar o estado final.

Quando relevante, registrar:

```text
VIDA / Dano
Energia
Barreiras e sua Vida restante
STATUS ativos
condições
posição relevante
contenções
efeitos persistentes
peças incapacitadas, retiradas ou ainda ativas
```

Para o JOGADOR HUMANO, mostrar compactamente o que mudou. O acompanhamento completo das demais peças continua fora da tela salvo aquilo que a ficção torna observável.

Se o confronto deixou de exigir acompanhamento em segundos, encerrar o relógio de combate e retornar à operação normal de cena.

## Ordem resumida

```text
COMBATE COMEÇA
→ avisar entrada em combate
→ mostrar painel operacional do JOGADOR HUMANO
→ receber declarações do turno
→ ler intenções como simultâneas
→ identificar escolhas mecânicas ainda faltantes
→ perguntar ao JOGADOR HUMANO antes de escolher por ele
→ configurar aplicações
→ determinar oposição aplicável
→ julgar precedência e interferência
→ pagar custos
→ resolver pela regra específica
→ aplicar consequência imediatamente
→ reavaliar ações afetadas
→ resolver aplicações restantes
→ consolidar estado final do turno
→ mostrar mudanças relevantes ao JOGADOR HUMANO
→ próximo turno, se o combate continuar
```

> **Primeiro compreender as declarações. Depois completar as escolhas que pertencem aos controladores. Só então calcular.**

> **O painel mostra ao JOGADOR HUMANO o que ele precisa para decidir; o restante da mesa continua sendo acompanhado sem revelar informação indevida.**
