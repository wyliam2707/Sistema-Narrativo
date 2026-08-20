# Checklist do Narrador — Uso Operacional

Este arquivo é uma **referência rápida durante a sessão**. Ele não cria regras novas e não substitui os documentos completos do sistema.

Use-o para verificar a resolução de uma cena sem precisar reler todos os arquivos a cada ação.

> **DECLARAÇÕES DOS JOGADORES → Escopo → Situação → Capacidades → Outros agentes → Resolução → Nova decisão → Persistência**

---

## 0. REGRA DE PRIORIDADE MÁXIMA — a Janela de Declarações foi concluída?

Antes de qualquer resolução de uma nova ação significativa, aplicar `ciclo-de-jogadores.md`.

O ciclo obrigatório é:

```text
JOGADOR HUMANO declara
↓
JOGADOR IA [1] declara
↓
JOGADOR IA [2] declara
↓
outros Jogadores IA/Eventuais ativos declaram, se existirem
↓
NARRADOR resolve
```

Verificar:

- todos os `JOGADOR IA` permanentes relevantes declararam intenção?
- todos os `JOGADOR EVENTUAL IA` atualmente ativos declararam intenção?
- algum Jogador Eventual deveria ser ativado antes da resolução?
- alguma intenção é apenas continuação de ação anterior?
- algum jogador legitimamente decidiu não iniciar nova ação?
- cada jogador da IA usou somente o conhecimento legítimo do personagem?
- nenhum jogador da IA foi escolhido retroativamente depois de o Narrador já conhecer o resultado?

A intenção de um jogador pode ser favorável, contrária, independente ou neutra em relação às demais.

A ordem de declaração é operacional e **não concede conhecimento automático** da intenção privada dos jogadores anteriores.

> **Jogadores escolhem intenções. Narrador descobre resultados.**

Se a Janela de Declarações ainda não terminou, **não resolver a cena**.

---

## 1. O que o jogador está tentando fazer?

Trate a declaração como **intenção**, mesmo quando escrita como afirmação.

> `Eu esquivo.` = intenção de esquivar.
>
> `Eu neutralizo os guardas.` = intenção de neutralizá-los.

Pergunte internamente:

- qual é o objetivo real?
- qual método foi declarado?
- até onde vai o escopo da ação?
- existe alguma condição implícita importante, como manter contenção, silêncio, proteção ou outra ação já em andamento?

> **Intenção não garante resultado. Escopo define o que está sendo tentado.**

---

## 2. O que já está acontecendo na cena?

Antes de resolver, considerar:

- posição dos personagens;
- ações já iniciadas;
- efeitos ativos;
- obstáculos;
- ameaças em andamento;
- tempo disponível;
- informação acessível;
- STATUS relevante.

A cena não reinicia a cada nova declaração.

> **Interferência relevante devolve o controle. Devolver o controle não congela os demais agentes.**

Se alguém já estava fugindo, atirando, perseguindo, tratando um ferido, mantendo uma barreira ou executando outro plano, essa ação continua até ser concluída, abandonada, interrompida, neutralizada, tornada impossível ou substituída por nova decisão daquele agente.

---

## 3. A ficha sustenta a execução?

Consultar apenas o que realmente importa para aquela ação:

- atributo;
- perícia;
- poder e especializações;
- equipamento;
- condições;
- Energia;
- preparação;
- informação disponível.

Não somar números automaticamente.

> **Cada capacidade fica no próprio quadrado.**

Um valor alto em uma capacidade não corrige automaticamente uma limitação de outra.

Quando o resultado for óbvio pelas capacidades e pela situação, resolver diretamente sem criar incerteza artificial — **mas somente depois de encerrada a Janela de Declarações**.

---

## 4. Existe capacidade já comprometida?

Não existe economia abstrata de ações.

Verificar quanto da capacidade relevante já está sendo usado por ações ou efeitos que realmente exigem manutenção.

Pergunte:

- o personagem está perto do limite daquela capacidade?
- a nova ação compete pela mesma capacidade?
- as duas coisas podem coexistir de forma coerente?
- o efeito anterior possui apenas duração ou exige sustentação ativa?

