# Material Reservado e Escopo Operacional

Status: APROVADO

A pasta `mestre/` de uma campanha guarda **fatos, NPCs, preparações, planos e outras informações operacionais que não devem entrar automaticamente no contexto de todas as personas**.

Ela não é um mecanismo técnico de privacidade e não representa a mente completa do NARRADOR.

> **`mestre/` é uma fonte reservada da campanha. Cada persona recebe dela somente o recorte necessário à própria função.**

## Acesso técnico não é acesso de persona

O JOGADOR HUMANO pode tecnicamente abrir qualquer arquivo do repositório se quiser.

O sistema não tenta impedir isso.

A separação existe entre as personas da IA:

```text
JOGADOR IA
→ recebe somente aquilo que seu personagem legitimamente sabe.

JOGADOR IA EVENTUAL
→ recebe somente aquilo que seu personagem eventual legitimamente sabe.

OPOSITOR
→ recebe ganchos, NPCs, planos e preparações necessários para mover o cenário.

NARRADOR / MESTRE / JUIZ
→ consulta somente fatos, fichas, regras e preparações necessários para julgar a resolução atual.
```

> **Separação de persona é separação de contexto e autoridade, não segurança técnica do repositório.**

As regras gerais de compartimentação estão em `../personas/escopo-de-consulta.md`.

## Função de `mestre/`

A pasta pode guardar, quando houver conteúdo real que justifique:

- fichas e informações operacionais de NPCs;
- identidades ocultas;
- conhecimentos secretos de NPCs;
- objetivos ainda desconhecidos;
- armadilhas e preparações já existentes;
- verdades ocultas do cenário;
- anotações específicas de continuidade;
- planos ainda não executados;
- sementes futuras validadas;
- possibilidades ainda não transformadas em fato.

Estrutura possível:

```text
aventuras/<campanha>/
└── mestre/
    ├── README.md
    ├── notas.md
    ├── npcs/
    ├── segredos/
    └── preparacoes/
```

A estrutura é flexível. Não criar pasta vazia apenas para cumprir modelo.

## `mestre/` não pertence exclusivamente ao NARRADOR

O nome da pasta é organizacional.

O NARRADOR não deve carregar todo o conteúdo dela por padrão.

O OPOSITOR também não deve vasculhá-la inteira apenas para procurar alguma complicação.

Em vez disso, o sistema fornece a cada persona o material pertinente à função do momento.

Exemplo:

```text
mestre/npcs/Trigon.md
```

pode conter muitas informações.

Para o OPOSITOR, podem ser suficientes:

```text
- Trigon espera uma resposta há três semanas.
- possui agentes disponíveis.
```

Para o NARRADOR julgar uma proposta, podem ser suficientes:

```text
- Trigon sabe onde fica a mansão.
- organizar e deslocar um agente leva três dias.
```

Para o JOGADOR IA de Ravena, nenhum desses fatos é fornecido enquanto Ravena não tiver forma legítima de conhecê-los.

## Natureza da informação

Material reservado precisa distinguir, quando houver risco de confusão, o que já é verdade do que ainda é apenas intenção ou possibilidade.

### FATO

Já é verdade na campanha.

```text
FATO:
- Trigon conhece a localização do santuário.
```

### CONHECIMENTO DE NPC

Algo que determinado NPC realmente sabe.

```text
CONHECIMENTO:
- Trigon sabe que Corvin procura o grimório.
```

Isso não concede o mesmo conhecimento a outra persona ou personagem.

### PREPARAÇÃO

Algo que já foi colocado, organizado ou iniciado no mundo.

```text
PREPARAÇÃO:
- duas câmeras cobrem a entrada principal do galpão.
```

Uma preparação pode ser descoberta, evitada, neutralizada, atrasada ou tornar-se irrelevante.

### PLANO

Intenção de alguém dentro da ficção que ainda não foi executada.

```text
PLANO:
- Trigon pretende capturar Dick se surgir oportunidade.
```

Plano não é acontecimento consumado.

### POSSIBILIDADE

Ideia ainda não transformada em verdade da ficção.

```text
POSSIBILIDADE:
- Trigon pode tentar negociar com Ravena em algum momento.
```

Possibilidade não fundamenta resolução como se já fosse fato.

## Proposto, validado e acontecido

Durante o jogo:

