# Organização e Persistência de uma Aventura

Este documento ensina como transformar as regras universais de `sistema/` em uma aventura concreta que possa ser retomada por outro chat ou outra IA sem depender de memória anterior.

## Estrutura recomendada

Cada campanha deve ficar em uma pasta própria:

```text
aventuras/<nome-da-aventura>/
├── README.md
├── diretrizes/
├── personagens/
├── mundo/
├── relacionamento/
├── cronologia/
├── estado/
│   └── atual.md
└── livro/
```

## Função de cada pasta

### `README.md`
É a porta de entrada da aventura.

Deve informar:
- premissa;
- protagonistas ou personagens centrais;
- ponto atual da campanha;
- hierarquia de cânone;
- quais diretrizes devem ser lidas antes de narrar;
- onde está o estado atual.

### `diretrizes/`
Define **como aquela aventura deve ser narrada**.

Pode conter:
- tom;
- ritmo;
- pessoa/ponto de vista;
- tamanho médio das cenas;
- comandos especiais do jogador;
- regras de conversão para livro;
- limites ou escolhas estilísticas.

Essas diretrizes pertencem à aventura e **não** ao sistema universal.

### `personagens/`
Contém as fichas estáveis de personagens Centrais e Relevantes.

A ficha responde principalmente:
- quem é;
- como costuma agir;
- quais capacidades possui;
- quais relações duradouras possui.

Ferimentos, cansaço e condições temporárias não pertencem à ficha permanente.

### `mundo/`
Contém regras e fatos específicos do cenário:
- lugares;
- organizações;
- cosmologia;
- regras sobrenaturais locais;
- tecnologia;
- limitações específicas;
- fatos que personagens podem descobrir.

Uma regra específica do mundo não deve ser promovida automaticamente a regra universal do sistema.

### `relacionamento/`
Usar para vínculos Centrais ou complexos que precisem de mais contexto do que um valor `REL` consegue representar.

O arquivo pode registrar:
- natureza do vínculo;
- evolução;
- desejos conflitantes;
- limites;
- acontecimentos que mudaram a relação;
- trajetórias planejadas, sempre separando plano de fato ocorrido.

### `cronologia/`
Índice rápido do que aconteceu.

Para cada acontecimento relevante, registrar quando possível:
- capítulo;
- dia/período relativo;
- local;
- personagens presentes;
- fato;
- consequência;
- informação que cada personagem passou a conhecer.

A cronologia ajuda o narrador a evitar conhecimento impossível e contradições de continuidade.

### `estado/atual.md`
É o **savegame operacional** da aventura.

Ele não substitui fichas nem capítulos. Guarda apenas como as coisas estão no momento exato em que a história parou.

Para personagens Centrais e Relevantes, pode registrar:
- VIDA atual;
- ENERGIA atual;
- CONDIÇÕES;
- danos temporários de equipamento;
- efeitos ativos;
- localização;
- situação imediata.

Exemplo:

```text
## Peter Parker
VIDA: Ferido
ENERGIA: Metade
COND: costela machucada
Local: telhado do laboratório
Efeito ativo: nenhum
```

### `livro/`
Contém o registro canônico consolidado do que realmente aconteceu, em capítulos ou outra forma narrativa definida pelas diretrizes da aventura.

O material jogado é matéria-prima; o capítulo consolidado é o registro principal dos fatos quando a aventura adotar esse modelo.

## FICHA x STATUS

### FICHA
É memória de longo prazo.

Guarda características relativamente estáveis:
- identidade;
- descrição e personalidade;
- atributos;
- perícias;
- poderes;
- equipamento recorrente importante;
- relações.

### STATUS
É memória de curto prazo.

Guarda:
- Vida;
- Energia;
- Condições;
- efeitos temporários;
- danos temporários;
- situação imediata.

> **Ficha = quem o personagem é. Status = como ele está agora.**

## Quando mostrar STATUS ao jogador

O narrador deve mostrar/atualizar STATUS:
- quando houver mudança importante de Vida;
- quando Energia mudar de faixa;
- quando surgir ou desaparecer uma condição relevante;
- quando uma consequência temporária mudar substancialmente as opções do personagem;
- sempre que o jogador pedir `status, narrador` ou equivalente.

Não repetir STATUS a cada ação se nada importante mudou.

Para Figurantes, normalmente basta acompanhar narrativamente enquanto permanecerem na cena; não é necessário persistir cada detalhe.

## Quando alterar a ficha permanente

Não reescrever fichas por mudanças passageiras.

Alterações permanentes podem ser registradas quando a história realmente as produz, especialmente:
- mudança relevante de `REL`;
- aquisição/perda permanente de poder;
- aprendizado relevante de perícia;
- transformação corporal permanente;
- mudança estrutural de identidade ou personalidade sustentada por acontecimentos.

Uma relação direcional deve ser alterada somente na ficha de quem mudou.

## Fechamento de capítulo

Ao encerrar um capítulo ou bloco canônico:

1. Consolidar em `livro/` somente os acontecimentos realmente válidos.
2. Remover comandos, correções fora da história, tentativas descartadas e versões substituídas.
3. Atualizar `cronologia/` com fatos e conhecimentos relevantes.
4. Atualizar fichas apenas com mudanças duradouras.
5. Atualizar arquivos de `relacionamento/` quando houver evolução complexa importante.
6. Sobrescrever `estado/atual.md` com o ponto exato de continuação.
7. Remover do STATUS condições que já terminaram.

## Hierarquia de cânone

Cada aventura deve definir sua própria hierarquia no `README.md`.

Como padrão recomendado:

1. correção explícita mais recente do usuário;
2. capítulos consolidados em `livro/`;
3. diretrizes canônicas da aventura;
4. personagens, mundo e relacionamentos consolidados;
5. cronologia;
6. `estado/atual.md` para o estado operacional presente;
7. material antigo ou rascunho apenas como referência.

`estado/atual.md` é autoridade sobre o **agora**, mas não pode contradizer um fato canônico sem que exista um acontecimento posterior que explique a mudança.

## Continuação em outro chat

Para retomar uma campanha sem contexto anterior:

1. ler o sistema universal;
2. ler o `README.md` da aventura;
3. ler as diretrizes indicadas;
4. ler as fichas dos personagens presentes ou centrais;
5. consultar relações e mundo relevantes;
6. ler a cronologia suficiente para entender a situação;
7. ler `estado/atual.md`;
8. consultar o último capítulo consolidado quando necessário;
9. só então continuar a narrativa.

> **Nunca depender de “lembrar da conversa anterior” quando os arquivos da aventura existem.**
