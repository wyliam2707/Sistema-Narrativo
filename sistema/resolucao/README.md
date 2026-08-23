# Resolução

Status: BASE PRINCIPAL EM USO

Esta pasta reúne as regras que respondem à pergunta:

> **Dadas as intenções, capacidades, circunstâncias e movimento do cenário, como descobrimos o que acontece?**

A definição estável dos personagens pertence a `../personagem/`. STATUS e demais verdades persistentes pertencem a `../persistencia/`. A ordem das declarações e o ciclo entre JOGADORES, OPOSITOR e NARRADOR pertencem a `../operacao/`.

## Responsabilidades desta área

Esta pasta concentra:

- intenção versus resultado;
- quando um resultado é evidente e quando exige resolução;
- leitura qualitativa de atributos, perícias e poderes;
- comparação de capacidades e manutenção de disputas equilibradas;
- motor geral de disputas progressivas contra personagens e cenário;
- escalas de efeito, exigência, consolidação e proteção;
- preparação, contexto e oposição;
- resolução social;
- investigação e informação;
- combate e dano;
- energia, reservas e custos de uso;
- recuperação de VIDA, Regeneração, Cura e Medicina;
- contenção sustentada por agentes;
- efeitos persistentes, Defesa/Vida e Dissipar;
- ações prolongadas e passagem de tempo quando houver resolução envolvida.

## Arquivos principais

- `principio-de-resolucao.md` — resultado evidente, impossibilidade evidente e incerteza real;
- `leitura-da-ficha-na-resolucao.md` — como Atributos, Perícias, Poderes, meio, situação e conhecimento entram sem soma automática;
- `comparacao-e-disputa.md` — comparação qualitativa, estratégia, preparação, soluções válidas e disputas equilibradas;
- `motor-de-disputa.md` — Potência, Resistência, Exigência, progresso, tempo, custo, contenção sustentada e integração com Consolidação;
- `escalas-de-efeito.md` — tabelas e manifestações-base dos efeitos;
- `consolidacao.md` — Alcance, Alvos, Área/Tamanho, Duração, limite de Ampliação, custo exato e estrutura de efeitos persistentes;
- `combate-e-dano.md` — fonte de Dano, Perícia efetiva, Ataque efetivo, Dano aplicado e defesa aplicável;
- `energia.md` — Reserva, custos, Ampliação, Bateria e recuperação;
- `recuperacao-da-vida.md` — recuperação natural, Regeneração, Cura e Medicina;
- `resolucao-social.md` — influência social sem Defesa Social universal e com preservação de agência;
- `informacao-e-investigacao.md` — existência, acesso, percepção, interpretação, hipótese, investigação e confirmação, separando investigação normal do efeito especial Informação.

## Regra de migração

A pasta `resolucao/` é a referência atual para os temas que já foram consolidados aqui.

Alguns documentos históricos ainda existem em outras áreas enquanto houver conteúdo não migrado. Arquivos antigos já substituídos e removidos não são fontes válidas e não devem ser procurados.

O registro das substituições e remoções fica em `../MIGRACAO-ESTRUTURAL.md`.

Quando uma formulação histórica ainda existente contradiz uma regra já aprovada nesta pasta ou em `../personagem/`, prevalece a formulação nova e explicitamente aprovada.

## Princípio de entrada

```text
RESULTADO EVIDENTE → estabelece
IMPOSSIBILIDADE EVIDENTE → estabelece
INCERTEZA REAL → resolve
```

A resolução não fabrica dúvida quando o resultado já está claro.

Quando houver incerteza:

```text
A cena determina quais capacidades importam.
Atributos, Perícias e Poderes não se somam automaticamente.
Patamares são qualitativos e não lineares.
Contexto altera a situação, não cria bônus obrigatório.
Mesmo aspecto pode ser comparado diretamente.
Aspectos diferentes são interpretados em suas funções próprias.
Preparação cria condições, não bônus.
Uma solução válida pode encerrar um problema importante.
Uma disputa equilibrada pode continuar sem vencedor artificial.
```

## Motor geral

Quando Perícias dos dois lados realmente participam:

`Perícia efetiva = Perícia de aplicação − Perícia de oposição`

O Efetivo geral é:

`Efeito efetivo = Potência usada + 1 + (Perícia efetiva × 0,2)`

O Resultado/Progresso é:

