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
- preparação, vantagem, contexto e oposição;
- resolução social;
- investigação e informação;
- combate e dano;
- energia, reservas e custos de uso;
- recuperação de VIDA;
- ações prolongadas e passagem de tempo quando houver resolução envolvida.

A ordem das declarações e o ciclo entre JOGADORES, OPOSITOR e NARRADOR pertencem a `../operacao/`.

## Arquivos aprovados nesta área

- `principio-de-resolucao.md` — distingue resultado evidente, impossibilidade evidente e incerteza real; somente a incerteza real exige resolução comparativa;
- `leitura-da-ficha-na-resolucao.md` — define como Atributos, Perícias, Poderes, meio, situação e conhecimento entram na resolução sem soma automática nem conversões fixas de patamar;
- `comparacao-e-disputa.md` — define comparação qualitativa, estratégia e preparação, soluções que mudam o problema, agência diante de planos e manutenção de disputas equilibradas sem vencedor artificial;
- `combate-e-dano.md` — define resolução compacta de combate, Perícia efetiva, Ataque efetivo, progressão exponencial de dano, defesa aplicável, ataques detalhados e referência de VIDA;
- `energia.md` — define Reserva, custo por patamar efetivamente usado, estados de Energia, Bateria e transferência de carga;
- `recuperacao-da-vida.md` — define recuperação natural por estado, tempos de referência e relação entre VIDA, dano acumulado e estabilização.

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

Em combate:

```text
Perícia efetiva = Perícia ofensiva − Perícia defensiva
Ataque efetivo = Dano + 1 + (Perícia efetiva × 0,2)
Dano aplicado = 2^(Ataque efetivo − Defesa efetiva)
```

Para Energia:

```text
Reserva [0] = 10
Reserva [1–5] = maior Atributo × 20
Custo = patamar efetivamente usado
Bateria [X] = X × 20
```

A cena continua decidindo quais capacidades realmente entram no cálculo.

> **Resolução não existe para fabricar incerteza nem para produzir um número único. Ela existe para decidir, pela ficção e pelas capacidades relevantes, qual resultado é coerente quando mais de um continua plausível.**

> **O NARRADOR preserva a continuidade da campanha, não a permanência dos problemas nem o planejamento anterior.**
