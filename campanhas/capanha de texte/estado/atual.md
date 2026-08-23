# Estado atual

Campanha iniciada.

## Situação atual

Capítulo 002 em andamento.

Durante a tarde, Corvin permaneceu na biblioteca estudando Magia da Ordem até o jantar. Wanda treinou de forma controlada e depois se preparou para a reunião com Tony Stark do dia seguinte. Ravena manteve a tarde tranquila, meditando, lendo e verificando assuntos dos Titãs sem compromisso imediato.

Depois do jantar, Corvin avisou Wanda e Ravena que sairia brevemente para uma negociação de rotina com um informante antigo: faria uma entrega e receberia um livro antigo sobre um culto de Tiamat, descrita por ele como uma criatura semelhante a um dragão de dez cabeças. Corvin deixou claro que o assunto não era relacionado a Trigon e que nem sabia ainda se Tiamat era real.

Corvin informou que teleportaria sozinho para Ganadex, na Índia, encontraria o ponto de entrega e retornaria em uma ou duas horas. Wanda e Ravena permaneceram em casa.

## Cena atual

Corvin chegou sozinho a Ganadex e encontrou o ponto combinado para a troca nos fundos de uma construção comercial fechada. O informante ainda não apareceu.

Dois homens surgiram no corredor. Um deles possui uma lâmina ritual escura; o outro iniciou um gesto ritual. Eles reconheceram Corvin pelo nome e exigiram aquilo que, segundo eles, pertence à "Mãe das Dez Gargantas".

A situação passou para confronto ativo e o combate foi declarado iniciado.

### Resultado do teste de combate

O combate foi executado até o encerramento usando o fluxo revisado de HUD, confirmação das escolhas do JOGADOR HUMANO, processamento interno das IAs/OPOSITOR, resolução por turno e exibição discreta dos resultados mecânicos.

Corvin iniciou com `VIDA [35/35] | ENERGIA [80/80]`.

Ele consolidou uma Proteção [3] em si mesmo, depois uma Contenção [3] contra o cultista da lâmina, usou Dano [3] contra o cultista ritualista e, por fim, aplicou Sono [3] ampliado de Cena para Dia no cultista contido.

Estado final do combate:

```text
Corvin: VIDA [35/35] | ENERGIA [66/80]
Proteção: [D3,8 / V2,06] — Cena
Cultista ritualista: incapacitado, inconsciente — VIDA [0/15]
Cultista da lâmina: adormecido — Sono [3] — Dia
```

O combate terminou sem Dano sofrido por Corvin.

## Observações do teste

O teste confirmou o seguinte fluxo operacional:

```text
HUD → declaração humana → confirmação mecânica, se necessária → IAs/Opositor → resolver → atualizar estado → novo HUD
```

Toda informação puramente mecânica deve aparecer de forma visualmente discreta, em bloco destacado/itálico, mostrando preferencialmente o resultado e não o cálculo intermediário.

Ao iniciar combate e no início de cada nova ação humana, o HUD deve apresentar:

```text
Nome — VIDA | ENERGIA | efeitos benéficos
Atributos
Perícias relevantes
Um Poder por linha
Status [+]
Status [-]
```

Escolhas mecânicas do JOGADOR HUMANO não devem ser tomadas silenciosamente pelo NARRADOR. Se uma declaração já vier completa e válida, apenas confirmar quando necessário. Se houver alcance, ampliação, custo ou outra configuração insuficiente, recomendar uma alternativa sem escolhê-la automaticamente.

JOGADORES IA e NPCs fazem suas configurações equivalentes fora da tela.

O combate usa turnos simultâneos de até 10 segundos enquanto o confronto estiver ativo.