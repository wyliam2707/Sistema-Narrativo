# Ordem Operacional do Combate

Status: APROVADO

Este arquivo define **como aplicar o sistema durante um combate**.

O Turno e a Iniciativa pertencem a `turnos-de-combate.md`. As fórmulas e resultados mecânicos pertencem a `../resolucao/`.

> **Operação organiza a sequência. Resolução calcula. O NARRADOR julga.**

## Princípio de autoridade

Durante combate, o NARRADOR continua sendo somente o **juiz da mesa**.

```text
JOGADOR HUMANO
→ controla o próprio personagem

JOGADOR IA / JOGADOR IA EVENTUAL
→ controla aliados ou NPCs delegados

OPOSITOR
→ controla inimigos e forças adversárias válidas

NARRADOR
→ JULGA
→ NARRA A SENTENÇA
→ REGISTRA
```

O NARRADOR não escolhe ações voluntárias para nenhuma dessas peças.

> **Quem controla a peça declara. O NARRADOR julga o que foi declarado.**

## Atalho operacional

```text
início do combate
→ rolar Iniciativa uma vez
→ ordenar participantes
→ iniciar o Turno
→ chamar a vez atual
→ persona responsável declara
→ configurar, quando necessário
→ NARRADOR julga
→ resolver ação e Defesa aplicável
→ NARRADOR narra a sentença
→ registrar estado
→ NARRADOR pergunta se pode prosseguir
→ com autorização, chamar o próximo da Iniciativa
→ ao processar o último, encerrar o Turno
→ ao voltar ao primeiro, iniciar novo Turno
```

## 1. Entrada, Iniciativa e interface

Ao entrar em combate:

```text
identificar participantes
→ cada participante rola Iniciativa = 4d6 + Controle uma única vez
→ ordenar do maior para o menor
→ apresentar a ordem
→ iniciar o Turno pela primeira posição
```

A ordem permanece fixa até o fim do combate conforme `turnos-de-combate.md`.

### JOGADOR HUMANO

Ao chegar a vez do JOGADOR HUMANO, mostrar o HUD completo necessário para decisão:

```text
Nome — Vida atual/máxima | Mana atual/máxima | Trama, quando aplicável
Potência [X] · Controle [X] · Resistência [X]
Intelecto [X] · Presença [X] · Vontade [X]
Perícias > Perícia 1, Perícia 2, Perícia 3
Poderes > Poder 1, Poder 2, Poder 3
Status > nenhum
Barreira > nenhuma
```

Regras:

- mostrar sempre os seis Atributos, inclusive `[0]`;
- exatamente duas linhas de Atributos;
- Perícias em uma linha sempre que couber;
- Poderes em uma linha sempre que couber;
- `Status > nenhum` e `Barreira > nenhuma` quando vazios;
- não inserir linhas vazias dentro do HUD.

### Peças controladas por IA ou OPOSITOR

Quando chegar a vez de uma peça controlada por JOGADOR IA, JOGADOR IA EVENTUAL ou OPOSITOR, não é necessário exibir ao humano uma interface completa de decisão da peça.

Quando for útil mostrar seu estado observável, usar apresentação compacta:

```text
Aliado [1] — Vida [X/X] | Mana [X/X]
Status > nenhum
```

ou:

```text
Inimigo [1] — Vida [X/X] | Mana [X/X]
Status > nenhum
```

A persona responsável pode consultar internamente a ficha e as regras necessárias sem exigir do JOGADOR HUMANO um Hub de memória equivalente ao HUD humano.

Informação realmente oculta continua oculta, salvo regra da campanha que determine exposição diferente.

## 2. Etapa da vez do JOGADOR HUMANO

Quando a vez do JOGADOR HUMANO chegar:

```text
1. mostrar HUD
→ 2. receber intenção do jogador
→ 3. configurar o que exigir escolha
→ 4. NARRADOR julga
→ 5. resolver
→ 6. narrar sentença
→ 7. registrar
→ 8. perguntar se pode prosseguir
```

Se a intenção estiver indefinida a ponto de não ser possível saber qual ação o jogador deseja realizar, a decisão continua pertencendo ao JOGADOR HUMANO.

### Poderes e Hubs

Quando o JOGADOR HUMANO declarar o uso de um Poder, consultar a resolução desse Poder e **apresentar seu Hub aplicável antes de resolver o uso**.

Depois de apresentar o Hub, aguardar a configuração do jogador.

O NARRADOR não escolhe automaticamente a melhor configuração do Poder e não otimiza Dano, Alcance, Área, Alvos, Duração, Defesa ou qualquer outra progressão do Hub.

O jogador pode declarar somente as alterações que deseja. As opções do Hub que ele não alterar permanecem em suas **posições iniciais**, desde que sejam válidas para a intenção e a situação.

Ao configurar um Poder:

- respeitar todas as escolhas declaradas pelo JOGADOR HUMANO;
- respeitar `[X]`, custos, alcance, recursos disponíveis e demais regras;
- não aumentar automaticamente opções apenas porque existe Mana disponível;
- não substituir o Poder declarado por outro;
- não trocar a intenção do jogador;
- depois que a configuração estiver válida, não pedir confirmação mecânica adicional desnecessária.