> **Duração não é sustentação.**

Um efeito pode continuar existindo sem continuar ocupando capacidade se sua natureza não exigir manutenção.

---

## 5. Quem mais pode agir?

Todos os personagens presentes continuam sendo agentes da história.

Para cada personagem relevante, considerar:

- personalidade;
- objetivos;
- medos;
- conhecimento real;
- relações;
- capacidades;
- STATUS;
- oportunidade;
- ações já em andamento.

Também verificar o campo `CONTROLE` da ficha:

- `JOGADOR IA` — sua intenção já deve ter sido declarada na Janela de Declarações antes da resolução;
- `JOGADOR EVENTUAL IA` — decidir se a situação justifica ativá-lo como jogador antes de fechar a janela;
- `JOGADOR EVENTUAL IA` inativo — tratá-lo normalmente como NPC;
- `NPC` — interpretar pela função de narrador.

Uma decisão tomada pela IA como jogadora deve usar apenas o conhecimento legítimo daquele personagem. Conhecimento exclusivo do narrador, de `mestre/` ou de outro personagem não pode vazar para esse ciclo de decisão.

Se um antagonista relevante possuir ficha reservada em `mestre/viloes/`, consultar essa ficha quando ele estiver envolvido. Usar suas capacidades e objetivos normalmente, mas **não revelar ao jogador informações que o protagonista ainda não descobriu**.

Inimigos comuns não exigem ficha persistente. Para eles, basta o modelo rápido e as exceções necessárias à cena.

Não esperar ordens do protagonista quando um aliado competente possui intenção própria e uma ação óbvia coerente com ela.

Não fazer nenhum personagem agir com informação que ele não possui.

Não criar retroativamente nova capacidade para um inimigo apenas porque o jogador encontrou uma solução eficaz.

Durante o RPG ao vivo, a IA pode usar internamente os pensamentos de `NPC`, `JOGADOR IA` e `JOGADOR EVENTUAL IA` para decidir suas ações, mas **não os mostra diretamente ao jogador humano por padrão**. Mostrar somente fala, gesto, expressão, ação ou outro sinal perceptível.

Toda fala direta deve permanecer identificada:

```text
[Nome] — Fala.
```

Pensamento direto durante a sessão só pode aparecer para o personagem com `CONTROLE: JOGADOR HUMANO`, quando declarado ou autorizado pelo jogador humano, e usa:

```text
[Nome, pensa] — Pensamento.
```

> **Agência decide o que cada personagem quer fazer. Resolução decide o que realmente consegue fazer. A interioridade de NPCs, Jogadores IA e Jogadores Eventuais IA permanece oculta ao jogador humano por padrão durante a sessão.**

---

## 6. Há oposição ou interferência relevante?

Considerar oposição física, mental, social, sobrenatural, ambiental ou circunstancial quando realmente existir.

Um obstáculo não interrompe automaticamente o fluxo.

- porta destrancada: continuar;
- porta trancada, chave correta disponível: usar e continuar;
- porta trancada sem método já definido: nova escolha necessária, parar.

Critério principal:

> **Aconteceu algo que poderia plausivelmente mudar a próxima decisão voluntária do jogador?**

Se não, continuar a resolução.

Se sim, devolver o controle e abrir nova Janela de Declarações antes da próxima resolução significativa.

---

## 7. O que realmente aconteceu?

Separar:

- tentativa;
- execução;
- acerto ou contato;
- efeito real;
- objetivo final.

> **Ataque não significa acerto. Acerto não significa dano. Dano não significa neutralização.**

A resolução pode ser composta.

Exemplo:

> o personagem esquiva parcialmente; o tiro raspa; a contenção enfraquece; ele fica Ferido.

Não reduzir toda situação a sucesso/falha binário quando a causalidade sustenta um resultado parcial.

Quando várias intenções foram declaradas na mesma janela, resolver também:

- simultaneidade;
- precedência real;
- interferência mútua;
- compatibilidade entre objetivos;
- ações que se ajudam;
- ações que se anulam ou dificultam.

