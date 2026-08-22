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

`Efeito efetivo = Potência usada + 1 + (Perícia efetiva × 0,2) − Ampliação não paga`

Quando não existe ampliação ou toda a ampliação foi paga em Energia, `Ampliação não paga = 0`.

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

Quando a capacidade usada consome Energia, cada aplicação paga normalmente o custo do patamar efetivamente empregado.

Quando o efeito é ampliado além de sua manifestação-base, a ampliação pode acrescentar custo de Energia.

O NARRADOR apresenta a aplicação de forma compacta:

`custo [patamar usado + carga de ampliação]`

O JOGADOR decide quanto da carga adicional paga em Energia.

Cada ponto de ampliação não pago reduz em `1` o Efeito efetivo daquela aplicação.

Assim, a ampliação pode ser paga integralmente em Energia, integralmente em perda de eficiência ou por uma combinação das duas.

Quando existem várias aplicações:

`Custo efetivo = soma da Energia realmente paga em cada aplicação`

A Resistência também pode elevar o custo indiretamente: ela reduz o progresso por aplicação, exige mais aplicações e abre mais janelas de gasto e reação.

> **Ampliação cobra Energia, eficiência ou ambas. Resistência cobra tempo, custo e oportunidade de reação.**

As faixas e cargas de ampliação pertencem a `consolidacao.md`.

## 6. Oportunidade de reação

Cada aplicação necessária para completar uma disputa cria uma janela temporal real.

Quando a ficção permite perceber a tentativa, personagens e cenário podem agir durante essas janelas.

Uma barreira forte pode não impedir definitivamente um portal, mas pode atrasá-lo o bastante para que seus defensores percebam a pressão, reforcem a proteção, ataquem quem está executando o efeito ou mudem a situação.

A continuidade de uma tentativa nunca suspende a agência dos demais participantes.

> **Quando um efeito precisa acumular progresso, o tempo necessário também cria oportunidade de reação.**

## 7. Consolidação

Consolidação define a escala concreta de uma manifestação depois que a natureza do efeito está estabelecida.

Todo efeito possui uma manifestação mínima de custo `[0]`. Como referência: duração instantânea, um alvo, área/tamanho mínimo coerente e alcance natural da capacidade.

A Consolidação pode ampliar dimensões como:

`Alcance` | `Alvos` | `Área/Tamanho` | `Duração`

As dimensões não são lidas automaticamente pelo mesmo valor. Cada ampliação é escolhida conforme a intenção e a natureza do Poder.

Um Poder não ganha repertório novo por possuir Consolidação suficiente. Telecinese não se transforma em banimento planar apenas porque produziu resultado alto.

Efeitos persistentes permanecem integrais enquanto sua Consolidação restante for maior que zero e sua Duração não tiver terminado.

Reduzir a Consolidação não enfraquece gradualmente as propriedades declaradas. O efeito é rompido quando chega a zero.

A tentativa de remover um efeito antes do fim usa o motor normal: a capacidade de remoção funciona como ataque, a capacidade que sustenta o efeito fornece a resistência coerente e o resultado reduz a Consolidação restante.

> **Duração determina quando o efeito termina sozinho. Consolidação determina quanto trabalho é necessário para rompê-lo antes disso.**

As tabelas e regras operacionais estão em `consolidacao.md`.

## 8. Aplicações

O mesmo motor pode ser usado, quando fizer sentido, para:

- Dano e outras formas de ataque;
- Cura;
- domínio mental;
- maldições;
- imobilização;
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

## 9. Princípios

> **A Exigência determina quanto precisa ser alcançado. A Resistência determina quanto avanço consegue passar por aplicação.**

> **Toda disputa progressiva pergunta quanto o personagem consegue produzir, quanto a situação consegue resistir e quanto precisa ser acumulado para alcançar o objetivo.**

> **Potência determina capacidade. Perícia determina eficiência de aplicação. Resistência determina quanto progresso atravessa. O objetivo determina quanto progresso é necessário.**

> **Uma capacidade inferior pode alcançar um objetivo superior quando a natureza da ação permite acumulação, mas pode pagar por isso em tempo, Energia e exposição.**
