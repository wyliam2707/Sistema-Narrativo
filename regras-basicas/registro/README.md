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

O Registro responde:

```text
QUEM É A PERSONAGEM E O QUE ELA PRECISA LEMBRAR PARA SER INTERPRETADA?
→ ficha da personagem.

O QUE ACONTECEU?
→ Livro / histórico canônico.

COMO A CAMPANHA ESTÁ AGORA?
→ Estado Atual.

O QUE É VERDADE EXTERNA À PERSONAGEM?
→ mundo, livros e demais fontes apropriadas.

O QUE CONTINUA EXISTINDO FORA DA CENA?
→ processos, prazos, planos e outras fontes apropriadas.
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

Explica onde cada tipo de verdade deve ser salvo.

> **Cada verdade deve ter uma fonte principal.**

### `salvar-a-historia.md`

Manual operacional para salvar sem avançar a ficção.

### `estado-atual.md`

Define a fotografia operacional necessária para retomar a campanha exatamente de onde ela parou.

### `livro-e-capitulos.md`

Define o histórico canônico do que realmente aconteceu.

## Estrutura recomendada de uma campanha

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
→ fichas reais; principal fonte de interpretação de cada personagem.

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

## Ficha e memória da personagem

A ficha é a principal fonte de interpretação da personagem.

Quando um fato adquirido passa a ser importante para decisões futuras, relações, evolução emocional ou leitura recorrente de situações, ele deve ser consolidado em `Conhecimento relevante` ou no bloco apropriado da própria ficha.

```text
se esquecer provavelmente faria a personagem agir de forma incoerente
→ consolidar na ficha.

se importa apenas para o momento atual
→ Estado Atual.

se é contexto externo já bem guardado em livro, mundo ou outra fonte
→ não duplicar integralmente na ficha.
```

O que merece consolidação depende do foco da campanha. Romance, terror e investigação podem tornar informações diferentes importantes para interpretação.

Conhecimento consolidado não deve ser tratado novamente como descoberta apenas porque a campanha foi retomada depois.

## Verdade estabelecida x informação disponível

Um fato pode ser verdadeiro na campanha sem ser conhecido por todas as personagens.

```text
CAMPANHA SABE
≠
PERSONAGEM SABE
```

Arquivos podem permanecer visíveis no repositório, mas informação reservada não pode ser usada por uma personagem que ainda não a descobriu.

Relações registradas na ficha representam o ponto de vista do dono daquela ficha. A percepção de outra personagem só entra como conhecimento quando for legitimamente conhecida.

## Registrar somente fatos concluídos

Nunca salvar como acontecimento algo que ainda é somente intenção, hipótese ou plano.

```text
JOGADOR
→ vou procurar Ravena amanhã.

NÃO SALVAR COMO HISTÓRIA
→ encontrou Ravena amanhã.
```

Pode ser preservado, quando relevante:

```text
INTENÇÃO ATUAL
→ pretende procurar Ravena amanhã.
```

Da mesma forma, um plano futuro do Opositor permanece plano até realmente acontecer.

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

## Duplicação legítima

Uma mesma realidade pode aparecer em duas fontes quando cada uma possui função diferente.

```text
LIVRO
→ registra que a personagem descobriu um fato.

FICHA / CONHECIMENTO RELEVANTE
→ preserva o fato que ela precisa continuar sabendo.
```

Outro exemplo:

```text
LIVRO
→ registra que houve um ferimento.

ESTADO ATUAL
→ preserva as marcas de Vida que ainda estão presentes.
```

Isso não é duplicação ruim porque cada fonte responde a uma pergunta diferente.

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

Isso inclui:

- fichas reais;
- relações consolidadas;
- conhecimento relevante;
- Estado Atual;
- Vida, Mente, Mana e condições atuais;
- acontecimentos;
- capítulos;
- mundo;
- processos;
- prazos;
- eventos futuros já estabelecidos;
- planos do Opositor;
- registros do Mestre.

Recursos permanentes pertencem à ficha; recursos temporários podem pertencer ao Estado Atual quando precisarem ser acompanhados.

## Regra final

> **Registro é a memória canônica da campanha. A ficha é a principal memória de interpretação da personagem; o Livro preserva o passado, o Estado preserva o presente e as demais fontes guardam contexto e processos externos. Salve somente o que foi legitimamente estabelecido e não faça uma personagem esquecer conhecimento já consolidado.**
