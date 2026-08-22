# Motor geral de disputa

Status: APROVADO

Este arquivo define o motor geral usado quando existe uma disputa real e o resultado pode avançar progressivamente contra uma resistência, uma exigência ou ambas.

Ele pode resolver disputas contra outros personagens e contra o cenário.

Não substitui o princípio geral da resolução:

`Resultado evidente → estabelece` | `Impossibilidade evidente → estabelece` | `Incerteza real → resolve`

O motor progressivo só entra quando a situação realmente pede progresso, resistência, tempo, custo ou oportunidade de reação.

> **O motor existe para disputas progressivas, não para transformar toda ação em cálculo.**

## 1. Estrutura geral

A resolução separa quatro perguntas:

`Potência → quanto o personagem consegue produzir` | `Resistência → quanto consegue impedir por aplicação` | `Exigência → quanto precisa ser alcançado` | `Aplicação → quanto tempo cada tentativa representa`

Quando houver Perícias realmente aplicáveis dos dois lados:

`Perícia efetiva = Perícia de aplicação − Perícia de oposição`

Quando não houver Perícia defensiva ou oposição técnica real, considera-se apenas a Perícia aplicável de quem executa.

O efeito efetivo é:

`Efeito efetivo = Potência usada + 1 + (Perícia efetiva × 0,2)`

O progresso produzido por aplicação é:

`Progresso por aplicação = 2^(Efeito efetivo − Resistência efetiva)`

A Potência pode vir de um Poder, Atributo ou outra capacidade que a cena estabeleça como responsável pelo efeito.

A Resistência pode vir de um personagem, estrutura, barreira, proteção, sistema, ambiente ou qualquer outro elemento que realmente se oponha ao efeito.

A cena continua decidindo quais capacidades entram na resolução. Valores não são somados apenas por existirem na ficha.

## 2. Exigência do objetivo

A Exigência representa quanto progresso precisa ser alcançado para cumprir exatamente o objetivo declarado.

Objetivos diferentes podem exigir profundidades diferentes mesmo quando usam a mesma capacidade.

O personagem não precisa alcançar o efeito máximo possível se sua intenção exige menos.

> **O jogador declara o objetivo. A resolução determina quanto precisa ser alcançado para realizá-lo.**

Exemplo conceitual: uma influência forte pode exigir muito menos progresso do que controle mental absoluto.

A Exigência pode vir da profundidade do efeito, resistência do cenário, dificuldade da alteração ou outra propriedade relevante.

Alcance, quantidade de alvos, área/tamanho e duração são tratados pelas regras de Consolidação em `consolidacao.md`.

## 3. Progresso acumulado

Se uma aplicação não alcança a Exigência e a natureza da ação permite continuidade, o progresso pode permanecer acumulado.

`Aplicações necessárias = teto(Exigência ÷ Progresso por aplicação)`

Uma capacidade inferior não é automaticamente proibida de tentar um objetivo maior. Ela pode precisar de mais aplicações, desde que a ficção permita acumulação e o personagem consiga sustentar o custo e o tempo necessários.

> **Patamar maior não precisa significar fazer outra coisa. Pode significar fazer a mesma coisa mais rápido, com menos exposição e com maior capacidade de consolidação.**

Quando a própria natureza do efeito não permite progresso acumulado, esta regra não cria acumulação artificial.

## 4. Tempo por aplicação

A unidade de tempo pertence à natureza da tarefa, não à cena em que ela acontece.

Escalas padrão:

`6 segundos → aplicação imediata` | `1 minuto → aplicação curta` | `1 hora → aplicação prolongada` | `1 dia → aplicação extensa`

Uma ação de combate, uma maldição rápida ou uma pressão mental podem usar `6 segundos` por aplicação.

Um hackeamento comum, ritual curto ou preparação semelhante pode usar `1 minuto` por aplicação.

Uma cirurgia, fabricação ou trabalho técnico prolongado pode usar `1 hora` por aplicação.

Pesquisa extensa, construção, encantamento ou projetos equivalentes podem usar `1 dia` por aplicação.

A natureza concreta da atividade pode justificar outra escala, mas entrar em combate não acelera uma tarefa naturalmente lenta.

`Tempo efetivo = número de aplicações × tempo por aplicação`

