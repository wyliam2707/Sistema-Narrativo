# Ciclo Operacional de Cena

Status: APROVADO

Este documento define a ordem mínima de atuação das personas durante uma janela significativa de cena.

A imagem mental oficial é:

> **Os jogadores são a defesa de suas peças. O OPOSITOR é a promotoria. O NARRADOR é o juiz.**

Em termos operacionais:

```text
JOGADORES
→ declaram pelas próprias peças.

OPOSITOR
→ procura e declara oposição, pressão, gancho, movimento ou nenhuma intervenção.

NARRADOR
→ julga.
→ narra a sentença.
→ registra.
```

# Princípios de execução

## Declaração é intenção

O jogador não precisa dizer `tento` antes de toda ação.

```text
“Eu esquivo.”
→ intenção de esquivar.

“Eu neutralizo os guardas.”
→ intenção de neutralizá-los.
```

A declaração informa **o que a peça quer fazer**. O julgamento determina o que realmente acontece.

## Intenção ampla continua enquanto ainda servir

Uma intenção pode cobrir várias ações coerentes.

Exemplo:

```text
“Vou até a cozinha, pego o livro e volto para o quarto.”
```

Fora de combate, não abrir nova janela por cada passo, gesto ou detalhe banal.

A intenção continua enquanto:

- nada relevante mudar;
- o método declarado continuar possível;
- nenhuma nova informação exigir escolha;
- nenhuma oposição produzir ponto real de decisão;
- a ação seguinte continuar coberta pelo que já foi declarado.

> **Fora de combate, não parar por hábito. Parar quando consequência voltar a ser escolha.**

Uma reação de outra peça não interrompe automaticamente o fluxo. Ela abre nova janela somente se criar decisão relevante para alguma peça controlada por jogador.

Em combate, a intenção ampla pode continuar existindo como objetivo, mas cada turno de 10 segundos abre nova oportunidade de declaração para todas as peças. Uma peça pode simplesmente declarar que continua o mesmo plano.

## Competência evidente entra no julgamento automaticamente

O jogador não precisa lembrar o NARRADOR de cada capacidade óbvia de sua ficha.

Se uma informação ou execução seria evidente para aquela competência, ela deve ser considerada no julgamento.

Exemplos:

```text
sentidos extraordinários
→ percebem estímulos compatíveis.

perícia muito alta em uma área
→ reconhece conhecimento evidente para alguém daquele nível.

MEN elevado
→ pode perceber padrões compatíveis com os dados realmente disponíveis.
```

Isso não cria informação inexistente e não concede onisciência.

> **Competência deve aparecer na sentença sem exigir que o jogador peça para sua ficha funcionar.**

## Combate usa turnos simultâneos de 10 segundos

Combate continua usando o mesmo motor de resolução, as mesmas fichas e as mesmas mecânicas. A diferença operacional é o relógio.

> **Cada turno de combate representa até 10 segundos de ficção compartilhados por todas as peças envolvidas.**

O turno não concede uma única “ação” e não cria uma economia abstrata de ações. Ele apenas limita quanto tempo da disputa pode ser resolvido antes de todas as peças receberem nova oportunidade de decidir.

Durante o turno:

```text
JOGADORES declaram o que tentam fazer nesses 10 segundos
↓
OPOSITOR declara pelas peças e recursos adversários disponíveis
↓
NARRADOR julga precedência, interferência e resultado usando as regras existentes
↓
NARRADOR narra no máximo esses 10 segundos
↓
NARRADOR registra o estado resultante
↓
NOVO TURNO
```

A ordem de declaração é operacional. Ela **não determina automaticamente a ordem cronológica das ações dentro dos 10 segundos**.

O NARRADOR julga precedência real conforme os fatos e as regras aplicáveis, incluindo quando relevante:

- velocidade;
- distância;
- surpresa;
- preparação;
- posição;
- mecanismo da ação;
- oportunidade;
- ações já iniciadas;
- interferência entre as peças.

Exemplo:

```text
JOGADOR
→ saco a arma e atiro.

OPOSITOR
→ o guarda, que já estava com a arma apontada, dispara.

NARRADOR
→ julga qual ação ocorre primeiro ou como elas se interferem dentro dos mesmos 10 segundos.
```

### Declaração ampla não resolve o combate inteiro

Em combate, uma declaração pode estabelecer um objetivo maior sem resolver antecipadamente tudo que seria necessário para alcançá-lo.

```text
JOGADOR
→ entro na sala e mato todo mundo.
```

Isso pode ser entendido como:

