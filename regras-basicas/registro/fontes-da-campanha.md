# Fontes da Campanha

Status: REFORMULAÇÃO / NÃO IMPLEMENTADO

Este arquivo define **onde salvar cada tipo de verdade** dentro de `campanhas/<nome>/`.

> **Cada verdade deve ter uma fonte principal.**

## Regra de roteamento

```text
QUEM É A PERSONAGEM?
→ personagens/

O QUE ELA SABE?
→ personagem / arquivo de conhecimento apropriado

COMO A CAMPANHA ESTÁ AGORA?
→ estado/atual.md

O QUE É VERDADE ESTÁVEL NO CENÁRIO?
→ mundo/

O QUE O MESTRE PRECISA PRESERVAR?
→ mestre/

O QUE O OUTRO LADO DA TRAMA ESTÁ FAZENDO?
→ opositor/

O QUE REALMENTE ACONTECEU?
→ livro/
```

## `personagens/`

Guarda dados persistentes das personagens.

Pode incluir:

- ficha;
- personalidade;
- relações estáveis;
- capacidades;
- recursos permanentes;
- conhecimentos persistentes quando a campanha optar por separá-los por personagem.

Não usar a ficha como diário completo de tudo que aconteceu.

## Conhecimento da personagem

Informação que uma personagem pode usar em decisões futuras precisa estar disponível em uma fonte legítima dela quando não puder depender apenas da cena atual.

Exemplos:

```text
Ravena descobriu que a mansão possui proteção contra demônios.

Corvin descobriu o verdadeiro nome do ritual.

Dick recebeu informação de que Ravena foi vista em outra cidade.
```

A forma exata pode variar por campanha:

```text
personagens/<nome>/conhecimento.md
```

ou outra fonte claramente indicada no README da campanha.

O importante é preservar a separação:

```text
PERSONAGEM A SABE
≠
PERSONAGEM B SABE
```

## `estado/atual.md`

Guarda o retrato operacional do presente.

Exemplos:

- local e momento atuais;
- quem está presente;
- Vida e Mana atuais quando relevantes;
- condições e efeitos ativos;
- posição importante;
- ação interrompida ou processo imediato;
- fatos recentes que ainda alteram diretamente as opções atuais.

Não é histórico.

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

Pode conter:

- direção narrativa local;
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

Exemplo:

```text
LIVRO
→ registra que Corvin foi envenenado durante o jantar.

ESTADO ATUAL
→ Envenenado | efeito ainda ativo.
```

Outro exemplo:

```text
LIVRO
→ Ravena descobriu o nome do culto.

CONHECIMENTO DE RAVENA
→ nome do culto: Ordem de X.
```

O Livro preserva o acontecimento.

A fonte operacional preserva aquilo que ainda precisa ser usado.

## Evitar cópia sem função

Não repetir por padrão:

- a cena inteira no estado atual;
- a ficha inteira no README;
- todos os segredos em vários arquivos;
- todos os fatos do Livro em conhecimento;
- todo plano do Opositor em estado atual.

Se uma informação já possui fonte principal suficiente, apontar para ela ou consultá-la quando necessário.

## Regra final

> **Escolha a fonte pela função da verdade: personagens guardam quem são e o que sabem; estado guarda o presente; mundo guarda verdades estáveis; mestre guarda material operacional do Narrador; opositor guarda o outro lado da trama; Livro guarda o que aconteceu.**