> **A tarefa define a escala de tempo da aplicação. A disputa define quantas aplicações são necessárias.**

## 5. Custo efetivo e ampliação

Quando a capacidade usada consome Energia, cada aplicação paga normalmente o custo da configuração escolhida.

`Custo = patamar efetivamente usado + Ampliação usada`

Não existe pagamento parcial de Ampliação. Se o JOGADOR não dispõe da Energia necessária ou quer gastar menos, escolhe antes da resolução um patamar menor, menos Ampliação ou ambos.

Quando existem várias aplicações:

`Custo efetivo = soma da Energia paga em cada aplicação`

A Resistência também pode elevar o custo indiretamente: ela reduz o progresso por aplicação, exige mais aplicações e abre mais janelas de gasto e reação.

> **Potência e Ampliação são escolhas separadas. Energia paga exatamente a configuração escolhida. Resistência pode cobrar tempo, custo e oportunidade de reação.**

As faixas, cargas e limite de Ampliação pertencem a `consolidacao.md`.

## 6. Oportunidade de reação

Cada aplicação necessária para completar uma disputa cria uma janela temporal real.

Quando a ficção permite perceber a tentativa, personagens e cenário podem agir durante essas janelas.

Uma barreira forte pode não impedir definitivamente um portal, mas pode atrasá-lo o bastante para que seus defensores percebam a pressão, reforcem a proteção, ataquem quem está executando o efeito ou mudem a situação.

A continuidade de uma tentativa nunca suspende a agência dos demais participantes.

> **Quando um efeito precisa acumular progresso, o tempo necessário também cria oportunidade de reação.**

## 7. Contenção sustentada por agentes

Uma contenção realizada diretamente por um personagem, criatura ou Invocação ativa não cria automaticamente uma estrutura persistente `D/V`. Ela existe porque o agente continua sustentando a ação.

A tentativa usa o motor normal. O agente escolhe um mecanismo coerente, normalmente um Atributo e eventualmente uma Perícia aplicável, e o alvo reage pelo eixo realmente disponível na situação.

Em uma disputa corporal direta, `FIS` normalmente responde pelo mecanismo físico dos dois lados.

Exemplo sem Perícias: `FIS [2] → Efetivo 3` contra `FIS [2] → Resultado 2`.

O Resultado é lido pela escala aplicável de Mobilidade:

`[2] Dificultar` | `[4] Restringir` | `[8] Imobilizar` | `[16] Conter` | `[32] Aprisionar`

Assim, `FIS [2]` contra `FIS [2]` produz normalmente `Resultado 2`: uma contenção inicial, agarrão ou dificuldade relevante, não Imobilização completa.

A condição é registrada como **Sustentada**, porque depende da ação contínua de quem segura.

Exemplo: `Agarrado [2] — Sustentado pelo Guarda`.

Estar agarrado não apaga automaticamente todas as ações dos envolvidos. Ambos continuam podendo realizar ações coerentes com a posição: atacar com o corpo, tentar escapar, mudar a posição, usar uma capacidade acessível ou lançar um efeito que a situação realmente permita.

O personagem preso também pode escolher atacar quem o segura em vez de tentar escapar. Nesse caso, ele gasta sua ação no ataque; não recebe uma tentativa gratuita de fuga na mesma ação.

### Manutenção

Sustentar a contenção consome a ação do agente na nova janela. A cada ação de manutenção existe nova resolução conforme a situação atual.

Se quem sustenta solta, é incapacitado, muda de ação ou deixa de conseguir manter o mecanismo, a contenção sustentada termina ou precisa ser novamente estabelecida.

Escapar de uma contenção sustentada não destrói o agente que a produziu. O agente continua existindo e pode tentar conter novamente em uma janela posterior.

### Vários agentes

Quando vários agentes coordenam contenções compatíveis contra o mesmo alvo na mesma janela, **não se somam os Atributos**.

Cada agente resolve sua própria aplicação contra a defesa coerente do alvo. Depois, os Resultados compatíveis são somados para determinar a contenção conjunta daquela janela.

Exemplo: quatro guardas com `FIS [2]` enfrentam um alvo com `FIS [2]`. Cada aplicação produz `Resultado 2`.

