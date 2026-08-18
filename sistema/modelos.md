# Modelos de Arquivos

Estes modelos existem para tornar a criação de aventuras consistente e rápida.

## Regra durante a criação

Durante a criação conceitual, preencher somente o que já foi realmente definido.

Campos ainda desconhecidos permanecem **em branco** até a revisão correspondente.

> **Nunca usar `[0]` para representar algo ainda não definido. Zero é um valor mecânico real.**

Enquanto uma ficha apresentável ao jogador ainda estiver sendo construída ou revisada, usar:

```text
Status: PENDENTE DE REVISÃO
```

Somente depois da aprovação explícita do jogador mudar para:

```text
Status: APROVADO
```

Essa exigência de aprovação não se aplica a fichas reservadas do narrador em `mestre/viloes/`, porque apresentá-las ao jogador destruiria o sigilo. Essas fichas seguem a regra própria definida abaixo.

## TRAÇOS

`TRAÇOS` registram verdades permanentes ou estáveis sobre um personagem que importam para a ficção, mas não precisam de graduação numérica.

Exemplos:

- Não envelhece.
- Não precisa respirar.
- Corpo artificial.
- Herança demoníaca.
- Não pode mentir.

Um TRAÇO não possui grau oculto e não é somado a atributos, perícias ou poderes.

Se uma característica representa capacidade ativa, potência, resistência ou algo que precise ser comparado em escala, ela deve ser registrada como atributo, perícia ou poder.

Exemplos:

- `Herança demoníaca` pode ser TRAÇO.
- `Empatia [3]` é Poder.
- `RES [4]` é atributo.

Um TRAÇO pode influenciar diretamente a ficção quando sua própria natureza resolve a questão. Um personagem com `Não precisa respirar`, por exemplo, não começa a sufocar debaixo d'água.

TRAÇOS não devem duplicar desnecessariamente capacidades que já estejam descritas mecanicamente.

> **TRAÇO = verdade qualitativa estável. Atributo, perícia ou poder = capacidade graduada.**

## Regra de revisão das fichas apresentáveis

O modelo de arquivo é o mesmo, mas o **método de revisão muda conforme quem controla o personagem**.

### Personagem controlado pelo jogador

Revisar com controle fino, seguindo a ficha de cima para baixo.

Campos simples são apresentados **um por vez** e precisam ser aprovados antes de avançar.

Três conjuntos são tratados como blocos próprios:

```text
ATRIBUTOS = FOR | AGI | RES | MEN | VON
PERÍCIAS = todas as perícias relevantes
PODERES = todos os poderes e especializações
```

Fluxo recomendado:

```text
nome/identidade
↓
idade
↓
conceito
↓
descrição
↓
TRAÇOS
↓
ATRIBUTOS — bloco
↓
PERÍCIAS — bloco
↓
PODERES — bloco
↓
EQP
↓
REL
↓
personalidade e tendências
↓
desejos/objetivos atuais
↓
medos/limites relevantes
↓
história consolidada relevante
↓
ficha completa para aprovação final
```

Se um campo já estiver definido, apresentá-lo como está para confirmação em vez de recriá-lo.

Nos blocos de ATRIBUTOS, PERÍCIAS e PODERES, reapresentar o bloco inteiro normalizado antes de pedir aprovação.

> **No personagem do jogador, cada campo simples é uma etapa; ATRIBUTOS, PERÍCIAS e PODERES são blocos próprios.**

### Demais personagens apresentáveis ao jogador

Revisar em **quatro blocos**:

**Bloco 1 — Identidade e conceito**
- nome;
- idade;
- conceito;
- descrição;
- `TRAÇOS`.

**Bloco 2 — Capacidades**
- atributos;
- perícias;
- poderes e especializações.

**Bloco 3 — Recursos**
- `EQP` e recursos recorrentes;
- `REL` atual e recorrente.

**Bloco 4 — Interpretação**
- personalidade e tendências;
- desejos/objetivos atuais;
- medos/limites relevantes;
- história consolidada relevante.

O narrador pode propor uma base para cada bloco, mas deve obter aprovação antes de avançar para o próximo.

Depois dos quatro blocos, apresentar a ficha completa para aprovação final.

Fichas reservadas em `mestre/viloes/` não passam por revisão aberta.

## 1. Ficha — personagem Central

```text
# Nome

Status: PENDENTE DE REVISÃO
Importância: Central

Idade:
Conceito:
Descrição:

TRAÇOS:
- ...

ATR: FOR [ ] | AGI [ ] | RES [ ] | MEN [ ] | VON [ ]
PER:
Poder [Fonte opcional] [ ] => uso / uso / especialização [ ]
Poder [ ] => ...
EQP:
REL:

## Personalidade e tendências
- ...

## Desejos/objetivos atuais
- ...

## Medos/limites relevantes
- ...

## História consolidada relevante
- somente fatos necessários para interpretar o personagem; detalhes completos ficam no livro/cronologia
```

A ficha Central pode ser mais descritiva porque precisa sustentar agência e continuidade por muito tempo.