```text
OBJETIVO
→ entrar na sala
→ tentar derrotar todos os adversários
```

Mas a sentença do turno resolve apenas aquilo que realmente pode acontecer dentro daqueles 10 segundos, considerando as declarações e reações das demais peças.

Os adversários também possuem esses mesmos 10 segundos para:

- atacar;
- procurar cobertura;
- fugir;
- render-se;
- ativar poderes;
- pedir ajuda;
- mudar de posição;
- executar qualquer outra ação legítima.

> **Uma intenção ampla define direção. O turno define quanto dessa direção pode realmente ser resolvido antes que a mesa volte a decidir.**

### Limite da sentença em combate

Durante combate, a sentença termina no primeiro destes limites:

```text
1. surge um novo ponto real de decisão antes dos 10 segundos
OU
2. completam-se os 10 segundos do turno
```

Assim, combate nunca permite atravessar vários intervalos de reação apenas porque uma declaração foi escrita de forma ampla.

### Fechamento mecânico do turno

Antes de iniciar o turno seguinte, todas as consequências mecânicas produzidas naquele intervalo devem estar resolvidas e o estado atual deve refletir o resultado.

Isso inclui, quando aplicável, Dano, Cura, Energia, efeitos, contenções, proteções, condições e demais elementos já definidos em `../resolucao/`.

`operacao/` não redefine nenhum desses cálculos.

> **O turno organiza o tempo. `resolucao/` continua determinando os números.**

### Início e fim do modo de combate

O relógio de turnos começa quando existe confronto ativo no qual várias peças podem agir, reagir ou interferir dentro do mesmo intervalo curto.

Ele termina quando essa necessidade deixa de existir: oposição encerrada, fuga concluída, rendição, separação efetiva ou outra situação em que o tempo não precise mais ser dividido em blocos de 10 segundos.

Depois disso, volta a valer o fluxo normal de janelas fora de combate.

# O que é uma janela de cena

Uma janela abre quando existe algo relevante a decidir ou resolver.

Fora de combate, não é necessário abrir uma nova janela para cada frase, passo ou microação.

Nova janela é necessária quando, por exemplo:

- surge informação capaz de mudar uma escolha;
- aparece obstáculo ou oportunidade relevante;
- outra peça toma iniciativa e exige resposta;
- o OPOSITOR puxa um gancho;
- uma oposição entra em cena;
- o resultado exige nova resposta;
- a intenção anterior deixa de cobrir a ação seguinte.

Em combate, cada turno de 10 segundos constitui uma nova janela mesmo quando a intenção estratégica permanece a mesma.

## Passagem de tempo dentro de uma intenção

Fora de combate, uma declaração pode cobrir minutos, horas ou período maior quando não houver decisão intermediária importante.

Antes de narrar todo o intervalo como concluído, verificar se durante ele:

- outra peça com agência possui ação que intersecta o período;
- um compromisso ou retorno chega ao momento relevante;
- um gancho do OPOSITOR amadurece;
- uma oposição válida interrompe o plano;
- surge informação que mudaria uma decisão.

Se nada disso acontecer, o tempo pode avançar normalmente.

Se algo acontecer no meio, a sentença para **no momento causal da mudança**, não depois de completar artificialmente toda a intenção original.

Durante combate, essa regra é substituída pelo limite máximo de 10 segundos por turno.

# Ordem-base

Fora de combate:

```text
1. JOGADOR HUMANO declara
↓
2. JOGADORES IA aplicáveis declaram, cada um por sua peça
↓
3. JOGADOR IA EVENTUAL é avaliado e, se ativo, declara pelas peças eventuais necessárias
↓
4. OPOSITOR declara movimento, oposição, gancho ou nenhuma intervenção
↓
5. NARRADOR JULGA
↓
6. NARRADOR NARRA A SENTENÇA até o próximo ponto de decisão
↓
7. NARRADOR REGISTRA o que passou a ser verdade
↓
8. nova janela quando houver nova decisão
```

Em combate, a mesma ordem é aplicada a cada turno de 10 segundos:

```text
1. JOGADOR HUMANO declara para o turno
↓
2. JOGADORES IA aplicáveis declaram para o turno
↓
3. JOGADOR IA EVENTUAL declara pelas peças ativas, se houver
↓
4. OPOSITOR declara pelas peças e recursos adversários disponíveis
↓
5. NARRADOR JULGA os mesmos 10 segundos
↓
6. NARRADOR NARRA A SENTENÇA até nova decisão ou até o limite de 10 segundos
↓
7. NARRADOR REGISTRA o estado resultante
↓
8. próximo turno de 10 segundos, se o combate continuar
```