`2 + 2 + 2 + 2 = 8 → Imobilizado [8] — Sustentado pelos 4 guardas`

Na janela seguinte entram apenas os agentes que continuam gastando sua ação para sustentar a contenção.

> **Agentes não somam Atributos. Ações coordenadas podem somar Resultados quando produzem a mesma consequência na mesma janela.**

### Passagem para uma contenção física

Uma contenção sustentada pode criar a condição necessária para aplicar uma estrutura física de prisão.

Se o alvo já está funcionalmente Imobilizado e nada adicional impede a aplicação, colocar algemas, cordas ou outro dispositivo adequado pode ser um resultado evidente em vez de exigir nova disputa artificial.

Depois que a estrutura física está aplicada, os agentes podem deixar de sustentar o agarrão. A prisão passa a depender do objeto.

Uma estrutura desse tipo pode usar a lógica estrutural de Invocação. Exemplo: `Algemas → FIS [3] | V10`.

`FIS [3]` representa o mecanismo físico de contenção quando alguém tenta vencê-lo corporalmente. `V10` representa a Vida estrutural do objeto. Outras formas de escapar ou atacar a estrutura usam o mecanismo e a defesa que realmente forem aplicáveis.

> **Agarrão é uma disputa sustentada entre agentes. Algemas são uma estrutura física que continua existindo depois que os agentes soltam.**

## 8. Consolidação

Consolidação define a escala concreta de uma manifestação depois que a natureza do efeito está estabelecida.

Todo efeito possui uma manifestação mínima de custo `[0]`. Como referência: duração instantânea, um alvo, área/tamanho mínimo coerente e alcance natural da capacidade.

A Consolidação pode ampliar dimensões como:

`Alcance` | `Alvos` | `Área/Tamanho` | `Duração`

As dimensões não são lidas automaticamente pelo mesmo valor. Cada ampliação é escolhida conforme a intenção e a natureza do Poder.

Um Poder não ganha repertório novo por possuir Consolidação suficiente. Telecinese não se transforma em banimento planar apenas porque produziu resultado alto.

Quando um efeito permanece depois da aplicação, ele possui sua estrutura persistente própria:

`Efeito [D x / V5] — Duração`

`D` é a Defesa estrutural estabelecida para o efeito e `V5` é sua Vida padrão. Perder Vida não reduz gradualmente a intensidade do efeito; enquanto `V > 0`, ele continua produzindo o Resultado já estabelecido. Em `V0`, termina.

A remoção por Dissipar usa o motor normal de ataque e dano contra essa estrutura:

`Dissipar efetivo vs D do efeito → Dano aplicado → reduz V`

A duração continua determinando quando o efeito termina naturalmente.

> **Duração determina quando o efeito termina sozinho. D/V determina sua estrutura enquanto permanece.**

As tabelas e regras operacionais estão em `consolidacao.md` e `escalas-de-efeito.md`.

## 9. Aplicações

O mesmo motor pode ser usado, quando fizer sentido, para:

- Dano e outras formas de ataque;
- Cura;
- domínio mental;
- maldições;
- imobilização;
- contenção sustentada;
- teleporte e portais;
- rompimento de barreiras;
- hackeamento;
- arrombamento;
- fabricação;
- pesquisa;
- rituais;
- construção;
- outras disputas contra personagens ou cenário.

Cada aplicação interpreta Potência, Resistência, Exigência, Consolidação e tempo de acordo com sua própria natureza.

Dano é uma aplicação especializada deste motor, não a definição de todas as demais.

## 10. Princípios

> **A Exigência determina quanto precisa ser alcançado. A Resistência determina quanto avanço consegue passar por aplicação.**

> **Toda disputa progressiva pergunta quanto o personagem consegue produzir, quanto a situação consegue resistir e quanto precisa ser acumulado para alcançar o objetivo.**

> **Potência determina capacidade. Perícia determina eficiência de aplicação. Resistência determina quanto progresso atravessa. O objetivo determina quanto progresso é necessário.**

> **Uma capacidade inferior pode alcançar um objetivo superior quando a natureza da ação permite acumulação, mas pode pagar por isso em tempo, Energia e exposição.**

> **Efeito persistente cria estrutura. Contenção por agente precisa ser sustentada. Estrutura física continua existindo por conta própria.**
