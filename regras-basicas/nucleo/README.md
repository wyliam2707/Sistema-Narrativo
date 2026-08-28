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

0.4-disputas-simultaneas.md
→ resolve ações realmente simultâneas com uma única rolagem e faixas espelhadas em torno de 7, sem vantagem artificial por ordem de declaração.

0.5-combate.md
→ Ataque contra Defesa resolve técnica e gera Potência Nula/1/2/3; Poder ou equipamento ofensivo soma depois somente quando o efeito entra.

0.6-dano-e-ferimentos.md
→ resolve `1d6 + Potência` contra `1d6 + Resistência`, converte a diferença em gravidade e aplica a recuperação pelos degraus de Cura, sem pontos de Vida.

0.7-iniciativa.md
→ usa a ordem ficcional quando evidente e só resolve prioridade quando agir primeiro realmente estiver em disputa; não mantém iniciativa permanente.

0.8-tempo-e-acoes.md
→ define rodada como aproximadamente 10 segundos, turno como oportunidade operacional da personagem e uma intenção principal plausível sem economia rígida de ações.

0.9-alcance-e-movimento.md
→ usa quatro faixas relativas — Toque, Perto, Médio e Longe — e movimento abstrato sem exigir mapa ou metros.

0.10-mana.md
→ define Mana como esforço extra com limite total de 2 por turno, distribuído na declaração entre Ação, Efeito e Defesa; Mana defensiva dura até o início do próximo turno da personagem.

0.11-vida-e-mente.md
→ define dois trilhos universais em linha, Vida e Mente, com a mesma progressão Leve/Sério/Grave/Crítico/Incapacitado e descrição narrativa do estado concreto.

0.12-ataques-mentais.md
→ espelha o dano físico para Mente: acerto técnico, Potência Mental contra Resistência Mental e a mesma escala de gravidade.

0.13-cura-e-recuperacao.md
→ usa a Potência de Efeito universal para gerar Cura e aplica o resultado diretamente em Vida ou Mente conforme o escopo Física, Mental ou Completa.

0.14-potencia-de-efeito.md
→ transforma o resultado de `Atributo + Perícia` em Potência Nula/1/2/3; Poder soma depois somente quando a execução produz efeito.

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
→ disputas realmente simultâneas usam 0.4-disputas-simultaneas.md para evitar vantagem artificial de lado ativo.

COMBATE
→ Ataque usa Atributo + Combate ou Conjuração.
→ Defesa usa Atributo + Defesa.
→ a única rolagem técnica usa `2d6 + Ataque - Defesa + situação`.
→ 6- gera Potência Nula: o ataque falha, o efeito não entra e a resolução ofensiva encerra.
→ 7–9 / 10–11 / 12+ geram Potência de Execução 1 / 2 / 3.
→ em um acerto, somar depois Poder ou equipamento ofensivo pertinente.
→ `Potência Final = Potência de Execução + Poder`.
→ proteção não aumenta automaticamente Defesa técnica; entra na Resistência quando pertinente.

POTÊNCIA DE EFEITO
→ um teste de execução usa `2d6 + Atributo + Perícia`.
→ 6- gera Potência Nula e encerra o efeito.
→ 7–9 / 10–11 / 12+ geram Potência de Execução 1 / 2 / 3.
→ se um Poder ou equipamento fornecer a força do efeito, somar sua graduação depois.
→ `Potência Final = Potência de Execução + Poder`.
→ efeito direto usa a Potência Final diretamente.
→ efeito resistido usa `1d6 + Potência` contra `1d6 + Resistência`.

DANO
→ depois de um acerto, resolver `1d6 + Potência Final` contra `1d6 + Resistência`.
→ diferença positiva determina gravidade do ferimento.
→ não existem pontos de Vida.
→ ferimentos iguais acumulam e sobem uma categoria.

