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
uma relação mudou de forma consolidada?
um desejo, medo, hábito ou percepção mudou de forma duradoura?
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
3. SEPARAR personagem, passado, presente, contexto e processos.
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

```text
Prazo inicial: 10 dias
Tempo transcorrido: 3 dias
Restante: 7 dias
```

Ou manter uma data/momento-alvo quando a campanha usar calendário absoluto.

## Conhecimento adquirido

Se uma personagem aprende algo que deverá influenciar decisões futuras, verificar se esse conhecimento precisa entrar em `Conhecimento relevante` da ficha.

Regra prática:

```text
se esquecer provavelmente faria a personagem interpretar ou decidir de forma incoerente
→ atualizar a ficha.

se é apenas detalhe momentâneo
→ Estado Atual, se ainda importar.

se é contexto amplo já preservado em livro, mundo ou outra fonte
→ não copiar integralmente sem necessidade.
```

Exemplo:

```text
Ravena descobre que relações múltiplas são culturalmente normais para Estelar.
```

Se isso passa a ser importante para interpretar sua relação futura, pode gerar na ficha de Ravena:

```text
## Conhecimento relevante
--- Sabe que relações múltiplas são culturalmente normais para Estelar.
```

Não copiar automaticamente para outras personagens.

## Evolução de interpretação

Quando algo muda de forma duradoura em quem a personagem é ou em como ela entende uma relação, atualizar o bloco apropriado da ficha.

Pode afetar:

```text
Personalidade e tendências
Desejos / objetivos
Medos / limites
Rotina e hábitos persistentes
Relações
Conhecimento relevante
História consolidada relevante
```

Não reescrever a ficha por uma emoção passageira. A mudança precisa estar realmente consolidada.

Uma vez consolidada, a nova informação passa a orientar interpretações futuras e não deve ser tratada como descoberta novamente sem fato novo.

## Mudança de estado

Se algo deixa de ser verdade no presente, atualizar ou remover da fonte operacional atual.

```text
ANTES
Status: Envenenado

DEPOIS DO ANTÍDOTO
Status: nenhum
```

Marcas atuais de Vida/Mente e Mana atual são atualizadas em `estado/atual.md` quando precisarem ser acompanhadas.

O fato histórico continua pertencendo ao Livro quando relevante.

## Mudança permanente

Quando a campanha estabelecer mudança permanente de ficha, relação, mundo, capacidade, Traço ou Recurso, atualizar a fonte estável correspondente.

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

- Estado Atual;
- conhecimento relevante que afeta interpretação;
- mudanças consolidadas de personagem;
- processos;
- prazos;
- mudanças estáveis do mundo.

## Checklist rápido

Antes de encerrar um salvamento:

```text
[ ] salvei somente fatos já estabelecidos?
[ ] o presente está correto?
[ ] Vida, Mente e Mana atuais estão corretas quando relevantes?
[ ] conhecimento importante ficou com a personagem certa?
[ ] alguma evolução consolidada precisa atualizar a ficha?
[ ] relações continuam refletindo o ponto de vista do dono da ficha?
[ ] processos e prazos continuam vivos?
[ ] planos futuros não viraram acontecimentos?
[ ] removi estados que já terminaram?
[ ] evitei duplicação desnecessária?
[ ] não avancei a ficção durante o salvamento?
```

## Regra final

> **Salvar a história é distribuir verdades já estabelecidas nas fontes corretas. O Livro preserva o passado, o Estado preserva o presente e a ficha preserva quem a personagem é e o conhecimento que ela precisa levar para futuras interpretações. Consolidar não é redescobrir nem criar fato novo.**
