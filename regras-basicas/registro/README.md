# Manual de Registro da Campanha

Status: REFORMULAÇÃO / NÃO IMPLEMENTADO

Esta pasta é o **manual de persistência da história**.

Ela explica como transformar acontecimentos já julgados e narrados em arquivos permanentes dentro de:

```text
campanhas/<nome>/
```

`regras-basicas/registro/` contém somente regras e modelos.

Nenhum fato vivo de uma campanha deve ser salvo aqui.

> **O jogo acontece na mesa. O Registro preserva o que precisa continuar verdadeiro depois da resposta.**

## Função do Registro

O Registro responde a quatro perguntas:

```text
O QUE ACONTECEU?
→ Livro / histórico canônico.

COMO A CAMPANHA ESTÁ AGORA?
→ Estado atual.

O QUE CADA PERSONAGEM SABE?
→ fontes de conhecimento daquela personagem.

O QUE CONTINUA EXISTINDO FORA DA CENA?
→ mundo, processos, prazos, planos e outras fontes apropriadas.
```

Registrar não cria ficção.

```text
DECLARAÇÃO
→ intenção.

JULGAMENTO / RESOLUÇÃO
→ estabelece realidade.

NARRAÇÃO
→ apresenta a realidade.

REGISTRO
→ preserva a realidade que precisa sobreviver.
```

## Arquitetura deste manual

```text
registro/
├── README.md
├── fontes-da-campanha.md
├── salvar-a-historia.md
├── estado-atual.md
└── livro-e-capitulos.md
```

### `fontes-da-campanha.md`

Explica **onde cada tipo de verdade deve ser salvo**.

Princípio:

> **Cada verdade deve ter uma fonte principal.**

### `salvar-a-historia.md`

Manual operacional para salvar sem avançar a ficção.

Explica:

- o que registrar depois de uma sentença;
- como salvar no meio de uma cena;
- como preservar processos e prazos;
- como atualizar conhecimento;
- como evitar registrar intenção como fato.

### `estado-atual.md`

Define a fotografia operacional necessária para retomar a campanha exatamente de onde ela parou.

### `livro-e-capitulos.md`

Define o histórico canônico: como consolidar o que realmente aconteceu em capítulos sem transformar o Livro em log técnico da sessão.

## Estrutura recomendada de uma campanha

A estrutura concreta pode variar, mas a referência geral é:

```text
campanhas/<nome>/
├── README.md
├── personagens/
├── estado/
│   └── atual.md
├── mundo/
├── mestre/
├── opositor/
└── livro/
```

Função de cada área:

```text
README
→ identidade, estado geral e roteamento da campanha.

PERSONAGENS
→ quem as personagens são e, quando necessário, o que cada uma conhece.

ESTADO
→ como a campanha precisa ser retomada agora.

MUNDO
→ verdades estáveis do cenário.

MESTRE
→ dados operacionais próprios do Narrador quando necessários.

OPOSITOR
→ planos, processos e informações do outro lado da trama.

LIVRO
→ o que efetivamente aconteceu na história.
```

## Verdade estabelecida x informação disponível

Um fato pode ser verdadeiro na campanha sem ser conhecido por todas as personagens.

```text
CAMPANHA SABE
≠
PERSONAGEM SABE
```

Arquivos podem permanecer visíveis no repositório.

A separação é operacional:

```text
arquivo visível
→ pode ser auditado e editado pelo responsável pela campanha.

informação reservada
→ não pode ser usada como conhecimento da personagem que ainda não a descobriu.
```

## O Registro também é memória da personagem

O jogador não precisa memorizar perfeitamente tudo que sua personagem já sabe.

Quando uma informação foi legitimamente adquirida e precisa sobreviver entre cenas ou retomadas, ela deve estar disponível em uma fonte apropriada da campanha.

Assim:

```text
FICHA
+
FATOS ESTABELECIDOS NA CENA ATUAL
+
REGISTRO LEGÍTIMO DA PERSONAGEM
→ base de memória e decisão da personagem.
```

## Registrar somente fatos concluídos

Nunca salvar como acontecimento algo que ainda é somente intenção, hipótese ou plano.

```text
JOGADOR
→ vou procurar Ravena amanhã.

NÃO SALVAR COMO HISTÓRIA
→ encontrou Ravena amanhã.
```

Pode ser registrado, quando relevante:

```text
INTENÇÃO ATUAL
→ pretende procurar Ravena amanhã.
```

Da mesma forma:

```text
OPOSITOR
→ Vilão X prepara um sequestro para daqui a 5 dias.

NARRADOR julga como válido
→ processo/plano pode entrar no Registro do Opositor.

LIVRO
→ não registra o sequestro como acontecido enquanto ele não acontecer.
```

## Processos e prazos

Um resultado pode continuar vivo mesmo fora da cena.

Exemplo:

```text
Dick inicia investigação.
NARRADOR estabelece: primeiras pistas em 10 dias.
```

Salvar:

```text
Processo: investigação de Dick
Estado: em andamento
Prazo: primeiras pistas em 10 dias
```

O processo não precisa ser redeclarado em toda janela distante.

O Registro mantém a continuidade.

## Não duplicar tudo

Não copiar a mesma informação inteira para vários arquivos apenas por segurança.

Exemplo:

```text
Livro
→ registra que o envenenamento aconteceu.

Estado atual
→ registra que a personagem continua Envenenada.
```

Isso não é duplicação ruim porque cada fonte responde a uma pergunta diferente.

Mas não é necessário copiar toda a cena do envenenamento para `estado/atual.md`.

> **Livro guarda passado. Estado guarda presente.**

## Salvamento não joga

Quando o usuário pedir para salvar, registrar ou fechar capítulo:

- parar no último fato estabelecido;
- não criar uma cena extra;
- não resolver ação ainda pendente;
- não decidir pelo jogador;
- não executar automaticamente plano futuro;
- não inventar consequência para produzir fechamento.

```text
SALVAR
→ preservar.

SALVAR
≠
continuar jogando.
```

## Dados vivos ficam somente em `campanhas/`

Tudo que pertence a uma história específica deve ser salvo em:

```text
campanhas/<nome>/
```

Isso inclui:

- fichas reais;
- conhecimentos;
- relações;
- estado atual;
- Vida, Mana, condições e recursos;
- acontecimentos;
- capítulos;
- mundo;
- processos;
- prazos;
- eventos futuros já estabelecidos;
- planos do Opositor;
- registros do Mestre.

## Regra final

> **Registro é a memória canônica da campanha. Salve somente o que foi legitimamente estabelecido, coloque cada verdade em sua fonte principal e mantenha separados o passado da história, o presente operacional, o conhecimento das personagens e os processos ainda em andamento. Tudo que for dado vivo deve existir dentro de `campanhas/<nome>/`.**