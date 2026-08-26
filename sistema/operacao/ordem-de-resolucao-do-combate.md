# Ordem Operacional do Combate

Status: APROVADO

Este arquivo define **como aplicar o sistema durante um turno de combate**.

A duração e simultaneidade do turno pertencem a `turnos-de-combate.md`. As fórmulas e resultados mecânicos pertencem a `../resolucao/`.

> **Operação organiza a sequência. Resolução calcula.**

## Atalho operacional

```text
HUD
→ declaração humana
→ apresentar Hub, quando um Poder for declarado
→ completar automaticamente escolhas mecânicas não declaradas
→ declarações das demais personas
→ julgar interferência e precedência
→ aplicar resoluções necessárias
→ atualizar estado
→ apresentar resultado
→ novo HUD
```

## 1. Entrada e HUD

Ao entrar em combate, sinalizar claramente e mostrar um HUD discreto do JOGADOR HUMANO apenas com informação necessária para decidir.

O formato padrão é compacto e não usa linhas vazias dentro do bloco:

```text
Nome — Vida atual/máxima | Mana atual/máxima | Trama, quando aplicável
Potência [X] · Controle [X] · Resistência [X]
Intelecto [X] · Presença [X] · Vontade [X]
Perícias > Perícia 1, Perícia 2, Perícia 3
Poderes > Poder 1, Poder 2, Poder 3
Status > nenhum
Barreira > nenhuma
```

Regras de apresentação do HUD:

- mostrar sempre os **seis Atributos**, inclusive valores `[0]`;
- dividir os Atributos em exatamente duas linhas: Corpo e Mente;
- listar Perícias em uma única linha sempre que couber;
- listar Poderes em uma única linha sempre que couber;
- usar `Status > nenhum` e `Barreira > nenhuma` quando não houver valores ativos;
- quando houver Status, Barreiras ou outros efeitos ativos relevantes, substituir `nenhum` pelos valores atuais;
- não inserir linhas vazias dentro do HUD;
- não revelar automaticamente informação oculta de adversários.

O HUD é uma interface de decisão, não uma ficha completa. Informações que não ajudam a decisão imediata não precisam ser repetidas.

A forma visual pode seguir `../narracao/` sem transformar apresentação em regra mecânica.

## 2. Declaração humana e configuração

Receber a intenção do JOGADOR HUMANO.

Quando o JOGADOR HUMANO declarar o uso de um Poder, consultar a resolução desse Poder e apresentar seu Hub aplicável antes de resolver o uso, para que o jogador possa ver as opções disponíveis e declarar as escolhas que desejar.

Depois da declaração do jogador, qualquer escolha mecânica que permaneça não declarada — alvo, Alcance, Área, Duração, intensidade, modo, Defesa, Atributo defensivo ou outra configuração aplicável — é completada automaticamente pelo NARRADOR com a **melhor opção válida para realizar a intenção declarada**.

Ao completar automaticamente:

- respeitar todas as escolhas já declaradas pelo JOGADOR HUMANO;
- respeitar limites, custos, alcance, recursos disponíveis e demais regras do Poder;
- usar a melhor opção mecanicamente válida dentro da ação já escolhida;
- não substituir o Poder declarado por outro;
- não trocar a intenção do jogador por uma ação diferente;
- não interromper o fluxo apenas para perguntar uma configuração que possa ser completada dessa forma.

Se a própria intenção estiver indefinida a ponto de não ser possível saber qual ação o jogador deseja realizar, a decisão continua pertencendo ao JOGADOR HUMANO.

> **O jogador escolhe a ação. O sistema completa a mecânica que ele deixou em aberto.**

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

> **HUD → declaração → Hub quando aplicável → completar mecânica omitida → demais declarações → interferência → resolução necessária → atualização → apresentação → novo HUD. `operacao/` determina a ordem; `resolucao/` determina os resultados.**
