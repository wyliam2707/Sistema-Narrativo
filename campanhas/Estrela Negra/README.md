# Estrela Negra

STATUS: PRONTO PARA JOGAR
Temporada atual: 1

## Identidade

A narrativa da campanha está em `mestre/narrativa.md`.
O roteiro da primeira temporada está em `mestre/roteiro.md`.
O ponto exato de início / retomada está em `estado/atual.md`.

## Elenco protagonista inicial

- `personagens/Corvin Blackwood.md` — protagonista controlado pelo jogador.
- `personagens/Ravena.md` — protagonista controlada pela IA.
- `personagens/Estelar.md` — protagonista controlada pela IA.

A primeira temporada usa somente esses três como núcleo protagonista presente.

## Retomada em nova conversa

Ao iniciar uma nova sessão, a IA deve ler primeiro:

1. `estado/atual.md`
2. `mestre/narrativa.md`
3. `mestre/roteiro.md`
4. as fichas de Corvin Blackwood, Ravena e Estelar

Depois deve começar exatamente no ponto indicado em `estado/atual.md`, sem depender de memória de conversas anteriores.

O início absoluto é Corvin chegando à região um dia antes de Ravena e Estelar, após perceber energia estranha e luzes de uma cidade que não constava nas informações que tinha sobre a área.