`Progresso por aplicação = 2^(Efeito efetivo − Resistência efetiva)`

Quando a tarefa permite acúmulo:

`Aplicações necessárias = teto(Exigência ÷ Progresso por aplicação)`

Escalas padrão de aplicação:

`6 segundos → imediata | 1 minuto → curta | 1 hora → prolongada | 1 dia → extensa`

## Ampliação e Energia

Cada efeito possui uma manifestação-base. Ampliar acima dela acrescenta carga nas dimensões aplicáveis.

Dimensões gerais:

`Alcance | Alvos | Área/Tamanho | Duração`

Cada passo aprovado acima da base gera `+1` de Ampliação. Regras específicas podem adicionar uma dimensão própria, como quantidade de STATUS em Dissipar.

Cada efeito possui limite:

`Ampliação [X] = patamar máximo do efeito + maior entre MEN e VON`

O custo é sempre exato:

`Custo = patamar efetivamente usado + Ampliação usada`

**Não existe pagamento parcial de Ampliação nem redução de Efetivo por falta de pagamento.** Se o JOGADOR não possui Energia suficiente ou quer gastar menos, reduz a potência usada, a Ampliação ou ambas antes da resolução.

Reserva própria:

`maior Atributo [0] → 10 | [1] → 20 | [2] → 40 | [3] → 60 | [4] → 80 | [5] → 100`

Bateria:

`Bateria [1] → 20 | [2] → 40 | [3] → 60 | [4] → 80 | [5] → 100`

## Combate e Dano

`FIS` pode ser a fonte de potência de um golpe corporal. Uma arma ou Poder que possua `Dano [X]` usa seu próprio valor. As fontes não se somam automaticamente.

Exemplo: `FIS [2] | Pistola Dano [1] | Espada Mágica Dano [3]`.

Quando técnica ofensiva e defensiva participam:

`Perícia efetiva = Perícia ofensiva − Perícia defensiva`

`Ataque efetivo = Dano + 1 + (Perícia efetiva × 0,2)`

`Dano aplicado = 2^(Ataque efetivo − Defesa efetiva)`

`Dano mínimo contabilizável = 0,25`, salvo quando o próprio mecanismo é incapaz de afetar o alvo.

## Cura

`Cura efetiva = Cura usada + 1 + (Perícia aplicável × 0,2)`

`Cura aplicada = máx(1, 2^(Cura efetiva − RES do alvo))`

A configuração ampliada é paga integralmente antes da resolução.

## Efeitos persistentes

Todo efeito persistente consolidado, benéfico ou prejudicial, possui estrutura:

`Efeito [D x / V5] — Duração`

`D` é a Defesa estrutural, normalmente o Efetivo que estabeleceu o efeito. `V5` é um grau de Vida.

Perder Vida **não reduz a intensidade** do efeito. Enquanto `V > 0`, ele permanece com o Resultado estabelecido. Em `V0`, termina.

Referência estrutural:

`Efeito persistente → V5 | Proteção/Barreira → V5 | Invocação → V10 | Personagem → V35`

`Dissipar` é um efeito separado que causa Dano sobre a Vida de STATUS persistentes:

`Dissipar efetivo vs D do STATUS → Dano aplicado → reduz V`

Quantidade própria de STATUS para Dissipar:

`1 +0 | 2 +1 | 4 +2 | 6 +3 | 16 +4 | 32 +5`

## Contenção

Uma contenção criada por efeito persistente usa sua estrutura `D/V5`.

Uma contenção realizada por personagem, criatura ou Invocação ativa é **Sustentada**: depende do agente continuar gastando sua ação e não cria automaticamente `D/V` próprio.

Vários agentes não somam Atributos; quando realizam a mesma contenção coordenada na mesma janela, seus **Resultados compatíveis podem ser somados**.

Uma estrutura física aplicada depois, como algemas, continua existindo por conta própria e usa sua estrutura correspondente, por exemplo `Algemas → FIS [3] | V10`.

## Princípios finais

> **Resolução não existe para fabricar incerteza. Ela decide o que acontece quando mais de um resultado continua realmente plausível.**

> **A Resistência transforma dificuldade em tempo, custo e oportunidade de reação.**

> **O plano não vence o patamar. O plano muda o problema.**

> **O NARRADOR preserva a continuidade da campanha, não a permanência dos problemas nem o planejamento anterior.**