Não preencher `TRAÇOS`, `EQP`, `REL`, poderes ou qualquer outro campo apenas para completar visualmente a ficha.

Relações circunstanciais que ainda podem voltar a importar, mas não pertencem à vida recorrente do personagem, devem ficar em `progressao/` em vez de ampliar indefinidamente `REL`.

## 2. Ficha — personagem Relevante

```text
# Nome

Status: PENDENTE DE REVISÃO
Importância: Relevante

Idade:
Conceito:
Descrição:

TRAÇOS:
- ...

ATR: FOR [ ] | AGI [ ] | RES [ ] | MEN [ ] | VON [ ]
PER:
Poder [ ] => ...
EQP:
REL:

## Personalidade e tendências
- ...

## Desejos/objetivos atuais
- ...

## Medos/limites relevantes
- ...

## História consolidada relevante
- ...
```

Adicionar apenas o detalhe necessário ao papel real do personagem.

Uma ficha Relevante pode permanecer mais curta que uma Central. Se algum bloco não for importante, deixá-lo vazio em vez de inventar conteúdo.

### Criação conceitual mínima de aliados

Durante a criação conceitual, pode ser suficiente definir apenas **quantidade e nomes** dos aliados relevantes.

Nesse caso, criar os arquivos com a estrutura oficial e preencher somente aquilo que já foi realmente estabelecido. Todo o restante permanece em branco até a revisão.

Exemplo:

```text
# Lucia James

Status: PENDENTE DE REVISÃO
Importância: Relevante

Idade:
Conceito:
Descrição:

TRAÇOS:

ATR: FOR [ ] | AGI [ ] | RES [ ] | MEN [ ] | VON [ ]
PER:
Poder:
EQP:
REL:
```

O narrador não deve inventar aparência, personalidade, história, capacidades ou recursos apenas para completar a ficha, salvo quando o jogador delegar explicitamente essa criação.

## 3. Ficha reservada — antagonista importante

Um antagonista importante, recorrente ou poderoso pode receber ficha completa sem ser apresentado ao jogador.

Armazenar em:

```text
mestre/viloes/<nome>.md
```

Modelo recomendado:

```text
# Nome

Status: CANÔNICO DO MESTRE
Visibilidade: MESTRE
Importância: Relevante | Central

Idade:
Conceito:
Descrição:

TRAÇOS:
- ...

ATR: FOR [ ] | AGI [ ] | RES [ ] | MEN [ ] | VON [ ]
PER:
Poder [ ] => ...
EQP:
REL:

## Personalidade e tendências
- ...

## Desejos/objetivos atuais
- ...

## Medos/limites relevantes
- ...

## História consolidada relevante
- ...

## Segredos ainda não descobertos
- ...
```

`CANÔNICO DO MESTRE` significa que a ficha é uma verdade operacional reservada ao narrador. Ela não passa pelo fluxo `PENDENTE DE REVISÃO → APROVADO`, porque isso exigiria revelar o conteúdo ao jogador.

O narrador deve definir apenas o que realmente precisa existir. Não é necessário preencher todos os campos.

Sempre que for prático, capacidades ocultas relevantes devem ser definidas **antes** de serem usadas diretamente contra o protagonista.

Depois de estabelecida, a ficha não pode ganhar poderes, resistências, imunidades ou recursos retroativos apenas para contrariar uma solução válida, restaurar dificuldade ou proteger a trama.

Mudanças posteriores precisam nascer de acontecimentos reais da ficção.

Informações desta ficha só entram na narração como conhecimento do jogador quando o protagonista as descobrir de forma plausível.

> **Ficha oculta preserva segredo; não autoriza improvisar vantagem retroativa.**

## 4. Figurante / inimigo comum

Figurantes e inimigos comuns **não precisam de arquivo individual** na maioria dos casos.

Usar apenas o mínimo necessário para a cena.

Exemplos:

```text
Guarda — Humano [1] | Soldado [+2] | rifle / colete
```

```text
Invocação — Demônio [3] | FOR [4] | VON [1]
```

O modelo-base define todos os atributos. Só registrar exceções.

Esse registro pode existir apenas durante a resolução da cena; não precisa ser salvo em `personagens/`, `mestre/viloes/` ou outro arquivo persistente.

Se um inimigo inicialmente comum sobreviver, voltar a aparecer ou ganhar importância real, ele pode então receber ficha Relevante ou ficha reservada de antagonista.

Poder por si só não obriga a criar arquivo. O critério é a necessidade de continuidade e detalhe.

## 5. STATUS atual

```text
# Estado Atual

Momento: fim/início do capítulo ...
Local principal: ...
Situação imediata: ...

## Personagem Central/Relevante
VIDA: Ileso | Ferido | Grave | Crítico | Incapacitado
ENERGIA: Pleno | Metade | Limite | Crítico
COND: Nenhuma / condição 1 / condição 2
EQP temporário: dano, falta ou alteração circunstancial relevante
Efeitos ativos: ...
Local: ...

## Outro personagem
...

## Pontas imediatas
- ameaças em andamento;
- decisões pendentes;
- prazos imediatos;
- fatos que precisam ser lembrados ao retomar.
```