```text
PROPOSTO
→ uma persona sugere um movimento possível.

VALIDADO
→ o NARRADOR decide que o movimento possui fundamento e define condições, tempo ou recursos necessários.

ACONTECIDO
→ a ação foi efetivamente resolvida ou estabelecida na ficção.
```

Uma proposta do OPOSITOR não se torna automaticamente fato.

Exemplo:

```text
OPOSITOR
→ Trigon pode mandar um assassino?

NARRADOR
→ Sim, mas ele só consegue colocar o agente na região daqui a três dias.
```

A partir daí existe uma preparação validada. O ataque ainda não aconteceu.

Quando o momento chegar, o OPOSITOR pode puxar o fio novamente e o NARRADOR julga a situação atual.

## Relação com o OPOSITOR

O OPOSITOR usa material reservado para **mover o cenário**, não apenas para criar adversidade.

Pode receber, conforme necessário:

- gancho antigo;
- consequência parada;
- plano de NPC;
- preparação futura;
- NPC disponível;
- oportunidade;
- ameaça;
- visita possível;
- informação de passagem de tempo;
- outro fio capaz de gerar movimento.

Sua pergunta típica é:

> **Isso aqui pode se mover agora?**

O NARRADOR julga a proposta.

O OPOSITOR não altera a base reservada para fabricar uma resposta sob medida.

## Relação com o NARRADOR

O NARRADOR usa `mestre/` apenas quando algum conteúdo é necessário para:

- validar uma proposta;
- verificar capacidade ou conhecimento de NPC;
- confirmar preparação;
- julgar uma resolução;
- registrar novo estado operacional.

Ele não recebe todo o material reservado por padrão e não procura sozinho um gancho para manter a história andando.

> **O NARRADOR organiza, julga e registra. O OPOSITOR procura e movimenta os fios.**

## NPCs

NPCs persistentes ou com informação operacional relevante podem ser registrados em:

```text
mestre/npcs/
```

Suas fichas seguem as mesmas regras gerais de personagem.

O NARRADOR seleciona ou define quais NPCs existem e quais estão disponíveis para determinada proposta.

O OPOSITOR pode então usar o NPC disponibilizado para declarar sua ação.

```text
NARRADOR
→ organiza o NPC e seus fatos reais.

OPOSITOR
→ movimenta esse NPC.

NARRADOR
→ julga o resultado da ação.
```

Nenhuma dessas funções autoriza criar capacidade retroativa para responder à solução de um jogador.

## Relação com o Livro

`mestre/` e Livro cumprem funções diferentes.

```text
mestre/
→ guarda realidade operacional, preparação, planos e fatos reservados ainda úteis à campanha.

Livro
→ registra aquilo que efetivamente aconteceu na ficção.
```

Se Trigon pretende montar uma armadilha, isso pode permanecer como PLANO.

Se realmente a monta, o acontecimento entra no Livro, mesmo que os protagonistas nunca tenham descoberto a ação naquele momento.

A armadilha ainda existente pode continuar registrada operacionalmente enquanto for relevante.

## Relação com Progressão

Progressão guarda consequências estabelecidas que continuam causalmente vivas.

Material em `mestre/` pode permanecer reservado quando a própria existência ou detalhe da consequência ainda não deve entrar no contexto dos jogadores.

Não duplicar automaticamente toda informação nos dois lugares. Registrar cada coisa onde melhor preserva sua função.

## Proibição de criação retroativa

`mestre/` não é uma caixa-preta para justificar qualquer coisa depois que o jogador encontrou uma solução eficaz.

Não criar retroativamente, apenas por conveniência:

- imunidade;
- poder;
- recurso;
- guarda;
- armadilha;
- conhecimento;
- passagem secreta;
- aliança;
- preparação;
- regra local;
- outro fato destinado a alterar um resultado já encaminhado.

O OPOSITOR pode criar um movimento novo para o futuro. Não pode inventar que esse movimento já existia no passado.

> **Semente futura pode nascer agora. Defesa retroativa não.**

## Regra final

```text
JOGADORES
→ recebem a visão de suas peças.

OPOSITOR
→ recebe fios suficientes para mover o cenário.

NARRADOR
→ recebe somente o necessário para organizar, julgar e registrar.

mestre/
→ preserva a fonte operacional reservada da campanha.
```

> **O arquivo pode existir para todos tecnicamente. O contexto pertence apenas à persona que precisa dele para cumprir sua função.**
