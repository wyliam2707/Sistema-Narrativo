# Ordem Operacional do Combate

Status: APROVADO

Este arquivo define **como aplicar o sistema durante um combate**.

A rodada e a Iniciativa pertencem a `turnos-de-combate.md`. As fórmulas e resultados mecânicos pertencem a `../resolucao/`.

> **Operação organiza a sequência. Resolução calcula.**

## Atalho operacional

```text
início do combate
→ rolar Iniciativa
→ ordenar participantes
→ chamar o primeiro
→ declaração da peça ativa
→ apresentar Hub e aguardar configuração, quando o JOGADOR HUMANO declarar um Poder
→ resolver ação e Defesa aplicável
→ atualizar estado
→ apresentar resultado
→ chamar o próximo da Iniciativa
→ ao terminar a ordem, iniciar nova rodada
```

## 1. Entrada, Iniciativa e HUD

Ao entrar em combate:

```text
identificar participantes
→ rolar Iniciativa = 4d6 + Controle
→ ordenar do maior para o menor
→ apresentar a ordem
→ iniciar a primeira posição
```

A ordem permanece conforme `turnos-de-combate.md`.

Ao chegar a posição do JOGADOR HUMANO, mostrar um HUD discreto apenas com informação necessária para decidir.

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
- dividir os Atributos em exatamente duas linhas;
- listar Perícias em uma única linha sempre que couber;
- listar Poderes em uma única linha sempre que couber;
- usar `Status > nenhum` e `Barreira > nenhuma` quando não houver valores ativos;
- substituir `nenhum` pelos valores atuais quando houver Status ou Barreiras;
- não inserir linhas vazias dentro do HUD;
- não revelar automaticamente informação oculta de adversários.

A ordem de Iniciativa pode ser mostrada separadamente do HUD e não precisa ser repetida a cada posição se não tiver mudado.

## 2. Posição do JOGADOR HUMANO

Quando a posição do JOGADOR HUMANO chegar, receber sua intenção.

Se a própria intenção estiver indefinida a ponto de não ser possível saber qual ação ele deseja realizar, a decisão continua pertencendo ao jogador.

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
- depois que a configuração estiver válida, não pedir confirmação adicional.

> **Poder declarado → mostrar Hub → jogador escolhe alterações → restante fica na posição inicial.**

## 3. Defesa automática

Quando o JOGADOR HUMANO for alvo de uma ação que permita Defesa, o NARRADOR usa automaticamente a **melhor opção defensiva válida e coerente** disponível naquele instante.

Isso inclui, sem interromper o fluxo:

- o Atributo defensivo mais favorável entre os que a ficção realmente permite;
- a forma de defesa mecanicamente mais vantajosa já disponível;
- bônus defensivos, Status, Barreiras, Poderes já ativos ou outras fontes automáticas aplicáveis.

Essa regra não autoriza:

- ativar um novo Poder defensivo por decisão própria;
- gastar recurso opcional quando houver escolha estratégica real;
- inventar uma reação que não esteja disponível.

Nesses casos, a decisão continua pertencendo ao JOGADOR HUMANO.

A Defesa ocorre no momento da ação que a provocou e **não consome a posição de Iniciativa** do defensor.

> **Se a defesa já é possível, use a melhor. Se exige uma nova escolha, não invente a escolha.**

## 4. Posições das demais personas

Quando chegar a posição de uma peça controlada por JOGADOR IA, JOGADOR IA EVENTUAL, OPOSITOR ou outra persona aplicável:

```text
persona declara/processa a intenção da peça
→ configura opções ocultas quando necessário
→ NARRADOR resolve
→ aplica consequências
→ atualiza estado
→ segue para o próximo da Iniciativa
```

Configurações ocultas de adversários não são expostas automaticamente ao jogador.

A ordem de autoridade das personas continua pertencendo a `../personas/`; a Iniciativa determina apenas **quando a peça age no combate**.

## 5. Aplicar a resolução necessária

Para cada ação da posição atual:

```text
configurar o uso, quando necessário
→ pagar custo válido
→ resolver CD ou oposição somente se houver incerteza
→ aplicar Defesa
→ aplicar Dano/Efeito/Status conforme a regra específica
→ estabelecer consequência
→ atualizar estado
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

Assim que uma consequência for estabelecida, atualizar o estado **antes de chamar a próxima posição de Iniciativa**.

Isso pode alterar:

- Vida;
- Mana;
- Trama;
- Status;
- Barreiras;
- posição;
- alterações temporárias de Atributo;
- possibilidade de agir quando a posição futura chegar.

Se uma peça ficar incapaz de agir antes de sua vez, quando sua posição chegar usar o estado atual e encerrar a posição sem uma ação voluntária, salvo regra específica.

> **Resolveu → atualizou → próximo da Iniciativa.**

## 7. Apresentação

Mostrar ao JOGADOR HUMANO apenas resultados mecânicos relevantes à decisão e aquilo que a ficção torna observável.

Por padrão, mostrar o resultado de forma compacta, sem toda a conta intermediária.

A forma narrativa pertence a `../narracao/`.

## 8. Fechamento da rodada

A rodada só termina quando todas as posições aplicáveis da ordem de Iniciativa forem processadas.

```text
há participante ativo ainda não processado
→ chamar o próximo

última posição processada
→ fechar a rodada
→ iniciar nova rodada, se o combate continuar
```

Antes da nova rodada, `../persistencia/` deve refletir o estado já estabelecido.

Se o confronto deixar de exigir acompanhamento em segundos, retornar a `janelas-e-interrupcoes.md`.

## Regra final

> **Iniciativa → peça ativa → declaração → Hub quando aplicável → resolução e Defesa → atualização imediata → próximo da Iniciativa. Poder do jogador sempre abre o Hub; Defesa já disponível é automática; nenhuma peça ativa deve ser esquecida antes do fim da rodada.**