`Crítico` em ENERGIA significa: resta aproximadamente **uma última ação relevante** antes de esgotamento, falta de recurso ou colapso coerente com o personagem.

Informações de STATUS que devam permanecer secretas para o jogador não devem ser expostas em uma fonte tratada como apresentável ao jogador.

## 6. Relação complexa

```text
# Personagem A & Personagem B

Status: canônico / planejado / rascunho

## Situação atual
- A → B: [+ ]
- B → A: [+ ]

## Natureza do vínculo
- ...

## Dinâmica
- como A tende a agir com B;
- como B tende a agir com A;
- conflitos e compatibilidades relevantes.

## Evolução consolidada
- fatos que realmente aconteceram.

## Possibilidades/rumos planejados
- ideias futuras que ainda NÃO são fatos canônicos.
```

Nunca tratar trajetória planejada como acontecimento já ocorrido.

Usar este modelo para relações recorrentes ou complexas. Uma pessoa circunstancial que apenas pode voltar a importar não precisa ganhar um arquivo aqui; pode ser registrada em Progressão.

## 7. Progressão Narrativa — Evolução de Vida

A Progressão não é XP nem lista de recompensas. Registra **consequências ainda vivas que podem voltar a produzir efeito**.

Modelo recomendado:

```text
# Progressão Narrativa

## Relações circunstanciais
- Princesa Elara [+2] — ficou favorável após o resgate; fora da ficha porque não faz parte da vida atual.
- Capitão dos Corvos [-2] — passou a odiar o personagem após a humilhação pública.

## Acessos
- Mercado de Armas de Karsk — acesso liberado.

## Favores e dívidas
- Rei Alaric — deve um favor importante.

## Recursos ou apoios acionáveis
- Corvos Cinzentos — aceitam contratos do personagem.

## Posições / autoridade
- ...

## Restrições / perdas
- ...

## Ameaças ou promessas latentes
- Trigon passou a considerar o personagem um inimigo pessoal.
- Darek jurou vingança e continua vivo.
```

Não é obrigatório usar todos os subtítulos. Criar apenas os que realmente ajudam.

Uma entrada deve responder, de forma compacta:

```text
Consequência: o que mudou.
Origem: capítulo/cena, se útil.
Estado: ainda válida / encerrada, apenas se houver ambiguidade.
```

O arquivo não precisa registrar toda consequência menor.

> **Registrar somente o que ainda possui potencial causal futuro.**

Quando uma relação circunstancial passa a integrar de fato a vida recorrente do personagem, ela pode sair da Progressão e passar a ser acompanhada em `REL` da ficha ou em `relacionamento/`.

Quando um favor é usado, uma dívida é quitada, uma ameaça deixa de existir ou outra consequência perde qualquer futuro plausível, remover/arquivar a entrada; o fato histórico continua preservado em livro/cronologia.

## 8. Cronologia

```text
## Capítulo / período
Local: ...
Presentes: ...
Acontecimento: ...
Consequência: ...
Conhecimento adquirido:
- Personagem A passou a saber ...
- Personagem B ainda não sabe ...
```

O campo de conhecimento é importante para impedir metaconhecimento acidental.

> **Cronologia diz o que aconteceu. Progressão destaca o que ainda pode voltar a importar.**

## 9. README de uma aventura

```text
# Nome da Aventura

## Premissa
...

## Personagens centrais
- ...

## Modelo narrativo
Base herdada: `sistema/narracao-e-escrita-padrao.md`
Referência de calibração: `sistema/exemplo-de-estilo.md`

Exceções desta aventura:
- nenhuma; ou
- listar somente aquilo que realmente muda em relação ao padrão.

## Como narrar
Ler antes:
- `sistema/narracao-e-escrita-padrao.md`;
- diretrizes específicas desta aventura, se existirem.

As diretrizes locais complementam ou alteram apenas o que declararem explicitamente. Todo o restante continua herdado do modelo narrativo padrão.

## Hierarquia de cânone
1. correção explícita mais recente;
2. livro/capítulos consolidados;
3. diretrizes;
4. material reservado do narrador em `mestre/`, quando aplicável;
5. personagens/mundo/relacionamento;
6. progressão narrativa vigente;
7. cronologia;
8. estado atual;
9. rascunhos antigos.

## Ponto atual
Consultar: `estado/atual.md`

## Regra de continuidade
Nunca continuar apenas pela memória de outro chat; consultar as fontes desta aventura.
Ao consultar `mestre/`, usar a informação sem revelá-la ao jogador antes de ser descoberta na ficção.
```

## 10. Princípio de economia

Não preencher campos apenas porque o modelo existe.

> **Registrar somente o que ajuda o narrador a decidir, lembrar ou manter continuidade.**

Central recebe detalhe alto; Relevante recebe detalhe proporcional ao papel; Figurante e inimigo comum recebem apenas o necessário para a cena.

Antagonista reservado recebe ficha completa somente quando continuidade, poder, recorrência ou segredo realmente justificarem esse trabalho.

A Progressão segue a mesma regra: não guardar toda reação ou consequência menor, apenas aquilo que ainda pode ter vida futura.