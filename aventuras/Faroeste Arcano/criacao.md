# Criação da Campanha

Status geral: CONCLUÍDA

1. Cenário: APROVADO
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

## Pendências para revisão

- Revisar o método de fichas para oficializar uma revisão em quatro blocos: 1) identidade e conceito; 2) capacidades; 3) recursos; 4) interpretação. O narrador pode propor uma base em cada bloco, mas deve apresentar, ajustar e obter aprovação do jogador antes de avançar. A ficha completa só deve ser consolidada e salva como APROVADO depois dos quatro blocos revisados.
- Padronizar no protocolo onde o início aprovado da história deve ser armazenado. Neste exemplo ele foi consolidado em `mundo/inicio-da-historia.md`, enquanto o protocolo atual indica `estado/inicio.md`.
- Revisar o protocolo para que cada pasta estrutural da campanha seja criada desde o início com um `README.md` curto explicando sua finalidade. Isso preserva a estrutura no Git, que não mantém diretórios vazios, e permite que outra IA entenda rapidamente para que cada pasta serve.
- Padronizar falas e pensamentos. Durante o RPG ao vivo, usar `[Personagem] — fala`; pensamentos explícitos devem aparecer apenas para o personagem controlado pelo jogador, no formato `[Personagem, pensa] — pensamento`, sem revelar pensamentos internos dos NPCs. No livro consolidado, falas continuam identificadas e pensamentos de qualquer personagem podem aparecer no formato `[Personagem, pensa] — pensamento` quando fizer sentido para a cena. O Capítulo 1 deste exemplo precisa ser ajustado para esse padrão antes da versão final do exemplo.
