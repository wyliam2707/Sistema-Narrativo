# Resolução

Esta pasta reúne as regras que respondem à pergunta:

> **Dadas as intenções, capacidades, circunstâncias e movimento do cenário, como descobrimos o que acontece?**

## Estado da migração

A estrutura nova está sendo construída sem apagar os arquivos antigos.

Enquanto uma regra ainda não tiver sido reescrita e aprovada nesta pasta, o arquivo antigo correspondente em `sistema/` continua válido como fonte de migração.

## Responsabilidades desta área

Esta pasta deverá concentrar, progressivamente:

- intenção versus resultado;
- quando um resultado é evidente e quando exige resolução;
- leitura qualitativa de atributos, perícias e poderes;
- comparação de capacidades e manutenção de disputas equilibradas;
- motor geral de disputas progressivas contra personagens e cenário;
- escalas de efeito, exigência, consolidação e proteção;
- preparação, vantagem, contexto e oposição;
- resolução social;
- investigação e informação;
- combate e dano;
- energia, reservas e custos de uso;
- recuperação de VIDA, Regeneração, Cura e Medicina;
- ações prolongadas e passagem de tempo quando houver resolução envolvida.

A ordem das declarações e o ciclo entre JOGADORES, OPOSITOR e NARRADOR pertencem a `../operacao/`.

## Arquivos aprovados nesta área

- `principio-de-resolucao.md` — distingue resultado evidente, impossibilidade evidente e incerteza real; somente a incerteza real exige resolução comparativa;
- `leitura-da-ficha-na-resolucao.md` — define como Atributos, Perícias, Poderes, meio, situação e conhecimento entram na resolução sem soma automática nem conversões fixas de patamar;
- `comparacao-e-disputa.md` — define comparação qualitativa, estratégia e preparação, soluções que mudam o problema, agência diante de planos e manutenção de disputas equilibradas sem vencedor artificial;
- `motor-de-disputa.md` — define Potência, Resistência, Exigência, progresso por aplicação, acumulação, tempo, custo efetivo, oportunidade de reação e integração com Consolidação;
- `escalas-de-efeito.md` — reúne as tabelas de efeitos aprovadas, incluindo Sentidos, Controle, Mobilidade, Supressão, Proteção, Informação, Invocação, Transformação, Sono, Ilusão, Emoção e Deslocar;
- `consolidacao.md` — define manifestação-base, Alcance, Alvos, Área/Tamanho, Duração, carga de ampliação, custo em Energia, redução de Efeito efetivo e remoção de efeitos persistentes; permanece em revisão enquanto os pontos finais são calibrados;
- `combate-e-dano.md` — define resolução compacta de combate, Perícia efetiva, Ataque efetivo, progressão exponencial de dano, dano mínimo contabilizável, defesa aplicável, ataques detalhados e referência de VIDA;
- `energia.md` — define Reserva, custo-base por patamar efetivamente usado, carga de ampliação, estados de Energia, Bateria, recuperação e transferência de carga;
- `recuperacao-da-vida.md` — define recuperação natural por estado, Regeneração por hora, Cura como contraponto do Dano, Medicina sem oposição artificial e estabilização;
- `resolucao-social.md` — define resolução social sem Defesa Social universal, preservação de agência, função contextual de VON, Relações, autoridade, intimidação, enganação e resultados sociais abertos.

## Arquivos antigos ainda como fonte de migração

- `../ciclo-de-jogadores.md` — fonte histórica do ciclo; a nova arquitetura operacional está em `../operacao/ciclo-de-cena.md`;
- `../README.md` — base mecânica geral, atributos, perícias, poderes e princípios antigos de resolução.

## Regra de migração

Não copiar mecanicamente uma regra antiga apenas para mudar seu endereço.

Quando um tema for revisado:

1. consultar o arquivo antigo;
2. usar exemplos reais das campanhas quando ajudarem;
3. escrever a nova versão nesta pasta;
4. indicar na nova estrutura o que passou a substituir a formulação antiga;
5. manter os arquivos antigos como fonte até que sua migração esteja concluída.

## Princípios

```text
RESULTADO EVIDENTE
→ estabelece.

IMPOSSIBILIDADE EVIDENTE
→ estabelece.

INCERTEZA REAL
→ resolve.
```

Quando houver incerteza:

```text
A cena determina quais capacidades importam.
Atributos, Perícias e Poderes não se somam.
Patamares são qualitativos, não conversões fixas.
Contexto altera a situação, não cria bônus obrigatório.
Mesmo aspecto pode ser comparado diretamente.
Aspectos diferentes são interpretados em suas funções próprias.
Preparação cria condições, não bônus.
Uma solução válida pode encerrar um problema importante.
Uma disputa equilibrada pode continuar sem vencedor.
```

Para disputas progressivas:

```text
Perícia efetiva = Perícia de aplicação − Perícia de oposição
Efeito efetivo = Potência usada + 1 + (Perícia efetiva × 0,2) − Ampliação não paga
Progresso por aplicação = 2^(Efeito efetivo − Resistência efetiva)
Aplicações necessárias = teto(Exigência ÷ Progresso por aplicação)
```

Escalas padrão de aplicação:

`6 segundos → imediata` | `1 minuto → curta` | `1 hora → prolongada` | `1 dia → extensa`

Quando houver Energia, o custo-base é o patamar usado. Ampliações podem acrescentar carga. O JOGADOR escolhe quanto dessa carga paga em Energia; cada ponto não pago reduz o Efeito efetivo em `1` naquela aplicação.

A Consolidação parte da manifestação-base `[0]` e amplia, quando necessário:

`Alcance` | `Alvos` | `Área/Tamanho` | `Duração`

Em efeitos persistentes, a Duração determina quando terminam naturalmente. Tentativas de remoção reduzem sua Consolidação; o efeito permanece inteiro até a Consolidação chegar a zero.

Em combate:

```text
Perícia efetiva = Perícia ofensiva − Perícia defensiva
Ataque efetivo = Dano + 1 + (Perícia efetiva × 0,2) − Ampliação não paga
Dano aplicado = 2^(Ataque efetivo − Defesa efetiva)
Dano mínimo contabilizável = 0,25
```

Para Energia:

```text
Reserva [0] = 10
Reserva [1–5] = maior Atributo × 20
Custo-base = patamar efetivamente usado
Ampliação [2]/[4]/[8]/[16] = carga +1/+2/+3/+4
Bateria [X] = X × 20
```

Para Cura:

```text
Cura efetiva = Cura usada + 1 + (Perícia aplicável × 0,2) − Ampliação não paga
Cura aplicada = máx(1, 2^(Cura efetiva − RES do alvo))
```

A cena continua decidindo quais capacidades realmente entram no cálculo.

> **Resolução não existe para fabricar incerteza nem para produzir um número único. Ela existe para decidir, pela ficção e pelas capacidades relevantes, qual resultado é coerente quando mais de um continua plausível.**

> **A Resistência transforma dificuldade em tempo, custo e oportunidade de reação.**

> **O NARRADOR preserva a continuidade da campanha, não a permanência dos problemas nem o planejamento anterior.**
