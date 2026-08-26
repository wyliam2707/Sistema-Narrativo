# Criação e Revisão de Personagens

Status: APROVADO

Este arquivo define como uma personagem nasce, é registrada e depois revisada dentro do sistema.

Ele não substitui o processo completo de criação de campanha em `../criacao/README.md`.

---

## Princípio central

> **A ficha nasce completa em estrutura e mínima em conteúdo.**

Antes da revisão, definir somente:

```text
1 - NOME
2 - IMPORTÂNCIA
3 - CONTROLE
```

Se uma dessas informações já tiver sido fornecida explicitamente, registrá-la e não perguntar novamente.

`IMPORTÂNCIA` e `CONTROLE` são independentes. Suas regras pertencem a `ficha.md` e `../personas/`.

---

## Método de criação assistida

A revisão usa como padrão:

```text
base disponível
→ proposta coerente do NARRADOR
→ correções do JOGADOR HUMANO
→ reapresentação quando necessário
→ aprovação explícita
→ persistência
```

A base disponível pode vir de:

- versão conhecida ou canônica escolhida;
- Conceito e fatos já discutidos;
- blocos anteriores aprovados;
- relações e decisões já estabelecidas;
- material original criado para a personagem.

A proposta evita criação burocrática do zero, mas não vira fato antes da aprovação.

> **Proposta não é fato. Aprovação transforma a proposta em informação persistente.**

Uma correção pontual altera somente aquilo que realmente foi pedido, salvo quando a mudança exigir reorganização mais ampla.

---

## Nascimento da ficha

Assim que `NOME + IMPORTÂNCIA + CONTROLE` estiverem definidos:

1. criar o arquivo da personagem;
2. copiar o modelo-base completo de `ficha.md`;
3. usar `Status: PENDENTE DE REVISÃO`;
4. preencher apenas Nome, Importância e CONTROLE;
5. deixar os demais campos vazios.

Exemplo estrutural:

```text
# Nome

Status: PENDENTE DE REVISÃO
Importância: ...
CONTROLE: ...
Patamar: [ ]

Nome real:
Idade:
Aparência:
Estilo:
Conceito:
Descrição:

TRAÇOS:

ATR:
Corpo  → Potência [ ] | Controle [ ] | Resistência [ ]
Mente  → Intelecto [ ] | Presença [ ] | Vontade [ ]

Vida Máxima [ ] | Mana Máxima [ ]

PERÍCIAS:
PODERES:
RECURSOS:
REL:

## Personalidade e tendências
## Desejos / objetivos atuais
## Medos / limites relevantes
## Conhecimento atual relevante
## História consolidada relevante
```

Não inventar nem persistir antecipadamente os campos ainda não revisados.

---

## Campo desconhecido fica vazio

Nunca usar `[0]` para representar pendência.

```text
Controle [ ]
```

significa valor ainda não definido.

```text
Controle [0]
```

significa valor mecanicamente definido.

Perícias não usam `[+0]`. Uma Perícia ainda não escolhida simplesmente não aparece.

> **Zero é valor real, nunca marcador de informação ausente.**

---

## Ordem da revisão

Cada ficha é construída uma por vez em cinco blocos:

```text
1 - Identidade e Conceito
2 - Patamar, Atributos e Perícias
3 - Poderes e capacidades
4 - Traços, Recursos e relações
5 - Conferência final
```

Em todos os blocos:

```text
base disponível
→ proposta
→ discussão e correção
→ aprovação
→ salvar
→ próximo bloco
```

---

## Bloco 1 — Identidade e Conceito

Nome, Importância e CONTROLE já chegam definidos.

Revisar, quando relevantes:

- nome real;
- idade;
- aparência;
- estilo;
- origem;
- natureza;
- Conceito;
- descrição;
- demais elementos necessários para reconhecer e interpretar a personagem.

Para personagem conhecido ou licenciado, a versão-base serve como proposta reconhecível. O jogador pode adaptá-la antes de aprovar.

Depois da aprovação, a versão da campanha se torna a referência canônica local.

---

## Bloco 2 — Patamar, Atributos e Perícias

Definir o **Patamar** coerente com o desenvolvimento mecânico pretendido.

Aplicar `patamar.md`:

```text
Pontos de Atributo = Patamar × 4
Limite inicial por Atributo = Patamar + 2
máximo permanente = [7]
```

Distribuir os seis Atributos:

```text
Potência
Controle
Resistência
Intelecto
Presença
Vontade
```

Valores negativos podem devolver pontos conforme `patamar.md`.

Registrar apenas as Perícias realmente pertencentes à personagem.

Perícias não possuem grau; sua relevância concede `+1d` conforme `pericias.md` e `../resolucao/`.

Depois dos Atributos permanentes serem aprovados, calcular automaticamente:

```text
Vida Máxima
Mana Máxima
```

pelas regras de `../resolucao/vida.md` e `../resolucao/mana.md`.