---

## 8. A intenção foi cumprida?

Depois da resolução, verificar cada intenção declarada:

- objetivo cumprido completamente;
- objetivo cumprido parcialmente;
- objetivo cumprido com custo;
- objetivo não cumprido, mas a situação mudou;
- tentativa impossível nas condições atuais.

Falha não deve virar silêncio ou beco sem saída quando uma consequência coerente pode mover a história.

> **O resultado deve produzir uma nova situação real para todos os jogadores envolvidos.**

---

## 9. Informação foi tratada corretamente?

Quando a cena envolve percepção, análise ou investigação, verificar:

- a informação realmente existe?
- o personagem possui acesso?
- algo seria automaticamente perceptível?
- a perícia permite reconhecer conhecimento já dominado?
- MEN permite formular direção, hipótese ou método de investigação?
- são necessários exames, testes, pesquisa, tempo ou nova decisão?
- a conclusão está sustentada pelas evidências?

Não inventar informação ausente.

Não transformar MEN em conhecimento universal.

Não exigir que o jogador adivinhe uma frase secreta para investigar corretamente.

Informação presente em `mestre/` existe para o narrador, mas só se torna conhecimento do protagonista quando houver acesso, percepção, inferência ou descoberta plausível.

Pensamentos internos de `NPC`, `JOGADOR IA` ou `JOGADOR EVENTUAL IA` também não se tornam informação do protagonista apenas porque a IA os conhece.

> **Perícia reconhece conhecimento dominado. MEN constrói caminhos para descobrir.**

---

## 10. STATUS mudou?

Atualizar e mostrar STATUS quando houver mudança relevante de:

- Vida;
- Energia;
- Condição;
- efeito ativo;
- dano temporário importante;
- situação operacional que altere opções imediatas.

Não repetir STATUS se nada mudou.

Se Energia mudar de faixa, informar explicitamente.

Em Energia Crítico, avisar que resta aproximadamente uma última ação relevante antes do esgotamento coerente com o personagem.

Não expor STATUS secreto de antagonistas apenas porque o narrador o está acompanhando.

> **Ficha = quem ele é. STATUS = como ele está agora.**

---

## 11. Algo precisa persistir além da cena?

Não salvar tudo em todos os lugares.

### Ficha
Atualizar apenas se o personagem realmente mudou de forma estável.

Não existe XP, aumento automático por missão nem progressão obrigatória de poder.

### REL
Manter na ficha relações recorrentes da vida atual do personagem.

### Progressão
Registrar consequências que não precisam ocupar a ficha, mas ainda possuem potencial causal futuro, por exemplo:

- relação circunstancial relevante;
- favor;
- dívida;
- acesso;
- recurso acionável;
- posição ou autoridade;
- restrição;
- ameaça latente;
- promessa;
- inimigo que pode voltar;
- outra mudança de posição no mundo.

Não registrar consequência banal sem futuro plausível.

> **Progressão não é prêmio. É memória causal.**

### Material reservado do narrador
Se um antagonista importante possui ficha em `mestre/viloes/`, atualizar somente quando a ficção realmente tiver mudado algo relevante.

Não criar poder, resistência, imunidade ou recurso novo apenas para corrigir retrospectivamente uma dificuldade encontrada pelo vilão.

### Cronologia e livro
Registrar os fatos canônicos conforme as regras de persistência da aventura.

Ao consolidar livro, manter falas no formato `[Nome] — ...`. Pensamentos de qualquer personagem podem aparecer no livro como `[Nome, pensa] — ...` quando forem coerentes com a cena e não alterarem os fatos.

---

## 12. Um gancho está surgindo?

Uma consequência antiga ou recente pode criar oportunidade para uma cena futura.

Antes de usá-la, verificar:

- existe motivo?
- existe oportunidade?
- o agente possui informação?
- possui capacidade para agir?
- a circunstância é coerente?

> **Gancho não é obrigação de roteiro.**

Não fazer uma consequência reaparecer apenas porque está registrada. Ela volta quando a causalidade e a agência sustentarem isso.

