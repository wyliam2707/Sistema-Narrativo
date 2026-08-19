# Criação da Campanha

Status geral: CONCLUÍDA

1. Direção narrativa e cenário: APROVADO
   - Diretrizes narrativas: APROVADO
   - Cenário: APROVADO
2. Protagonista: APROVADO
3. Personagens relevantes: APROVADO
4. Início da história: APROVADO

Revisão final: CONCLUÍDA

## Correções já incorporadas ao sistema

- Durante a criação conceitual dos aliados, pode bastar definir apenas a quantidade e os nomes. As fichas estruturais podem ser criadas imediatamente com os campos ainda desconhecidos em branco, para desenvolvimento posterior durante a revisão.
- Inimigos comuns não precisam de ficha persistente. O narrador usa apenas o modelo rápido e as exceções necessárias à cena.
- Antagonistas importantes, recorrentes ou poderosos podem receber ficha completa quando passarem a importar. Se a ficha precisar permanecer oculta do jogador, ela deve ficar em `mestre/viloes/` e ser tratada como material reservado ao narrador.
- Fichas reservadas de antagonistas não passam pela aprovação aberta do jogador, mas devem ser definidas de forma coerente e não podem ser alteradas retroativamente apenas para contrariar soluções válidas ou recuperar dificuldade.
- Lúcio Marco poderá ser desenvolvido futuramente em `mestre/viloes/` quando passar a importar diretamente na campanha.
- O personagem com `CONTROLE: JOGADOR HUMANO` deve ser revisado com controle fino: campos simples são apresentados individualmente e confirmados antes do próximo; ATRIBUTOS, PERÍCIAS e PODERES são três blocos próprios. Ao final, a ficha completa é apresentada para aprovação final.
- Os demais personagens apresentáveis ao jogador são revisados em quatro blocos: 1) identidade e conceito; 2) capacidades; 3) recursos; 4) interpretação. Cada bloco precisa ser aprovado antes do seguinte, e a ficha completa é apresentada no final.
- O início aprovado da história deve ser armazenado em `estado/inicio.md`. Esse arquivo preserva o ponto de partida aprovado da campanha e não deve ser sobrescrito conforme a história avança; `estado/atual.md` continua sendo o savegame operacional mutável. O exemplo foi corrigido para seguir esse padrão.
- Toda campanha deve criar, junto com sua estrutura inicial, um `README.md` curto em cada pasta estrutural. Esses arquivos materializam as pastas no Git, explicam sua finalidade para outras IAs e permanecem como legenda da organização mesmo depois que a pasta recebe conteúdo real. O protocolo, a organização de aventura e os modelos foram atualizados para tornar isso padrão.
- Falas e pensamentos foram padronizados. Toda fala direta usa `[Personagem] — fala`. Durante o RPG ao vivo, pensamento explícito aparece somente para personagem com `CONTROLE: JOGADOR HUMANO`, quando declarado ou autorizado pelo jogador humano, e usa `[Personagem, pensa] — pensamento`; pensamentos de `NPC`, `JOGADOR IA` e `JOGADOR EVENTUAL IA` permanecem ocultos ao jogador humano por padrão e são percebidos apenas por sinais da ficção. No livro consolidado, pensamentos de qualquer personagem podem aparecer nesse mesmo formato quando forem coerentes com a cena e não alterarem o cânone. O Capítulo 1 foi corrigido para identificar todas as falas.
- A Etapa 1 da criação foi ampliada para `Direção narrativa e Cenário`. Primeiro se define que tipo de história o jogador quer viver — gênero ou combinação, tom, foco, ritmo, humor, romance/intimidade, atmosfera e demais escolhas que realmente importarem — e isso é salvo em `diretrizes/narracao.md`. Separadamente, `mundo/cenario.md` guarda apenas a realidade do mundo. O Faroeste Arcano foi reorganizado para servir de exemplo dessa separação.

## Pendências para revisão

Nenhuma pendência metodológica registrada neste exemplo.

## Ajuste posterior de controle

Após a conclusão da criação, o sistema passou a registrar explicitamente quem possui o ciclo de decisão de cada personagem.

Controle atual aprovado:

- Dik Vigarista — JOGADOR HUMANO
- Adan Stanfor — JOGADOR EVENTUAL IA
- Lucia James — JOGADOR EVENTUAL IA

Este ajuste não altera conceito, mecânica, história ou relações dos personagens.
