# Ordem Operacional do Combate

Status: APROVADO

Este arquivo define **como aplicar o sistema durante um combate**.

A Rodada, o Turno e a Iniciativa pertencem a `turnos-de-combate.md`. As fórmulas e resultados mecânicos pertencem a `../resolucao/`.

> **Operação organiza a sequência. Resolução calcula. O NARRADOR julga.**

## Escopo exclusivo de combate

A separação por **Rodada, Turno, posição de Iniciativa e vez** pertence somente ao combate ou a outro confronto que esteja explicitamente usando a estrutura de combate.

Fora do combate, não dividir automaticamente a cena em Turnos nem percorrer personagens por Iniciativa.

```text
COMBATE
→ usar Iniciativa
→ usar Rodada
→ usar Turno pessoal
→ processar uma vez por etapa

FORA DE COMBATE
→ usar as janelas normais de cena
→ não criar ordem de Turnos por padrão
```

Quando o confronto deixar de exigir essa estrutura, retornar a `janelas-e-interrupcoes.md`.

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

## Termos operacionais

```text
RODADA
→ ciclo completo da Iniciativa
→ começa no primeiro e termina no último

VEZ
→ momento em que uma peça age em sua posição

TURNO
→ intervalo pessoal de uma peça
→ começa em sua vez atual
→ atravessa o restante da Rodada e o começo da seguinte
→ termina no início de sua próxima vez
```

Exemplo:

```text
Iniciativa
10 → 9 → 8 → 7 → 6

Rodada
10 → 9 → 8 → 7 → 6

Turno da peça na posição 8
8 → 7 → 6 → 10 → 9
→ termina quando a posição 8 chega novamente
```

A cada Rodada, cada participante ativo recebe uma vez. Essa vez inicia um novo Turno pessoal para aquela peça.

## Atalho operacional

```text
início do combate
→ rolar Iniciativa uma vez
→ ordenar participantes
→ iniciar a Rodada
→ chamar a primeira posição
→ ao chegar a vez da peça, encerra seu Turno anterior e começa seu novo Turno
→ persona responsável declara
→ configurar, quando necessário
→ NARRADOR julga
→ resolver ação e Defesa aplicável
→ NARRADOR apresenta o resultado mecânico relevante
→ NARRADOR transforma o resultado em cena
→ registrar estado
→ NARRADOR pergunta se pode prosseguir
→ com autorização, chamar o próximo da Iniciativa
→ ao processar o último, encerrar a Rodada
→ ao voltar ao primeiro, iniciar nova Rodada
```

## 1. Entrada, Iniciativa e interface

Ao entrar em combate:

```text
identificar participantes
→ cada participante rola Iniciativa = 4d6 + Controle uma única vez
→ ordenar do maior para o menor
→ apresentar a ordem
→ iniciar a Rodada pela primeira posição
```

A ordem permanece fixa até o fim do combate conforme `turnos-de-combate.md`.

### JOGADOR HUMANO

Ao chegar a vez do JOGADOR HUMANO, mostrar somente o HUD útil para a decisão de combate:

```text
Nome — Vida atual/máxima | Mana atual/máxima | Trama atual/máxima
POT [X] | CON [X] | RES [X] | INT [X] | PRES [X] | VON [X]
DF [X] | RF [X] | DM [X] | RM [X] | Escudo [X] | RD [X]
Poderes > Poder 1, Poder 2, Poder 3
Status > nenhum
```

Exemplo:

```text
Kael — Vida 20/20 | Mana 18/18 | Trama 30/30
POT [2] | CON [1] | RES [1] | INT [0] | PRES [0] | VON [0]
DF [X] | RF [X] | DM [X] | RM [X] | Escudo [0] | RD [0]
Poderes > Golpe, Proteção
Status > nenhum
```

Regras:

- mostrar sempre os seis Atributos, inclusive `[0]`, em uma única linha compacta;
- usar as abreviações `POT`, `CON`, `RES`, `INT`, `PRES` e `VON` somente como forma de apresentação do HUD;
- mostrar `DF`, `RF`, `DM` e `RM` na terceira linha; suas fórmulas pertencem à resolução e devem ser definidas separadamente;
- mostrar `Escudo` e `RD` na terceira linha, inclusive quando `[0]`;
- não mostrar Perícias no HUD de combate;
- não mostrar uma linha separada de Barreira;
- Poderes permanecem em uma linha sempre que couber;
- usar `Status > nenhum` quando não houver Status relevante;
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

Quando a vez do JOGADOR HUMANO chegar, seu Turno anterior termina e seu novo Turno começa.

```text
1. mostrar HUD
→ 2. receber intenção do jogador
→ 3. configurar o que exigir escolha
→ 4. NARRADOR julga
→ 5. resolver
→ 6. apresentar resultado mecânico relevante
→ 7. narrar a cena resultante
→ 8. registrar
→ 9. perguntar se pode prosseguir
```

Se a intenção estiver indefinida a ponto de não ser possível saber qual ação o jogador deseja realizar, a decisão continua pertencendo ao JOGADOR HUMANO.

### Poderes e Hubs

Quando o JOGADOR HUMANO declarar o uso de um Poder, consultar a resolução desse Poder e **apresentar seu Hub aplicável antes de resolver o uso**.

Depois de apresentar o Hub, aguardar a configuração do jogador.

O NARRADOR não escolhe automaticamente a melhor configuração do Poder e não otimiza Dano, Alcance, Área, Alvos, Duração, Defesa ou qualquer outra progressão do Hub.

O jogador pode declarar somente as alterações que deseja. As opções do Hub que ele não alterar permanecem em suas **posições iniciais**, desde que sejam válidas para a intenção e para a situação.

Ao configurar um Poder:

- respeitar todas as escolhas declaradas pelo JOGADOR HUMANO;
- respeitar `[X]`, custos, alcance, recursos disponíveis e demais regras;
- não aumentar automaticamente opções apenas porque existe Mana disponível;
- não substituir o Poder declarado por outro;
- não trocar a intenção do jogador;
- depois que a configuração estiver válida, não pedir confirmação mecânica adicional desnecessária.

> **Poder declarado → mostrar Hub → jogador escolhe alterações → restante fica na posição inicial.**

## 3. Etapa da vez do JOGADOR IA / JOGADOR IA EVENTUAL

Quando chegar a vez de uma peça sob essas personas, seu Turno anterior termina e seu novo Turno começa.

O fluxo visível ao JOGADOR HUMANO é simples:

```text
1. JOGADOR IA declara a intenção da própria peça
→ 2. NARRADOR apresenta o resultado mecânico relevante
→ 3. NARRADOR transforma o resultado em descrição de cena
→ 4. NARRADOR pergunta se pode prosseguir
```

Exemplo:

```text
[JOGADOR IA — Ravena]
— Eu concentro energia e disparo contra ele.

[NARRADOR]
— Ravena acerta e causa 8 de dano.

[NARRADOR]
— A energia negra se condensa ao redor da mão de Ravena e dispara contra o adversário. O impacto o derruba, deixando-o incapaz de continuar lutando.

[NARRADOR]
— Posso prosseguir?
```

Entre a declaração e o resultado, JOGADOR IA e NARRADOR podem consultar ficha, Poder, Hub, custo, alcance, rolagens, Defesa e demais regras necessárias **sem expor toda essa conversa mecânica na tela**.

Esse processamento interno não altera a autoridade:

```text
JOGADOR IA
→ escolhe intenção, ação, alvo e uso voluntário de capacidades

NARRADOR
→ julga validade
→ aplica mecânica
→ estabelece resultado
```

O NARRADOR não escolhe a ação do aliado.

## 4. Etapa da vez do OPOSITOR

Quando chegar a vez de uma peça adversária, seu Turno anterior termina e seu novo Turno começa.

O OPOSITOR segue o mesmo fluxo usado pelo JOGADOR IA:

```text
1. OPOSITOR declara a intenção da peça adversária
→ 2. NARRADOR apresenta o resultado mecânico relevante
→ 3. NARRADOR transforma o resultado em descrição de cena
→ 4. NARRADOR pergunta se pode prosseguir
```

Exemplo:

```text
[OPOSITOR — Inimigo [1]]
— Eu avanço até Kael e tento golpeá-lo com a lâmina.

[NARRADOR]
— O ataque acerta e causa 5 de dano.

[NARRADOR]
— O inimigo fecha a distância e corta de lado. Kael tenta sair da trajetória, mas a lâmina alcança seu flanco antes que ele consiga escapar completamente.

[NARRADOR]
— Posso prosseguir?
```

A configuração mecânica pode acontecer internamente entre OPOSITOR e NARRADOR, sem revelar ao JOGADOR HUMANO Hub completo, estratégia reservada ou detalhes que não sejam observáveis.

O OPOSITOR escolhe a jogada. O NARRADOR apenas julga e resolve.

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

## 8. Apresentar resultado e narrar a cena

Depois do julgamento e da resolução, o NARRADOR apresenta primeiro o resultado mecânico necessário para compreensão da mesa e depois o converte em ficção.

Formato preferido:

```text
RESULTADO MECÂNICO
→ curto e objetivo
→ ataque, Defesa, Dano, efeito ou mudança de estado relevante

DESCRIÇÃO DA CENA
→ traduz o resultado em ação observável
→ não altera o resultado mecânico
```

Para JOGADOR IA e OPOSITOR, não mostrar por padrão toda a conta interna, Hub, escolha de modificadores ou diálogo técnico usado para chegar ao resultado.

Mostrar ao JOGADOR HUMANO somente:

- declaração visível da persona responsável;
- resultado mecânico relevante;
- aquilo que a ficção torna observável;
- mudança de estado necessária para a próxima decisão.

A forma narrativa pertence a `../narracao/`.

## 9. Registrar e pausar

Depois de narrar a cena:

```text
registrar o novo estado
→ não chamar automaticamente a próxima posição
→ perguntar ao JOGADOR HUMANO se pode prosseguir
```

Forma operacional simples:

> **Posso prosseguir?**

Somente depois da autorização o fluxo avança para a próxima posição da Iniciativa.

Essa autorização controla o avanço da mesa; ela não transforma o JOGADOR HUMANO em controlador das outras personas.

## 10. Fechamento da Rodada

A Rodada termina somente quando a última posição da Iniciativa foi processada.

```text
há posição ainda não processada
→ após autorização, chamar o próximo

última posição processada
→ encerrar a Rodada
→ perguntar se pode prosseguir
→ ao voltar ao primeiro, iniciar nova Rodada
```

O fechamento da Rodada **não encerra automaticamente o Turno pessoal de todas as peças**. Cada Turno termina apenas quando chega novamente a vez da própria peça.

Se o confronto deixar de exigir acompanhamento em segundos, retornar a `janelas-e-interrupcoes.md`.

## Regra final

> **Esta estrutura pertence ao combate. A Rodada percorre toda a Iniciativa, do primeiro ao último. O Turno é pessoal: começa na vez de uma peça e termina no início da próxima vez dessa mesma peça, podendo atravessar o fim da Rodada. A persona responsável declara; o NARRADOR julga e resolve. Para JOGADOR IA e OPOSITOR, a mecânica intermediária pode permanecer interna: na tela aparecem a declaração, o resultado mecânico relevante, a descrição da cena e a pergunta para prosseguir. Fora do combate, usar as janelas normais de cena.**