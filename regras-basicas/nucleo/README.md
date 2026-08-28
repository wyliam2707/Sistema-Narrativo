# Núcleo

Status: REFORMULAÇÃO / NÃO IMPLEMENTADO

Reúne as regras comuns que definem como a mesa funciona, quem possui autoridade e como conflitos são resolvidos.

## Estrutura atual

```text
0.1-resolucao.md
→ arquitetura da resolução de conflitos e testes.

0.2-rolagens.md
→ define que o Narrador executa todas as rolagens usando fonte aleatória real disponível.

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
```

## Princípio estrutural

```text
JOGADORES
→ decidem por suas próprias peças.

OPOSITOR
→ movimenta a oposição legítima.

NARRADOR
→ julga o conjunto apresentado.

RESOLUÇÃO
→ decide incertezas quando necessário.

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

As regras específicas de Defesas, Resistências, alcance, movimento, dano, Vida, Mana, condições, Poderes e demais mecânicas universais serão adicionadas ao Núcleo conforme forem reformuladas.

> O Núcleo define a arquitetura comum da mesa. Regras específicas usam essa base sem redefinir autoridade ou procedimento.