---

## 13. Antes de devolver o controle ao jogador

Confirmar rapidamente:

1. A ação declarada foi tratada como intenção?
2. **A Janela de Declarações foi concluída antes da resolução?**
3. Todos os Jogadores IA permanentes relevantes declararam?
4. Todos os Jogadores Eventuais ativos declararam?
5. Algum Jogador Eventual deveria ter sido ativado antes da resolução?
6. Nenhum jogador da IA escolheu retroativamente depois de o resultado ser conhecido?
7. O escopo foi respeitado?
8. A situação anterior continuou existindo?
9. Ficha, STATUS e capacidades foram aplicados sem soma cega?
10. Os demais agentes agiram segundo a própria agência e o próprio `CONTROLE`?
11. Informação usada por cada agente era realmente conhecida?
12. A resolução produziu um efeito causal claro?
13. Surgiu uma nova decisão relevante para o jogador?
14. STATUS mudou e precisa ser mostrado?
15. Alguma consequência merece persistência?
16. Se existe material reservado relevante, ele foi respeitado sem ser exposto?
17. Toda fala direta está identificada com `[Nome] — ...`?
18. Nenhum pensamento direto de `NPC`, `JOGADOR IA` ou `JOGADOR EVENTUAL IA` foi revelado ao jogador humano durante o RPG ao vivo?
19. Se apareceu pensamento do personagem com `CONTROLE: JOGADOR HUMANO`, ele foi declarado/autorizado e marcado como `[Nome, pensa] — ...`?
20. A decisão de personagem jogado pela IA usou apenas conhecimento legítimo dele?
21. Alguma ação autônoma fora da câmera deveria ter sido considerada?

Se ainda não surgiu uma nova decisão relevante, a cena pode continuar sob as intenções já declaradas. Quando surgir nova decisão significativa, abrir nova Janela de Declarações.

> **Não parar por hábito. Não resolver antes das declarações. Parar quando existir nova decisão.**

---

## 14. Alertas rápidos

Durante a sessão, evitar:

- **resolver a ação do Jogador Humano antes das declarações dos Jogadores IA ativos**;
- **escolher reação de Jogador IA depois de já saber o resultado**;
- **usar a ordem de declaração como conhecimento automático entre personagens**;
- transformar afirmação do jogador em sucesso automático;
- inventar dificuldade para proteger o roteiro;
- congelar os demais agentes enquanto o jogador decide;
- usar iniciativa ou turnos como regra fundamental;
- somar atributo + perícia + poder automaticamente;
- transformar MEN em onisciência;
- inventar pista que não existe;
- exigir microdeclarações para cada passo de uma ação coerente;
- criar custo de Energia por toda ação pequena;
- contar recursos comuns individualmente quando Energia já os abstrai;
- dar XP ou recompensa mecânica automática por missão;
- colocar toda relação circunstancial na ficha;
- salvar todo detalhe banal na Progressão;
- criar ficha persistente para todo inimigo comum;
- revelar material de `mestre/` antes de ser descoberto;
- revelar pensamento direto de `NPC`, `JOGADOR IA` ou `JOGADOR EVENTUAL IA` ao jogador humano durante o RPG ao vivo;
- inventar pensamento voluntário para o personagem com `CONTROLE: JOGADOR HUMANO`;
- escrever fala direta sem identificar quem falou;
- alterar ficha oculta retroativamente para contrariar uma solução válida;
- forçar um gancho apenas porque ele existe;
- criar reforço, segunda fase ou nova ameaça só para recuperar dificuldade perdida.

---

## Regra final

> **HUMANO DECLARA → IA [1] DECLARA → IA [2] DECLARA → OUTROS JOGADORES ATIVOS DECLARAM → NARRADOR RESOLVE. Depois: respeite o escopo, consulte a realidade da cena, use a ficha sem matemática desnecessária, deixe todos os agentes continuarem vivendo, preserve conhecimento e interioridade, mostre as consequências reais e abra nova Janela de Declarações quando surgir nova decisão significativa.**
