# Núcleo

Status: REFORMULAÇÃO / NÃO IMPLEMENTADO

Reúne as regras comuns que definem como a mesa funciona, quem possui autoridade e como conflitos são resolvidos.

## Estrutura atual

```text
0.1-resolucao.md
→ arquitetura da resolução de conflitos e testes.

0.2-rolagens.md
→ define que o Narrador executa todas as rolagens usando fonte aleatória real disponível.

0.3-consequencias.md
→ define como interpretar 7–9 sem criar punições arbitrárias; usa consequência do risco concreto ou resultado limitado ligado ao próprio objetivo.

1.0-tribunal.md
→ procedimento geral da mesa e interação entre as cadeiras.

1.1-narrador.md
→ juiz da mesa: julga, resolve, narra e registra.

1.2-jogador-humano.md
→ autoridade e funcionamento da personagem controlada pelo usuário.

1.3-jogador-ia.md
→ personagem autônoma com jogador IA dedicado.

1.4-jogador-ia-eventual.md
→ personagens eventuais e NPCs ad hoc com agência própria.

1.5-opositor.md
→ promotoria da mesa, ganchos, planos e oposição ativa.

1.6-execucao-por-uma-unica-ia.md
→ protocolo para uma única IA técnica executar várias cadeiras sem misturar conhecimento, objetivos ou autoridade.

1.7-criacao-emergente.md
→ autoridade limitada do Narrador para completar partes ainda indefinidas do mundo com fatos neutros, sem criar vantagens, obstáculos ou oposição retroativa.

1.8-origem-de-conflitos.md
→ permite ao Opositor originar novos conflitos coerentes em campanhas emergentes, sujeitos à validação do Narrador e sem construção retroativa contra ações ou fichas.
```

## Princípio estrutural

```text
JOGADORES
→ decidem por suas próprias peças.

OPOSITOR
→ movimenta a oposição legítima.
→ pode originar novos conflitos dentro dos limites de 1.8-origem-de-conflitos.md.

NARRADOR
→ julga o conjunto apresentado.
→ pode completar espaços ainda indefinidos do mundo somente dentro dos limites de criação emergente neutra.
→ valida a existência de conflitos novos antes que sejam usados na ficção.

RESOLUÇÃO
→ decide incertezas quando necessário.
→ 7–9 nunca obriga a criar punição desconectada; seguir 0.3-consequencias.md.

ROLAGENS
→ são executadas pelo Narrador com fonte aleatória real disponível.

EXECUÇÃO TÉCNICA
→ uma única IA pode executar várias cadeiras.
→ cada cadeira continua usando somente seu próprio escopo decisório.

REGISTRO
→ preserva o que passou a ser verdade.
```

A ordem usada pela IA para executar internamente as cadeiras não determina ordem ficcional, iniciativa ou prioridade.

As declarações operacionais das cadeiras da IA podem permanecer internas durante o jogo normal; o usuário recebe principalmente a sentença narrada e o próximo ponto em que sua própria decisão é necessária.

A criação emergente não autoriza o Narrador a alterar retroativamente uma situação em resposta à ação declarada. Fatos neutros podem completar o mundo ainda indefinido; fatos consequenciais precisam de fundamento legítimo conforme `1.7-criacao-emergente.md`.

A origem de conflito pertence ao Opositor, mas não é resultado automático. O Opositor propõe; o Narrador valida coerência, meios, tempo e oportunidade; o Registro fixa o que passou a existir; somente depois a oposição pode ser movimentada normalmente.

As regras específicas de Defesas, Resistências, alcance, movimento, dano, Vida, Mana, condições, Poderes e demais mecânicas universais serão adicionadas ao Núcleo conforme forem reformuladas.

> O Núcleo define a arquitetura comum da mesa. Regras específicas usam essa base sem redefinir autoridade ou procedimento.