A ordem organiza autoridade. Ela não exige revelar ao JOGADOR HUMANO declarações ou informações que precisem permanecer reservadas.

# 1. JOGADOR HUMANO

Declara o que sua própria peça tenta, quer, diz ou inicia.

Exemplo:

```text
JOGADOR HUMANO
→ atravesso o corredor e tento abrir a porta.
```

A declaração estabelece intenção, não resultado.

# 2. JOGADOR IA

Cada JOGADOR IA declara somente pela peça sob seu próprio controle.

Exemplo:

```text
JOGADOR IA — Ravena
→ vou dormir; não pretendo continuar a conversa esta noite.
```

A declaração deve refletir o que a personagem sabe, quer e faria, não o que seria conveniente para a história.

# 3. JOGADOR IA EVENTUAL

A persona verifica se algum personagem eventual autorizado precisa realmente tomar decisão naquela janela.

Se sim:

```text
JOGADOR IA EVENTUAL
→ assume a peça necessária e declara por ela.
```

Se não:

```text
JOGADOR IA EVENTUAL
→ nenhum personagem eventual precisa de decisão nesta janela.
```

A persona pode operar mais de uma peça eventual, mas cada uma mantém conhecimento, objetivos e decisões separados.

# 4. OPOSITOR — promotoria

Antes do julgamento, o OPOSITOR consulta os ganchos e fatos disponíveis e pergunta:

> **O que daqui eu posso usar para movimentar, pressionar ou fazer um plano adversário avançar?**

Pode declarar:

- retomada de gancho;
- reação de NPC;
- cobrança;
- retorno;
- pressão emocional;
- oportunidade;
- visita;
- conflito;
- ameaça;
- plano de antagonista;
- preparação futura;
- uso de NPCs ou recursos legitimamente disponíveis;
- nenhuma intervenção.

Exemplo doméstico:

```text
GANCHO
→ Ravena sente ciúme de Fulana quando ela está perto de Corvin.

CORVIN
→ vou passar a semana fora.

OPOSITOR
→ essa ausência pode reacender a dúvida de Ravena sobre Fulana.
```

Exemplo adversarial:

```text
GANCHO
→ Trigon quer usar Ravena para abrir caminho à Terra.

OPOSITOR
→ quero tentar capturá-la esta noite usando agentes disponíveis.
```

A declaração ainda não é resultado.

## Arquivo de ganchos

Quando houver ganchos ativos, o OPOSITOR pode consultar:

```text
campanhas/<nome>/mestre/ganchos-do-opositor.md
```

Esse arquivo contém apenas oportunidades atuais e é atualizado conforme `../agencia/ganchos-do-opositor.md`.

# 5. NARRADOR JULGA

O NARRADOR funciona como juiz.

Ele não cria nova oposição e não procura uma saída melhor para nenhum lado.

Consulta somente o necessário para decidir:

```text
DECLARAÇÕES
FICHAS
REGRAS
CENÁRIO
ESTADO ATUAL
CONHECIMENTO
MEIOS
OPORTUNIDADE
FATOS RELEVANTES
```

A pergunta é:

> **Diante do que foi apresentado e do que já é verdade, o que realmente pode acontecer e qual é o resultado?**

Quando o resultado for óbvio pelos fatos e capacidades, não criar incerteza artificial apenas para produzir teste.

Quando existir incerteza real que as regras mandem resolver, aplicar `../resolucao/`.

## Julgar proposta do OPOSITOR

Uma proposta pode ser:

```text
VÁLIDA AGORA
→ possui fundamento, meios e oportunidade.

INVÁLIDA
→ falta fundamento ou contradiz a realidade.

VÁLIDA, MAS AINDA NÃO
→ exige prazo, preparação, deslocamento ou condição futura.
```

Exemplo:

```text
OPOSITOR
→ Trigon envia um agente.

NARRADOR
→ a tentativa é possível, mas colocar esse agente na região exige três dias.
```

Se essa preparação continuar relevante, ela pode virar ou atualizar um gancho do OPOSITOR.

## In dubio pro reo

O julgamento segue esta ordem:

```text
FATO CLARO
→ aplicar.

REGRA CLARA
→ aplicar.

INCERTEZA QUE EXIGE RESOLUÇÃO
→ usar a mecânica.

DÚVIDA REAL QUE RESTOU ENTRE INTERPRETAÇÕES IGUALMENTE PLAUSÍVEIS
→ favorecer os jogadores.
```

> **In dubio pro reo — na dúvida genuína, favoreça a defesa.**

