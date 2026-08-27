# Salvar a História

Status: REFORMULAÇÃO / NÃO IMPLEMENTADO

Este arquivo define **como salvar a campanha sem continuar jogando**.

Salvar significa persistir somente o que já foi estabelecido.

> **Salvar preserva. Não cria.**

## Quando registrar

O Registro pode ser atualizado em três escalas:

```text
DEPOIS DE UMA SENTENÇA
→ registrar somente mudanças que precisam persistir imediatamente.

SALVAR ESTADO
→ preservar o ponto atual para retomada, mesmo no meio de uma cena.

FECHAR / SALVAR CAPÍTULO
→ consolidar o trecho encerrado no Livro e atualizar as fontes operacionais afetadas.
```

## Depois de uma sentença

Depois que o Narrador julga e narra uma sentença, verificar apenas:

```text
algo mudou de forma persistente?
alguém aprendeu algo que precisa ser lembrado depois?
um efeito ou condição continua ativo?
um processo começou, terminou ou mudou?
um prazo foi criado, reduzido ou venceu?
um fato estável do mundo mudou?
um plano do Opositor mudou?
```

Se a resposta for não, não é necessário criar registro só porque houve uma resposta narrativa.

## Procedimento básico

```text
1. PARAR no último fato estabelecido.
2. IDENTIFICAR o que realmente mudou.
3. SEPARAR passado, presente, conhecimento e processos.
4. ESCOLHER a fonte principal correta.
5. ATUALIZAR somente os arquivos afetados.
6. NÃO avançar a ficção durante o salvamento.
```

## O que nunca deve ser promovido a fato

Não salvar como realidade concluída:

- intenção ainda não executada;
- ação ainda não julgada;
- hipótese do jogador;
- suspeita como se fosse certeza;
- plano futuro como se já tivesse acontecido;
- informação secreta como conhecimento de quem não a descobriu;
- resultado que ainda depende de nova decisão ou teste.

Exemplo:

```text
JOGADOR
→ amanhã vou conversar com Ravena.
```

Pode ser preservado, se realmente relevante:

```text
Intenção: conversar com Ravena amanhã.
```

Não:

```text
Acontecimento: conversou com Ravena amanhã.
```

## Salvar estado no meio da cena

O usuário pode pedir para salvar em qualquer ponto.

Nesse caso:

```text
NÃO terminar a cena por conta própria.
NÃO criar fala de despedida.
NÃO concluir combate ou investigação pendente.
NÃO resolver a próxima decisão.
```

Salvar somente o último estado fechado da ficção.

Se algo estiver em andamento, registrar isso claramente.

Exemplo:

```text
Local: corredor da mansão
Situação: Corvin abriu a porta da biblioteca
Ravena está do outro lado
Próxima decisão ainda não foi declarada
```

## Processos fora de cena

Quando uma ação julgada cria um processo de duração maior, salvar:

```text
PROCESSO
→ o que está acontecendo.

RESPONSÁVEL
→ quem iniciou ou sustenta o processo, quando relevante.

ESTADO
→ em andamento / interrompido / concluído.

PRAZO
→ quando existe.

RESULTADO FUTURO JÁ ESTABELECIDO
→ somente aquilo que o Narrador realmente julgou.
```

Exemplo:

```text
Processo: investigação do desaparecimento de Ravena
Responsável: Dick
Estado: em andamento
Prazo: primeiras pistas em 10 dias
```

Não é necessário manter Dick ativo em todas as janelas apenas para esse processo continuar.

## Contagem de prazo

Quando tempo efetivamente passa, atualizar o prazo quando isso facilitar a continuidade.

Exemplo:

```text
Prazo inicial: 10 dias
Tempo transcorrido: 3 dias
Restante: 7 dias
```

Ou manter uma data/momento-alvo quando a campanha usar calendário absoluto.

O formato pode variar, mas o prazo precisa ser inequívoco.

## Conhecimento adquirido

Se uma personagem aprende algo que deverá poder usar depois, salvar na fonte legítima dela.

Exemplo:

```text
Ravena descobre que o símbolo pertence à Ordem de X.
```

Pode gerar:

```text
personagens/ravena/conhecimento.md
→ Símbolo reconhecido como pertencente à Ordem de X.
```

Não copiar automaticamente para outras personagens.

## Mudança de estado

Se algo deixa de ser verdade, atualizar ou remover da fonte operacional atual.

Exemplo:

```text
ANTES
Status: Envenenado

DEPOIS DO ANTÍDOTO
Status: nenhum
```

O fato de ter sido envenenado continua pertencendo ao histórico no Livro.

O estado atual mostra somente o presente.

## Mudança permanente

Quando a campanha estabelecer mudança permanente de ficha, relação, mundo ou capacidade, atualizar a fonte estável correspondente.

Não transformar automaticamente toda consequência temporária em mudança permanente.

## Planos do Opositor

Quando o Opositor declara um plano e o Narrador julga que ele é válido como processo futuro, salvar em:

```text
campanhas/<nome>/opositor/
```

Exemplo:

```text
Vilão X
Plano: atacar a base
Estado: preparando
Prazo: 5 dias
Conhecimento: sabe apenas [X]
Recursos: [somente os já estabelecidos]
```

Quando o plano muda, atualizar o mesmo registro em vez de manter versões conflitantes como igualmente atuais.

## O Livro não precisa ser atualizado a cada sentença

O Livro é histórico consolidado.

A campanha pode acumular várias sentenças e depois consolidá-las em um capítulo quando houver fechamento apropriado.

Durante a sessão, o mais importante é não perder:

- estado atual;
- conhecimentos persistentes;
- processos;
- prazos;
- mudanças estáveis.

## Checklist rápido

Antes de encerrar um salvamento:

```text
[ ] salvei somente fatos já estabelecidos?
[ ] o presente está correto?
[ ] conhecimento ficou com a personagem certa?
[ ] processos e prazos continuam vivos?
[ ] planos futuros não viraram acontecimentos?
[ ] removi estados que já terminaram?
[ ] evitei duplicação desnecessária?
[ ] não avancei a ficção durante o salvamento?
```

## Regra final

> **Salvar a história é distribuir as verdades já estabelecidas nas fontes corretas da campanha. Preserve o passado no Livro, o presente no Estado, a memória nas fontes de conhecimento e os processos futuros nas áreas responsáveis, sem criar nenhum fato novo durante o salvamento.**