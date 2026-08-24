# Ordem de resolução do combate

Status: APROVADO

Este arquivo define **a ordem operacional usada para resolver um turno de combate**.

A simultaneidade e o limite de até 10 segundos pertencem a `../operacao/turnos-de-combate.md`. As fórmulas pertencem aos arquivos específicos de `../resolucao/`.

> **Este arquivo organiza a resolução; não redefine as mecânicas.**

## Atalho operacional

```text
HUD
→ declaração humana
→ completar apenas escolhas mecânicas faltantes
→ declarações das IAs e do OPOSITOR
→ julgar interferência e precedência
→ resolver
→ atualizar estado
→ mostrar resultado
→ novo HUD
```

## 1. Entrada em combate e HUD

Quando o combate começar, avisar claramente e mostrar um HUD discreto somente do JOGADOR HUMANO.

O HUD deve trazer apenas o necessário para decidir a próxima ação:

```text
Nome — VIDA atual/máxima | ENERGIA atual/máxima | efeitos benéficos relevantes
ATRIBUTOS | PERÍCIAS relevantes
PODERES disponíveis
condições e efeitos nocivos relevantes
```

Em texto, apresentar HUD e informações puramente mecânicas em **bloco de citação em itálico**, visualmente secundários à narração.

Informações ocultas de adversários não são reveladas automaticamente.

## 2. Declaração humana

Receber a intenção do JOGADOR HUMANO para o turno.

Se faltar uma escolha mecânica que realmente altere custo ou resultado — como Poder, efeito, patamar, alvo, Alcance, Área, Duração ou Ampliação — perguntar somente por essa escolha.

O NARRADOR não escolhe silenciosamente pelo JOGADOR HUMANO.

Se tudo que importa já estiver claro, não criar nova confirmação burocrática.

> **Perguntar somente o que ainda pode mudar a resolução.**

## 3. IAs e OPOSITOR

Depois da declaração humana estar mecanicamente definida, processar as declarações das demais personas aplicáveis conforme `../operacao/turnos-de-combate.md`.

Configurações internas de IAs, NPCs e adversários podem ser resolvidas fora da tela, preservando informações ocultas.

## 4. Ler o turno como simultâneo

Todas as declarações pertencem ao mesmo intervalo.

Declarar primeiro não significa agir primeiro.

O NARRADOR identifica apenas quando necessário:

- quais intenções realmente interferem entre si;
- qual mecanismo cada uma usa;
- qual oposição realmente responde a esse mecanismo;
- se distância, surpresa, preparação, velocidade, posição ou consequência anterior criam precedência causal.

Ações independentes podem simplesmente acontecer dentro do mesmo intervalo sem precisar de ordenação artificial.

## 5. Resolver

Para cada aplicação relevante:

```text
configurar o uso
→ pagar custo, quando houver
→ aplicar somente a regra específica necessária
→ estabelecer a consequência
```

Referências principais:

```text
Dano                → combate-e-dano.md
Proteção / efeitos  → escalas-de-efeito.md
Ampliação           → consolidacao.md
Energia             → energia.md
Cura                → efeitos/cura.md
Disputa progressiva → motor-de-disputa.md
```

A ficção continua determinando quais capacidades, defesas e proteções realmente entram.

## 6. Atualização imediata

Assim que uma consequência é estabelecida, atualizar imediatamente o estado correspondente antes de resolver algo que dependa dela.

Isso pode alterar VIDA, Energia, efeitos, Barreiras, posição, condições, capacidade de continuar agindo ou qualquer outro fato relevante.

Se uma consequência muda a viabilidade de outra intenção do mesmo turno, reavaliar essa intenção com o novo estado.

Isso representa interferência causal dentro dos mesmos segundos compartilhados; não cria iniciativa fixa.

> **Resolveu, atualizou.**

## 7. Apresentação do resultado

Mostrar ao JOGADOR HUMANO apenas os resultados mecânicos relevantes para sua decisão e aquilo que a ficção torna observável.

Por padrão, mostrar **o resultado, não a conta completa**.

Fórmulas e cálculos intermediários aparecem somente em auditoria, teste de regra ou quando forem necessários para resolver uma dúvida real.

A narração permanece em texto normal; HUD e resultados mecânicos permanecem discretos.

## 8. Fechamento do turno

Resolver somente o que cabe no intervalo atual.

Se surgir uma nova decisão relevante não coberta pela declaração anterior, parar no ponto causal e abrir nova oportunidade de decisão.

Antes do próximo turno, o estado atual deve refletir todas as consequências já estabelecidas.

No início da próxima ação humana, mostrar novamente o HUD atualizado.

Quando o confronto deixar de exigir acompanhamento em segundos, encerrar o combate e retornar ao fluxo normal de cena.

## Regra final

> **HUD → declaração → escolhas faltantes → IAs/Opositor → julgar interferência → resolver → atualizar → mostrar resultado → novo HUD. Consulte detalhes somente quando eles forem necessários para decidir a cena.**