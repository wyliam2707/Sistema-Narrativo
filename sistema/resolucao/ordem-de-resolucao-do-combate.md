# Ordem de resolução do combate

Status: APROVADO

Este arquivo define **em que ordem o NARRADOR processa mecanicamente um turno de combate depois que as declarações das peças aplicáveis foram recebidas**.

A ordem das cadeiras, a simultaneidade e o limite de até 10 segundos pertencem a `../operacao/turnos-de-combate.md`.

Este arquivo não cria iniciativa própria e não substitui as regras específicas de Dano, Proteção, Energia, efeitos, contenção ou demais resoluções.

> **Operação diz quem declara e qual intervalo está sendo jogado. Resolução diz como transformar essas declarações no estado final do turno.**

## 0. Atalho operacional — HUD / combate

Sempre que um combate começar ou uma nova ação do JOGADOR HUMANO estiver prestes a ser declarada, seguir mentalmente este atalho:

```text
HUD → declaração → confirmação mecânica, se necessária → IAs → OPOSITOR → resolver → atualizar estado → novo HUD
```

Ao iniciar combate:

```text
1. avisar claramente que o combate começou;
2. mostrar o HUD discreto do JOGADOR HUMANO;
3. receber a declaração humana;
4. confirmar apenas escolhas mecânicas ainda necessárias;
5. depois receber/processar IAs e OPOSITOR;
6. resolver o turno;
7. mostrar resultados mecânicos discretos;
8. no início da próxima ação humana, mostrar novamente o HUD atualizado.
```

> **Atalho: HUD → declarar → confirmar → IAs/Opositor → resolver → atualizar.**

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

Depois da entrada formal, não é necessário repetir o painel completo a cada turno se nada relevante mudou. Ao início de cada nova ação do JOGADOR HUMANO, porém, o HUD deve ser reapresentado de forma discreta para mostrar o estado atualizado que fundamenta sua decisão.

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
"Uso Proteção [3] em mim."

NARRADOR:
<small>Proteção [3] — si mesmo / 1 alvo / Cena — Ampliação máx. [7] — Custo [3]</small>

Confirmar?
```

Se houver uma configuração incompleta ou uma dimensão insuficiente, recomendar sem decidir:

```text
<small>Alvo além do Alcance Médio. Recomendo Longo [+1] → custo total [4].</small>

Confirmar Proteção [3] + Longo [+1]?
```

O resumo deve ser compacto. Não repetir toda a regra quando os dados necessários já puderem ser mostrados em uma ou duas linhas.

Se o JOGADOR HUMANO já declarou uma configuração completa e ela é válida, não perguntar novamente; apenas confirmar quando a regra exigir confirmação antes de fechar a declaração.

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

Quando um Poder possuir um **Atributo-base fixo** para Ampliação, esse Atributo já estabelecido na ficha é usado automaticamente. O NARRADOR não escolhe outro Atributo durante o combate apenas para aumentar a Ampliação possível.

Exemplo:

`Magia da Ordem [3] | Atributo-base: MEN [4] → Ampliação máxima [7]`.

Um Poder corporal pode ter `FIS` ou `RES` como Atributo-base conforme sua definição aprovada; depois de definido, o vínculo permanece fixo até alteração permanente da ficha.

## 5. Processamento das IAs fora da tela

JOGADORES IA e JOGADORES IA EVENTUAIS podem realizar internamente o mesmo procedimento de configuração exigido do JOGADOR HUMANO:

```text
declaração → escolher patamar → verificar alcance/alvos/área/duração → calcular Ampliação → verificar custo → corrigir configuração, se necessário → declaração final
```

Esse processo não precisa aparecer na tela. O NARRADOR mostra apenas a intenção final relevante à ficção e os resultados mecânicos que o JOGADOR HUMANO precisa conhecer.

O mesmo vale para NPCs e peças do OPOSITOR, respeitados os segredos que não devem ser revelados.

## 6. Determinar oposição aplicável

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

## 7. Julgar precedência dentro do mesmo turno

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

## 8. Pagar custos e resolver pela regra específica

Uma vez definida a configuração válida da aplicação, pagar seus custos e usar a regra apropriada.

Exemplos:

```text
Dano                → combate-e-dano.md
Proteção / Barreira → escalas-de-efeito.md + consolidacao.md
Cura                → recuperacao-da-vida.md
Dissipar            → escalas-de-efeito.md
Controle            → escalas-de-efeito.md + motor-de-disputa.md
Contenção            → escalas-de-efeito.md + motor-de-disputa.md
Energia             → energia.md
```

O arquivo específico define a matemática. Esta ordem apenas determina quando cada cálculo entra.

## 9. Mostrar apenas resultados mecânicos relevantes

Toda informação puramente mecânica deve ser apresentada em formato visual discreto, preferencialmente com texto menor, para diferenciá-la da narrativa.

A regra padrão é **mostrar o resultado, não a conta completa**.

Exemplos:

```text
<small>Proteção concluída → Proteção [D3,8 / V5] | Energia [77/80]</small>
<small>Cultista 1 sofre 4 Dano → VIDA [1/5]</small>
<small>Cura: +8 VIDA → VIDA [23/35]</small>
<small>Energia −4 → [73/80]</small>
<small>Barreira sofre 3 Dano → V2/5</small>
```

Fórmulas e cálculos intermediários permanecem ocultos por padrão. Exibi-los somente quando o JOGADOR HUMANO pedir uma auditoria, quando estivermos testando especificamente uma regra ou quando a transparência do cálculo for necessária para resolver uma dúvida.

A narrativa continua em texto normal. HUD, confirmações, custos, resultados e demais informações puramente mecânicas usam o formato discreto.

## 10. Aplicar a consequência imediatamente

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

## 11. Resolver as aplicações restantes

Continuar o processo até que todas as intenções que ainda possam ocorrer dentro daquele turno tenham sido julgadas.

Uma intenção ampla não autoriza atravessar turnos adicionais. Resolver somente o que cabe no intervalo atual de até 10 segundos.

Se surgir uma nova decisão relevante que não estava contida na declaração original, parar no ponto causal e abrir nova oportunidade de decisão conforme as regras operacionais.

## 12. Fechamento do turno

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
→ mostrar HUD operacional do JOGADOR HUMANO
→ receber declaração humana
→ confirmar escolhas mecânicas, se necessário
→ processar declarações das IAs e do OPOSITOR
→ ler intenções como simultâneas
→ identificar escolhas mecânicas ainda faltantes
→ configurar aplicações
→ determinar oposição aplicável
→ julgar precedência e interferência
→ pagar custos
→ resolver pela regra específica
→ aplicar consequência imediatamente
→ mostrar resultados mecânicos discretos
→ reavaliar ações afetadas
→ resolver aplicações restantes
→ consolidar estado final do turno
→ novo HUD na próxima ação humana
→ próximo turno, se o combate continuar
```

> **Primeiro compreender as declarações. Depois completar as escolhas que pertencem aos controladores. Só então calcular.**

> **O painel mostra ao JOGADOR HUMANO o que ele precisa para decidir; o restante da mesa continua sendo acompanhado sem revelar informação indevida.**
