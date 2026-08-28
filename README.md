# Sistema Narrativo

Este repositório separa **as regras universais do RPG** dos **dados concretos de cada campanha**.

## Estrutura atual

```text
regras-basicas/
→ única fonte canônica das regras atuais.

campanhas/
→ campanhas, fichas, estado, mundo, material do Mestre, Opositor e Livro.
```

> **Regra fica em `regras-basicas/`. Verdade da mesa fica em `campanhas/<nome>/`.**

A antiga árvore `sistema/` foi aposentada depois da consolidação funcional. Ela não é mais fonte de regra nem dependência do motor atual.

## Como entrar

```text
NOVA CAMPANHA
→ regras-basicas/CRIACAO-DE-CAMPANHA.md

NOVA TEMPORADA
→ regras-basicas/CRIACAO-DE-TEMPORADA.md

COMEÇAR OU CONTINUAR CAMPANHA
→ regras-basicas/INICIO-E-RETOMADA.md
```

Para entender a arquitetura atual, começar por:

```text
regras-basicas/README.md
```

Não é necessário reler toda a árvore de regras antes de cada ação. Carregar o núcleo operacional e consultar especialidades quando a situação realmente exigir.

## Execução por uma única IA

Uma única IA técnica pode executar várias cadeiras desde que preserve autoridade e conhecimento separados.

```text
JOGADOR HUMANO
JOGADOR IA
JOGADOR IA EVENTUAL
OPOSITOR
NARRADOR
```

As regras de autoridade, autonomia, conhecimento e execução estão em:

```text
regras-basicas/nucleo/
```

A IA técnica poder acessar uma informação não significa que determinada personagem possa usá-la.

## Fonte da campanha

Para uma campanha concreta:

```text
campanhas/<nome>/README.md
→ identidade e roteamento.

campanhas/<nome>/personagens/
→ fichas.

campanhas/<nome>/estado/atual.md
→ presente necessário para retomar.

campanhas/<nome>/mundo/
→ verdades estáveis do cenário.

campanhas/<nome>/mestre/
→ narrativa, roteiro e material reservado.

campanhas/<nome>/opositor/
→ planos, processos e informações adversariais quando existirem.

campanhas/<nome>/livro/
→ histórico consolidado.
```

Não pedir novamente ao jogador informação que já esteja registrada em fonte canônica suficiente.

## Prioridade das fontes

Quando houver conflito real:

```text
correção explícita mais recente do JOGADOR HUMANO
→ prevalece depois de canonizada.

regra universal atual
→ regras-basicas/.

fato concreto da campanha
→ fonte canônica pertinente em campanhas/<nome>/.

memória, resumo ou modelo mental da IA
→ cache operacional; nunca prevalece sobre os arquivos atuais.
```

Correções e mudanças permanentes seguem:

```text
regras-basicas/registro/canonizacao-e-correcoes.md
```

## Operações destrutivas

Exclusão de arquivo, campanha ou árvore do repositório é operação administrativa, não ficção.

Antes de apagar material persistente:

```text
1. identificar exatamente o alvo;
2. verificar que ele existe;
3. não ampliar o alvo por inferência;
4. obter autorização explícita do usuário para aquela exclusão;
5. apagar somente o que foi autorizado.
```

Para apagar uma campanha inteira, usar o nome exato e deixar claro que toda a pasta `campanhas/<nome>/` será removida. Reclamação, comentário casual ou desejo de recomeçar não contam como autorização de exclusão.

## Continuidade

As fontes persistentes da campanha prevalecem sobre memória vaga de conversas anteriores.

Ao fechar um capítulo, seguir o protocolo atual de Registro: consolidar o que aconteceu, atualizar o presente, reancorar o núcleo operacional e continuar somente depois dessa reancoragem.

> **O repositório atual possui duas responsabilidades: `regras-basicas/` explica como jogar; `campanhas/` guarda o que existe e aconteceu.**
