# Fontes da Campanha

Status: REFORMULAÇÃO / NÃO IMPLEMENTADO

Este arquivo define **onde salvar cada tipo de verdade** dentro de `campanhas/<nome>/`.

> **Cada verdade deve ter uma fonte principal.**

## Regra de roteamento

```text
QUEM É A PERSONAGEM E O QUE ELA PRECISA LEMBRAR PARA SER INTERPRETADA?
→ ficha da personagem.

SOBRE O QUE A CAMPANHA É E QUE DIREÇÃO O NARRADOR DEVE PRESERVAR?
→ mestre/roteiro.md.

COMO A CAMPANHA ESTÁ AGORA?
→ estado/atual.md.

O QUE É VERDADE ESTÁVEL NO CENÁRIO?
→ mundo/.

O QUE MAIS O MESTRE PRECISA PRESERVAR?
→ mestre/.

O QUE O OUTRO LADO DA TRAMA ESTÁ FAZENDO?
→ opositor/.

O QUE REALMENTE ACONTECEU?
→ livro/.
```

## `personagens/`

Guarda as fichas reais das personagens.

A ficha é a **principal fonte de interpretação** e pode conter:

- identidade;
- Estado inicial;
- Atributos e Perícias;
- Poderes e equipamentos;
- Traços;
- Recursos permanentes;
- personalidade e tendências;
- desejos, medos e hábitos;
- relações pelo ponto de vista do dono da ficha;
- conhecimento relevante;
- história consolidada que ainda influencia a personagem.

Não usar a ficha como diário completo de tudo que aconteceu.

## Conhecimento relevante da personagem

Informação que uma personagem precisa lembrar para interpretar, decidir ou reagir com continuidade deve ser consolidada em `Conhecimento relevante` na ficha quando isso for a forma mais direta de mantê-la disponível.

Regra prática:

```text
se esquecer provavelmente faria a personagem agir de forma incoerente
→ ficha / Conhecimento relevante.

se importa apenas para a situação presente
→ Estado Atual.

se é contexto externo amplo já guardado em outra fonte
→ consultar essa fonte quando necessário.
```

O que é relevante depende da campanha. Romance, terror, investigação ou outros focos podem tornar conhecimentos diferentes importantes.

Uma campanha ainda pode possuir arquivos adicionais de conhecimento quando o volume ou a organização justificar, mas eles não devem esconder da ficha uma informação essencial para interpretar a personagem corretamente.

O importante é preservar a separação:

```text
PERSONAGEM A SABE
≠
PERSONAGEM B SABE
```

Conhecimento consolidado não deve ser reapresentado como descoberta apenas porque a campanha foi retomada depois.

## Relações e ponto de vista

Relações registradas na ficha pertencem ao ponto de vista íntimo do dono daquela ficha.

```text
FICHA DE A
→ como A entende seus vínculos.

FICHA DE B
→ como B entende seus vínculos.
```

As duas leituras podem ser diferentes sem contradição.

O que A sabe sobre a percepção de B pode ser registrado em `Conhecimento relevante` de A quando isso realmente importar.

## `estado/atual.md`

Guarda o retrato operacional do presente.

Exemplos:

- local e momento atuais;
- quem está presente;
- marcas atuais de Vida e Mente;
- Mana atual;
- condições e efeitos ativos;
- posição importante;
- alterações temporárias de deslocamento;
- ação interrompida ou processo imediato;
- fatos recentes que ainda alteram diretamente as opções atuais.

Não é histórico.

A estrutura de Vida, Mente, Mana máxima normal e deslocamentos básicos vem da ficha. O Estado Atual acompanha somente como esses elementos estão agora.

## `mundo/`

Guarda verdades estáveis do cenário.

Exemplos:

- localização de uma cidade;
- regra política estabelecida;
- organização conhecida;
- característica permanente de um local;
- evento que alterou de forma duradoura o mundo.

Não usar para planos secretos ou condições temporárias de personagens.

## `mestre/`

Guarda informações operacionais próprias do Narrador quando a campanha realmente precisar delas.

### `mestre/roteiro.md`

É a fonte principal da **direção persistente da campanha**.

Pode registrar de forma curta:

```text
foco principal
trama de fundo
miniquests ou variações
tom e premissa
direção que o Narrador precisa preservar
```

O roteiro não determina acontecimentos nem resultados. Ele impede que uma trama secundária, improvisação ou mudança automática de tom substitua aquilo que a campanha foi criada para explorar.

```text
ROTEIRO
→ sobre o que a história é.

ESTADO
→ o que está acontecendo agora.

LIVRO
→ o que aconteceu.
```

A classificação operacional de NPCs ou criaturas (`ALIADO`, `NEUTRO`, `HOSTIL`, `INIMIGO`) pode aparecer no material do Mestre quando for útil, sempre relativa aos personagens principais e conforme `../mestre/julgamento.md`.

Outros arquivos de `mestre/` podem conter:

- referências de cena;
- fatos ocultos que não pertencem especificamente ao Opositor;
- material necessário para julgamento futuro.

Esses arquivos podem ser visíveis no repositório sem se tornarem conhecimento automático das personagens.

## `opositor/`

Guarda o outro lado da trama.

Pode conter:

- planos de vilões;
- objetivos adversariais;
- preparação;
- prazos;
- conhecimento de agentes adversariais;
- recursos legitimamente disponíveis;
- etapas futuras já julgadas como processos válidos.

Plano não é acontecimento.

```text
opositor/
→ preserva que o vilão pretende atacar em 5 dias.

livro/
→ só registra o ataque quando ele realmente acontecer.
```

## `livro/`

Guarda a história canônica do que efetivamente aconteceu.

O Livro não registra:

- intenção que não foi executada;
- hipótese descartada como se fosse verdade;
- plano futuro como se já tivesse ocorrido;
- metaconversa;
- discussão de regra;
- versões anuladas ou substituídas.

## Duplicação legítima

Uma mesma realidade pode aparecer em duas fontes quando cada uma possui função diferente.

```text
LIVRO
→ registra que Ravena descobriu um costume importante de Estelar.

FICHA DE RAVENA / CONHECIMENTO RELEVANTE
→ preserva aquilo que Raven agora sabe e deve considerar no futuro.
```

Outro exemplo:

```text
LIVRO
→ registra que Corvin foi ferido.

ESTADO ATUAL
→ preserva as marcas de Vida que ainda estão presentes.
```

O Livro preserva o acontecimento. A fonte operacional preserva aquilo que ainda precisa ser usado.

## Evitar cópia sem função

Não repetir por padrão:

- a cena inteira no Estado Atual;
- a ficha inteira no README;
- todos os segredos em vários arquivos;
- todo o Livro em Conhecimento relevante;
- toda a lore do mundo dentro de cada ficha;
- todo plano do Opositor em Estado Atual;
- o roteiro inteiro em vários arquivos.

Se uma informação já possui fonte principal suficiente, apontar para ela ou consultá-la quando necessário.

## Regra final

> **Escolha a fonte pela função da verdade: o roteiro guarda a direção da campanha; a ficha guarda quem a personagem é e o que precisa permanecer disponível para interpretá-la; Estado Atual guarda o presente; mundo guarda contexto estável; mestre e opositor guardam material operacional próprio; Livro guarda o que aconteceu.**
