# Ordem Operacional do Combate

Status: APROVADO

Este arquivo define **como aplicar o sistema durante um turno de combate**.

A duração e simultaneidade do turno pertencem a `turnos-de-combate.md`. As fórmulas e resultados mecânicos pertencem a `../resolucao/`.

> **Operação organiza a sequência. Resolução calcula.**

## Atalho operacional

```text
HUD
→ declaração humana
→ completar somente escolhas mecânicas faltantes
→ declarações das demais personas
→ julgar interferência e precedência
→ aplicar resoluções necessárias
→ atualizar estado
→ apresentar resultado
→ novo HUD
```

## 1. Entrada e HUD

Ao entrar em combate, sinalizar claramente e mostrar um HUD discreto do JOGADOR HUMANO apenas com informação necessária para decidir:

```text
Nome — Vida atual/máxima | Mana atual/máxima | Trama, quando aplicável
Atributos e Perícias relevantes
Poderes e recursos relevantes
Status, Barreiras e efeitos ativos relevantes
```

Não revelar automaticamente informação oculta de adversários.

A forma visual do HUD pode seguir `../narracao/` sem transformar apresentação em regra mecânica.

## 2. Declaração humana

Receber a intenção do JOGADOR HUMANO.

Se faltar uma escolha que realmente altere custo ou resultado — Poder, alvo, Alcance, Área, Duração, intensidade, modo ou outra opção de Hub — perguntar somente essa escolha.

Se tudo já estiver claro, não criar confirmação burocrática adicional.

> **Perguntar somente o que ainda pode mudar a resolução.**

## 3. Demais declarações

Depois da intenção humana estar suficientemente definida, receber/processar as declarações das demais personas aplicáveis conforme `turnos-de-combate.md` e `../personas/`.

Configurações ocultas de adversários podem ser resolvidas sem expor informação reservada ao jogador.

## 4. Ler o intervalo como simultâneo

Todas as declarações pertencem ao mesmo intervalo de até 10 segundos.

Declarar primeiro não significa agir primeiro.

O NARRADOR identifica somente quando necessário:

- quais intenções interferem entre si;
- qual mecanismo cada intenção usa;
- quais reações realmente respondem a esse mecanismo;
- se distância, surpresa, preparação, velocidade, posição ou ação já iniciada estabelecem precedência.

Ações independentes podem coexistir sem ordenação artificial.

Quando duas ações competirem pelo mesmo instante e a ficção não decidir a precedência, usar uma oposição comum conforme `../resolucao/motor-de-disputa.md`.

Esse teste decide apenas aquela interferência local; não cria iniciativa permanente.

## 5. Aplicar a resolução necessária

Para cada incerteza relevante:

```text
configurar o uso, quando necessário
→ pagar custo válido
→ resolver CD ou oposição somente se houver incerteza
→ aplicar Dano/Efeito/Status conforme a regra específica
→ estabelecer consequência
```

Fontes mecânicas principais:

```text
motor universal        → ../resolucao/motor-de-disputa.md
combate / Dano / RD    → ../resolucao/combate-e-dano.md
Vida                    → ../resolucao/vida.md
recuperação             → ../resolucao/recuperacao-da-vida.md
Mana                    → ../resolucao/mana.md
Poderes e Hubs          → ../resolucao/poderes/
Status                  → ../resolucao/status/
Trama                    → ../personagem/trama.md
```

## 6. Atualização causal imediata

Assim que uma consequência for estabelecida, atualizar o estado antes de resolver outra intenção que dependa dela.

Isso pode alterar:

- Vida;
- Mana;
- Trama;
- Status;
- Barreiras;
- posição;
- alterações temporárias de Atributo;
- possibilidade de continuar uma intenção já declarada.

Se a nova consequência muda outra ação do mesmo intervalo, reavaliar essa ação com o estado atualizado.

> **Resolveu, atualizou.**

Isso representa causalidade dentro do mesmo turno simultâneo; não cria fila fixa.

## 7. Apresentação

Mostrar ao JOGADOR HUMANO apenas resultados mecânicos relevantes à decisão e aquilo que a ficção torna observável.

Por padrão, mostrar o resultado, não toda a conta intermediária.

A forma narrativa pertence a `../narracao/`.

## 8. Fechamento do turno

Resolver somente o que cabe no intervalo atual.

```text
surge nova decisão relevante
→ parar no ponto causal

intervalo chega ao limite
→ fechar o turno
```

Antes do próximo turno, `../persistencia/` deve refletir o estado já estabelecido.

Se o confronto deixar de exigir acompanhamento em segundos, retornar a `janelas-e-interrupcoes.md`.

## Regra final

> **HUD → declarações → interferência → resolução necessária → atualização → apresentação → novo HUD. `operacao/` determina a ordem; `resolucao/` determina os resultados.**