> **Poder declarado → mostrar Hub → jogador escolhe alterações → restante fica na posição inicial.**

## 3. Etapa da vez do JOGADOR IA / JOGADOR IA EVENTUAL

Quando chegar a vez de uma peça sob essas personas:

```text
1. persona responsável escolhe a ação do aliado/NPC
→ 2. configura internamente o necessário
→ 3. NARRADOR julga
→ 4. resolve
→ 5. narra a sentença
→ 6. registra
→ 7. pergunta se pode prosseguir
```

O NARRADOR não escolhe a ação do aliado.

Não é necessário mostrar ao JOGADOR HUMANO o Hub completo usado pela IA apenas para lembrar opções. A IA consulta diretamente a ficha e as regras.

## 4. Etapa da vez do OPOSITOR

Quando chegar a vez de uma peça adversária:

```text
1. OPOSITOR escolhe a ação do inimigo
→ 2. configura internamente o necessário
→ 3. NARRADOR julga validade, meios e oportunidade
→ 4. resolve
→ 5. narra somente o que é observável
→ 6. registra
→ 7. pergunta se pode prosseguir
```

O NARRADOR não escolhe a ação do inimigo.

Configurações, intenções ou informação reservada do OPOSITOR não precisam ser expostas automaticamente ao JOGADOR HUMANO.

## 5. Defesa automática

Quando o JOGADOR HUMANO for alvo de uma ação que permita Defesa, o NARRADOR usa automaticamente a **melhor opção defensiva válida e coerente já disponível naquele instante**.

Isso faz parte do julgamento mecânico da ação recebida e não transfere ao NARRADOR autoridade para criar uma nova vontade do personagem.

Pode usar automaticamente:

- o Atributo defensivo mais favorável entre os que a ficção realmente permite;
- a forma de defesa mecanicamente mais vantajosa já disponível;
- bônus defensivos, Status, Barreiras, Poderes já ativos ou outras fontes automáticas aplicáveis.

Não pode:

- ativar um novo Poder defensivo por decisão própria;
- gastar recurso opcional quando houver escolha estratégica real;
- inventar reação que não esteja disponível.

A Defesa ocorre no momento da ação que a provocou e **não consome a vez de Iniciativa** do defensor.

> **Se a defesa já é possível, use a melhor. Se exige uma nova escolha, não invente a escolha.**

## 6. Julgamento

Depois que a persona responsável declarar e configurar sua ação, o NARRADOR julga.

Pode verificar somente o necessário:

```text
fatos estabelecidos
regras aplicáveis
ficha
estado atual
conhecimento da peça
meios
alcance
recursos
oportunidade
incerteza real
```

O NARRADOR não modifica a intenção para produzir uma cena melhor e não cria uma nova ação para nenhuma peça.

Se houver incerteza real, aplica a resolução correspondente.

## 7. Resolução e atualização

Para a ação da vez atual:

```text
pagar custo válido, quando houver
→ resolver CD ou oposição quando necessário
→ aplicar Defesa
→ aplicar Dano/Efeito/Status conforme a regra específica
→ estabelecer consequência
→ atualizar o estado imediatamente
```

Fontes principais:

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

Assim que a consequência for estabelecida, atualizar o estado antes de qualquer posição posterior.

> **Resolveu → atualizou.**

## 8. Narrar a sentença

Depois do julgamento e da resolução, o NARRADOR apresenta o resultado.

Mostrar ao JOGADOR HUMANO somente:

- consequência mecânica relevante;
- aquilo que a ficção torna observável;
- mudança de estado necessária para a próxima decisão.

Por padrão, usar apresentação compacta sem toda a conta intermediária.

A forma narrativa pertence a `../narracao/`.

## 9. Registrar e pausar

Depois de narrar a sentença:

```text
registrar o novo estado
→ não chamar automaticamente a próxima posição
→ perguntar ao JOGADOR HUMANO se pode prosseguir
```

Forma operacional simples:

> **Posso prosseguir?**

Somente depois da autorização o fluxo avança para a próxima posição da Iniciativa.

Essa autorização controla o avanço da mesa; ela não transforma o JOGADOR HUMANO em controlador das outras personas.

## 10. Fechamento do Turno

O Turno termina somente quando a última posição da Iniciativa foi processada.

```text
há posição ainda não processada
→ após autorização, chamar o próximo

última posição processada
→ encerrar o Turno
→ perguntar se pode prosseguir
→ ao voltar ao primeiro, iniciar novo Turno
```

Se o confronto deixar de exigir acompanhamento em segundos, retornar a `janelas-e-interrupcoes.md`.

## Regra final

> **Combate é executado em etapas. A Iniciativa determina de quem é a vez; a persona responsável controla a peça; o NARRADOR apenas julga, narra a sentença e registra. Depois de cada vez, o NARRADOR pausa e pergunta se pode prosseguir. O último da Iniciativa encerra o Turno; voltar ao primeiro inicia o Turno seguinte.**