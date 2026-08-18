# Exemplo Prático — O Farol Partido

> **REFERÊNCIA DE SISTEMA. NÃO É UMA CAMPANHA ATIVA.**

Esta pasta mostra, em escala mínima, como uma campanha pronta pode ficar depois da criação, de uma primeira sessão e do fechamento de um capítulo.

Ela existe para consulta estrutural e operacional. Não deve aparecer na lista de campanhas em `aventuras/` e nunca deve ser continuada como jogo real, salvo se o usuário pedir explicitamente para transformá-la em campanha.

## Comando de consulta

Quando o usuário escrever:

```text
CONSULTAR EXEMPLO PRÁTICO
```

o narrador ou IA deve usar esta pasta como referência de aplicação do sistema.

Ordem recomendada:

1. `criacao.md` — como a criação concluída fica registrada;
2. `mundo/cenario.md` — cenário consolidado;
3. `personagens/nara-vale.md` — personagem Central;
4. `personagens/tomas-ribeiro.md` — personagem Relevante;
5. `estado/inicio.md` — ponto inicial antes do jogo;
6. `livro/capitulo-01.md` — o que efetivamente aconteceu;
7. `cronologia/cronologia.md` — índice factual e conhecimento;
8. `progressao/atual.md` — consequências ainda causalmente vivas;
9. `estado/atual.md` — savegame operacional depois do capítulo.

## Premissa

Na vila costeira de Brumal, um farol abandonado voltou a emitir luz durante tempestades. Nara Vale, uma taumaturga que trabalha resolvendo ocorrências sobrenaturais, aceita investigar o local ao lado de Tomas Ribeiro, guarda da vila.

## O que este exemplo demonstra

- conceito antes da mecânica;
- ficha Central e ficha Relevante;
- uso de `TRAÇOS`;
- diferença entre ficha permanente e STATUS;
- `estado/inicio.md` separado de `estado/atual.md`;
- capítulo consolidado como registro canônico;
- cronologia como índice do que aconteceu;
- Progressão como memória do que ainda pode voltar a importar;
- relações recorrentes na ficha sem transformar `REL` em histórico completo.

## Hierarquia interna do exemplo

1. capítulo consolidado em `livro/`;
2. personagens e mundo consolidados;
3. Progressão vigente;
4. cronologia;
5. `estado/atual.md` para o agora;
6. `estado/inicio.md` apenas como referência do ponto de partida;
7. `criacao.md` como registro do processo concluído.

> **Consultar para entender o formato. Não copiar detalhes ficcionais para outra campanha sem motivo.**