Isso não apaga consequência clara e não substitui uma resolução mecânica necessária.

# NPCs e delegação ao OPOSITOR

O OPOSITOR não controla automaticamente todas as forças do mundo.

Quando quiser usar uma peça adversária, o NARRADOR julga se ela realmente está disponível.

Exemplo:

```text
OPOSITOR
→ quero usar a polícia que já procura Corvin para prendê-lo quando ele voltar.
```

O NARRADOR verifica:

```text
- existe fundamento para a polícia agir?
- ela sabe que Corvin voltou?
- possui meios?
- possui oportunidade?
- quais policiais realmente podem participar?
```

Se válido:

```text
NARRADOR
→ delega temporariamente os NPCs disponíveis ao OPOSITOR.

OPOSITOR
→ passa a jogar suas decisões naquela oposição.
```

Exemplo de combate:

```text
JOGADOR IA — RAVENA
            VS
OPOSITOR — agentes de Trigon

NARRADOR
→ juiz.
```

Durante a delegação, o OPOSITOR decide estratégia, ações, alvos e uso legítimo das capacidades das peças cedidas.

O NARRADOR continua apenas julgando.

Quando a oposição termina, a delegação termina.

# 6. NARRADOR NARRA A SENTENÇA

Depois de julgar, o NARRADOR transforma o resultado em cena.

A narração pode mostrar:

- o que realmente aconteceu;
- sucesso ou falha;
- consequência;
- mudança de posição;
- dano ou condição;
- reação observável;
- informação legitimamente percebida;
- nova situação.

Fora de combate, ele narra somente até o próximo ponto em que alguém precise decidir novamente.

Em combate, ele narra somente até o primeiro destes limites:

```text
nova decisão relevante
OU
fim dos 10 segundos do turno
```

Exemplo fora de combate:

```text
JOGADOR HUMANO
→ atravesso o corredor e abro a porta.

OPOSITOR
→ um guarda autorizado entra no corredor antes disso.

NARRADOR
→ “Você cruza metade do corredor quando o guarda surge na esquina e o vê.”
```

A ação original não decide automaticamente se o personagem luta, foge, engana ou continua andando.

Nesse ponto abre-se nova janela.

> **Fora de combate, a sentença termina onde consequência volta a ser escolha. Em combate, ela termina nesse ponto ou no limite de 10 segundos, o que ocorrer primeiro.**

# 7. NARRADOR REGISTRA

Depois da sentença, o NARRADOR registra somente o que realmente passou a ser verdade.

Conforme o caso:

```text
estado/atual.md
→ situação presente.

mestre/ganchos-do-opositor.md
→ pontas, planos ou oportunidades que continuam vivos.

mundo/
→ nova verdade estável quando apropriado.

ficha
→ mudança estável conforme as regras de aprovação.

livro/
→ história efetivamente ocorrida quando consolidada.
```

Registrar não cria nova consequência.

Se um gancho foi resolvido, removê-lo. Se mudou, atualizá-lo. Se a sentença produziu nova ponta útil, ela pode ser adicionada.

Em combate, o registro ao fim do turno deve refletir todas as consequências mecânicas já resolvidas pelas regras de `../resolucao/`, sem criar cálculo paralelo em `operacao/`.

# Nenhum movimento também é válido

O OPOSITOR não precisa produzir intervenção em toda janela.

```text
OPOSITOR
→ nenhuma intervenção; a cena já está avançando por suas próprias decisões.
```

Isso é especialmente importante em romance, conversa, cotidiano, investigação ou qualquer cena que já esteja gerando escolhas suficientes.

Durante combate, `nenhuma intervenção` também é válido para um turno se o OPOSITOR não possuir ação adversária legítima naquele intervalo.

# Regra contra correção retroativa

Depois da sentença, nenhuma persona adiciona um fato anterior apenas para alterar o resultado.

O OPOSITOR não pode inventar nova oposição retroativa.

O NARRADOR não pode inventar dificuldade retroativa.

Se o resultado criar nova oportunidade legítima, isso pertence à próxima janela ou, em combate, ao próximo turno.

# Regra final

> **Fora de combate, cada janela é uma pequena audiência que termina quando consequência volta a ser escolha. Em combate, a mesma audiência é dividida em turnos simultâneos de 10 segundos: todas as peças recebem o mesmo intervalo, a ordem de declaração não define automaticamente a ordem dos acontecimentos, as mecânicas continuam pertencendo a `resolucao/`, e nenhuma sentença pode atravessar o limite do turno. Na dúvida genuína que restar depois das regras e fatos aplicáveis, in dubio pro reo.**