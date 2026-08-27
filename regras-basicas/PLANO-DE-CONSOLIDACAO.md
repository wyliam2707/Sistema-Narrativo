# Plano de Consolidação — regras-basicas

Status: EM TRABALHO

Este arquivo registra a análise comparativa entre `sistema/` e `regras-basicas/` e serve como roteiro para que `regras-basicas/` consiga substituir o trabalho operacional do sistema antigo sem copiar complexidade desnecessária.

## Objetivo

Testar a seguinte condição:

```text
NARRADOR A
→ usa somente sistema/

NARRADOR B
→ usa somente regras-basicas/

MESMA CAMPANHA
MESMAS DECLARAÇÕES
→ ambos devem conseguir executar todas as funções necessárias da mesa.
```

A migração não deve copiar automaticamente a arquitetura antiga. Cada ponto será discutido, simplificado e consolidado separadamente.

## O que já está suficientemente consolidado

### Tribunal e autoridade

`regras-basicas/nucleo/`

Já define:

- Narrador;
- Jogador Humano;
- Jogador IA;
- Jogador IA Eventual;
- Opositor;
- janelas sem ordem fixa de fala;
- declaração obrigatória das cadeiras participantes;
- intenção diferente de realidade;
- separação de conhecimento e autoridade.

### Agência e continuidade

A antiga função de `sistema/agencia/` foi absorvida por:

```text
Jogador IA Eventual
+
Opositor
+
Registro
+
processos e prazos
```

Não há necessidade atual de recriar uma pasta `agencia/`.

### Operação fora de combate

O fluxo antigo de janelas e interrupções foi absorvido pelo Tribunal e pelo manual do Mestre.

Fora de combate:

```text
situação aberta
→ cadeiras declaram
→ janela completa
→ Narrador julga
→ resolve quando necessário
→ narra
→ registra
```

### Narração

`regras-basicas/mestre/` já funciona como manual operacional do Narrador para:

- julgamento;
- interpretação;
- perspectiva;
- fala;
- ritmo;
- descrição;
- dramatização e resumo;
- limite da sentença.

Princípios consolidados:

```text
INTERPRETAR
≠
DECIDIR
```

```text
PERSONAGEM SABE
≠
JOGADOR PRECISA LEMBRAR
```

### Registro

`regras-basicas/registro/` já diferencia:

```text
LIVRO
→ passado canônico

ESTADO
→ presente operacional

PERSONAGEM
→ conhecimento/memória legítima

MUNDO
→ verdade estável

MESTRE
→ material de julgamento/direção necessário

OPOSITOR
→ outro lado da trama, planos e processos adversariais
```

## Pontos que faltam consolidar

Trabalhar nesta ordem, salvo decisão posterior do usuário.

### 1. Fichas de personagens — ATUAL

Destino decidido:

```text
regras-basicas/jogador/
```

Consolidar regras para criação e representação de:

- personagem do Jogador Humano;
- personagens de Jogador IA;
- personagens eventuais;
- NPCs e adversários.

Princípio inicial:

> NPC não precisa ser uma mecânica diferente. Pode usar a mesma estrutura de personagem, com quantidade de informação proporcional ao necessário.

Pontos a decidir:

- Status da ficha;
- Importância da personagem;
- Controle;
- modelo de ficha;
- ficha completa, rápida e mínima;
- Atributos;
- Perícias;
- Vida/Mana máximas quando definidas;
- Poderes;
- personalidade;
- conhecimento;
- relações;
- recursos.

### 2. Combate, Vida, Mana, Status e Poderes

Consolidar no novo Núcleo somente depois da ficha definir quais valores existem.

Precisará responder:

- iniciativa ou estrutura concorrente de combate;
- ataque;
- Defesa/Resistência;
- dano;
- Vida;
- Mana;
- condições temporárias;
- duração;
- recuperação;
- fórmulas próprias de Poder.

Não copiar automaticamente o combate antigo.

### 3. Manual operacional do Jogador

Depois que a ficha e as mecânicas estiverem definidas, completar `regras-basicas/jogador/` como manual de uso da peça.

Deve ensinar:

- como ler a ficha;
- como escolher uma ação;
- como usar Perícias;
- como usar Poderes;
- como gastar recursos;
- como agir em combate;
- como formular uma intenção sem precisar escrever literatura completa.

### 4. START, retomada e montagem da Mesa

Criar procedimento para uma IA nova ligar o motor usando somente `regras-basicas/` e `campanhas/`.

Fluxo esperado:

```text
ler regras-basicas/
→ Nova campanha ou Continuar
→ carregar campanha
→ reconstruir cadeiras
→ carregar estado atual
→ carregar fichas/fontes necessárias
→ respeitar escopos
→ continuar.
```

Também consolidar como uma única IA pode executar várias personas sem misturar conhecimento ou autoridade.

### 5. Criação de campanha

Depois de ficha, mecânicas e START estarem estáveis, consolidar procedimento de criação de uma campanha do zero.

Deve abranger somente o necessário:

```text
nome
→ estrutura da campanha
→ direção narrativa
→ personagens/fichas
→ estado inicial
→ Mesa operacional
→ START
```

## Critério de conclusão

A reformulação estará funcionalmente pronta para substituir o sistema antigo quando uma IA puder usar somente:

```text
regras-basicas/
+
campanhas/<nome>/
```

e conseguir:

- criar ou retomar campanha;
- montar as personas;
- interpretar fichas;
- receber e julgar declarações;
- resolver ações comuns e combate;
- usar Poderes e recursos;
- controlar continuidade e oposição;
- narrar resultados;
- registrar e salvar a história;
- continuar sem consultar `sistema/`.

## Regra de trabalho

```text
1. pesquisar em sistema/
2. identificar a função útil
3. remover duplicação e complexidade desnecessária
4. adaptar ao modelo novo
5. discutir e aprovar
6. salvar em regras-basicas/
7. não alterar sistema/ durante a migração
```

> **O plano é um roteiro de trabalho, não uma regra da mesa. Cada item deve ser consolidado ponto a ponto.**