Não escolher Vida por Importância narrativa e não calcular Mana pelo maior Atributo.

---

## Bloco 3 — Poderes e capacidades

Registrar quais Poderes realmente fazem parte do arsenal funcional da personagem.

Poderes não usam graduação genérica `[1]–[5]`.

A quantidade inicial segue `patamar.md` quando a personagem estiver sendo criada mecanicamente pelo Novo Motor.

Cada Poder possui funcionamento e Hub próprios.

Revisar:

- quais Poderes existem;
- limites conceituais;
- fonte ou manifestação narrativa quando relevante;
- equipamentos tratados como capacidade especial;
- demais capacidades ativas que precisem de regra própria.

Não criar um Poder para uma ação comum que Atributos e ficção já resolvam adequadamente.

---

## Bloco 4 — Traços, Recursos e relações

Revisar:

- Traços Comuns;
- Traços Sobrenaturais;
- Vícios;
- Corrupções;
- RECURSOS recorrentes;
- relações que realmente pertençam à ficha.

Traços positivos usam valores de aquisição `[1–3]` quando a regra específica exigir.

Vícios valem `[-1]`; Corrupções podem valer `[-1]` ou `[-2]`.

Esses valores não viram bônus genérico de teste.

A economia adicional gerada por Traços negativos segue `patamar.md`.

Relações e fatos já aprovados anteriormente devem reaparecer automaticamente na proposta; não perguntar de novo aquilo que já está estabelecido.

---

## Bloco 5 — Conferência final

Revisar a ficha inteira para transformar os blocos aprovados em uma personagem completa para interpretação e continuidade.

É apropriado completar e revisar aqui:

```text
Personalidade e tendências
Desejos / objetivos atuais
Medos / limites relevantes
Conhecimento atual relevante
História consolidada relevante
```

Também verificar:

- coerência entre Conceito e Patamar;
- soma e limites dos Atributos;
- Perícias sem graduação antiga;
- Vida e Mana derivadas corretamente;
- ausência de Poder `[1–5]` legado;
- ausência de ENERGIA como reserva universal;
- ausência de campos preenchidos sem aprovação.

Campos comprovadamente inúteis podem ser removidos somente depois desta conferência.

---

## Calibração independente

Cada personagem é construído pelo que ele próprio é, conforme `calibracao.md`.

Não usar outra ficha como régua automática.

Equilíbrio deliberado entre personagens só entra quando o JOGADOR HUMANO pedir explicitamente.

Patamar e Dificuldade também não são a mesma coisa.

> **A ficha descreve a personagem. A Dificuldade descreve o problema.**

---

## Salvamento durante a revisão

Cada bloco aprovado é persistido antes de avançar.

```text
bloco apresentado
→ discutir e corrigir
→ jogador aprova
→ atualizar ficha
→ avançar
```

Conteúdo ainda em discussão, alternativas recusadas e tentativas intermediárias não entram na ficha definitiva.

> **Bloco aprovado vira estado persistente. Conteúdo em discussão permanece fora da ficha.**

---

## Organização dos arquivos na campanha

Personagens com agência de jogador ficam em:

```text
campanhas/<nome>/personagens/<personagem>.md
```

Isso inclui:

```text
CONTROLE: JOGADOR HUMANO
CONTROLE: JOGADOR IA
CONTROLE: JOGADOR IA EVENTUAL
```

NPCs persistentes sem agência de jogador ficam em:

```text
campanhas/<nome>/mestre/
```

ou, quando útil:

```text
campanhas/<nome>/mestre/npcs/
```

Não usar `mundo/npcs/` como destino padrão.

---

## Antagonistas reservados

Antagonistas podem receber ficha reservada em `mestre/` quando a revisão aberta revelaria informação que precisa permanecer secreta.

Isso não altera as regras mecânicas nem a calibração.

Capacidades ocultas usadas contra outras peças devem estar previamente estabelecidas sempre que isso for necessário para continuidade e justiça ficcional.

Não alterar capacidades retroativamente apenas para contrariar uma solução válida.

---

## Estado de aprovação

Uma ficha apresentável ao jogador permanece:

```text
Status: PENDENTE DE REVISÃO
```

até a conferência final ser aprovada.

Depois:

```text
Status: APROVADO
```

---

## Alterações posteriores

A ficha não recebe melhorias automáticas apenas por missão, capítulo ou passagem de tempo narrativa.

Quando a ficção altera de forma estável a personagem, a ficha pode ser atualizada conforme as regras de progressão vigentes.

Mudanças permanentes nos Atributos exigem recálculo de Vida Máxima e Mana Máxima.

## Regra final

> **Criar personagem significa consolidar conceito e agência primeiro, depois Patamar, seis Atributos, Perícias sem graduação, Poderes por arsenal funcional, Traços e recursos. Nada é persistido antes de aprovação quando a ficha é aberta ao jogador.**