RECUPERAÇÃO
→ Vida e Mente usam a mesma matemática de Cura.
→ quando houver teste, usar `2d6 + Atributo + Perícia`.
→ 6- gera Potência Nula: não existe Cura Final naquela tentativa.
→ 7–9 / 10–11 / 12+ geram Potência de Execução 1 / 2 / 3.
→ Poder ou equipamento de Cura soma sua graduação depois.
→ `Cura Final = Potência de Execução + Cura`.
→ Cura é efeito direto: aplicar a Cura Final sem nova rolagem de efeito.
→ Mana na Ação pode melhorar o teste; Mana no Efeito pode aumentar a Cura Final conforme 0.10.
→ Cura é aplicada automaticamente do comprometimento menos grave para o mais grave.
→ marcas regridem pelos custos 1/2/4/8/16 até desaparecer.
→ Cura possui escopo: Física, Mental ou Completa.
→ Cura Física só afeta Vida; Cura Mental só afeta Mente.
→ Cura Completa escolhe Vida ou Mente em cada aplicação e não é numericamente mais potente por isso.
→ uma mesma aplicação não se divide entre os dois trilhos sem permissão explícita da capacidade.

INICIATIVA
→ ordem evidente vem da ficção.
→ só existe disputa quando agir primeiro realmente importa e a prioridade não está estabelecida.
→ normalmente usa Agilidade + Percepção e a resolução espelhada de 0.4.
→ não existe lista permanente de iniciativa.
→ iniciativa decide apenas prioridade e não gera Potência de Execução.
→ em rodadas, registrar apenas se cada participante já usou sua intenção principal.

TEMPO E AÇÕES
→ rodada representa aproximadamente 10 segundos de ficção.
→ turno é a oportunidade operacional de uma personagem dentro da rodada.
→ cada participante realiza uma intenção principal plausível.
→ movimentos e gestos necessários podem integrar a mesma intenção.
→ não há divisão automática em ação, movimento, bônus e reação.
→ a ordem operacional dos turnos não cria prioridade ficcional por si só.
→ o Narrador julga o que cabe pela ficção, capacidades e unidade da intenção.

ALCANCE E MOVIMENTO
→ usar Toque, Perto, Médio e Longe.
→ as faixas são relativas entre os elementos da cena, não zonas fixas de um mapa.
→ movimento comum usa 1 faixa por rodada como referência.
→ movimento pode integrar a intenção principal quando isso couber nos aproximadamente 10 segundos.
→ Poderes e obstáculos podem ampliar, restringir ou ignorar essa referência.

MANA
→ representa esforço extra, não combustível obrigatório de magia.
→ máximo de 2 Mana no total por turno.
→ a distribuição é declarada antes da resolução.
→ os 2 pontos podem ser concentrados ou divididos entre Ação, Efeito e Defesa.
→ Mana na Ação melhora o teste, ajudando a evitar falha e podendo elevar a Potência de Execução.
→ Mana no Efeito aumenta diretamente a Potência Final.
→ Mana na Defesa aumenta a Defesa técnica desde a declaração até o início do próximo turno da personagem.
→ o mesmo bônus defensivo vale para todas as defesas legítimas nesse intervalo, sem novo gasto por atacante.
→ os gastos não podem ser realocados depois dos resultados.
→ reserva normal 5 ou 10.
→ 1 hora de descanso curto adequado restaura a reserva ao máximo.

VIDA E MENTE
→ a ficha usa dois trilhos paralelos e independentes:
→ `Vida: Leve [ ] > Sério [ ] > Grave [ ] > Crítico [ ] > Incapacitado [ ]`
→ `Mente: Leve [ ] > Sério [ ] > Grave [ ] > Crítico [ ] > Incapacitado [ ]`
→ marcas iguais acumulam e sobem uma categoria.
→ Vida registra comprometimento físico ou corporal.
→ Mente registra comprometimento mental, emocional ou psíquico.
→ a categoria informa a gravidade técnica; a descrição narrativa informa o estado concreto.
→ Incapacitado é um ponto final técnico, não um resultado narrativo automático específico.

ATAQUES MENTAIS
→ usam o mesmo fluxo de dano físico.
→ primeiro resolvem acerto técnico contra Defesa quando houver defesa legítima.
→ depois resolvem `1d6 + Potência Mental` contra `1d6 + Resistência Mental`.
→ diferença 0 / 1–2 / 3–4 / 5–6 / 7+ gera nenhum comprometimento / Leve / Sério / Grave / Crítico.
→ o resultado marca o trilho de Mente.

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

As demais mecânicas universais serão adicionadas ao Núcleo conforme forem reformuladas.

> O Núcleo define a arquitetura comum da mesa. Regras específicas usam essa base sem redefinir autoridade ou procedimento.
