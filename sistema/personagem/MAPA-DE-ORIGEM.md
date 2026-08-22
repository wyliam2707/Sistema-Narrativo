# Mapa de Origem — Área Personagem

Status: APROVADO

Este arquivo registra de onde vieram as regras reunidas em `sistema/personagem/`.

Nenhum arquivo antigo foi apagado ou movido.

## Classificação do antigo `sistema/README.md`

| Seção antiga | Classificação principal | Destino novo |
|---|---|---|
| 1. Filosofia do sistema | PERSONAGEM + RESOLUÇÃO | `README.md`, `criacao.md`, referências em resolução |
| 2. Escala universal — 0 a 5 | PERSONAGEM | `escala.md` |
| 3. Atributos | PERSONAGEM | `atributos.md` |
| 4. Capacidades naturais | PERSONAGEM | `atributos.md` + `poderes.md` |
| 5. Perícias | PERSONAGEM | `pericias.md` |
| 6. Poderes — sintaxe | PERSONAGEM | `poderes.md` |
| 7. Combinação de capacidades | RESOLUÇÃO, com definição auxiliar de capacidades | permanece principalmente em resolução; princípio referenciado em `poderes.md` |
| 8. Vida | RESOLUÇÃO / STATUS | não migrado como definição de personagem |
| 9. Morte | RESOLUÇÃO | não migrado |
| 10. Armadura, proteção e defesa | RESOLUÇÃO + PERSONAGEM quando houver recurso estável | resolução permanece fora desta pasta; equipamento ou infraestrutura estável relevante pode aparecer em `RECURSOS` |
| 11. Cura, estabilização e recuperação | RESOLUÇÃO | não migrado |
| 12. Energia | STATUS / RESOLUÇÃO | não migrado |
| 13. Equipamento relevante | PERSONAGEM + PERSISTÊNCIA | convertido para `RECURSOS` em `ficha.md`; alterações temporárias continuam fora da ficha |
| 14. Condições temporárias | STATUS | não migrado |
| 15. Relações | PERSONAGEM + PERSISTÊNCIA | `relacoes.md` |
| 16. Social | RESOLUÇÃO | não migrado como regra de ficha |
| 17. Importância de personagens | PERSONAGEM | `ficha.md` + `npcs.md` |
| 18. NPCs rápidos — modelo-base | PERSONAGEM | `npcs.md`; preservada a ideia de ficha compacta, mas modelos automáticos como `Humano [1]` ou `Demônio [3]` foram abandonados |
| 19. Estrutura de ficha completa | PERSONAGEM | `ficha.md` |
| 20. Resolução de ações | RESOLUÇÃO | não migrado |
| 21. Preparação e criatividade | RESOLUÇÃO | não migrado |
| 22. O mundo não protege o enredo | RESOLUÇÃO / OPOSITOR / NARRADOR | não migrado |
| 23. Limites da criatividade | RESOLUÇÃO, apoiada na ficha | não migrado como regra de criação |
| 24. Exemplos compactos | PERSONAGEM | referências distribuídas entre `ficha.md` e arquivos mecânicos |
| 25. Instruções para outro narrador ou IA | OPERAÇÃO + RESOLUÇÃO + PERSONAGEM | apenas princípios definidores de ficha foram reaproveitados |

## Outros arquivos antigos relevantes

### `sistema/calibracao-independente.md`
Destino principal: `calibracao.md`.

Regras preservadas:
- cada personagem é calibrado pelo que ele próprio é;
- outra ficha nunca é régua mecânica;
- conceito/cânone antes da conversão;
- conversão para atributos, perícias e poderes somente depois;
- assimetria é válida;
- não balancear personagens entre si;
- calibração conservadora;
- PATAMAR é qualitativo e não linear;
- `[4]` é extremo e raro;
- `[5]` representa ápice real daquela capacidade.

### `sistema/modelos.md`
Destinos principais:
- `tracos.md`;
- `ficha.md`;
- `npcs.md`.

Regras preservadas ou reformuladas:
- TRAÇOS qualitativos;
- campo desconhecido fica em branco;
- `[0]` é valor real;
- mesma estrutura mecânica pode servir para qualquer personagem;
- ficha reservada do NARRADOR;
- Figurante/inimigo comum pode usar registro mínimo;
- `EQP` foi substituído por `RECURSOS`;
- `Importância` e `CONTROLE` são informações distintas;
- um personagem `Relevante` pode permanecer `CONTROLE: NPC`;
- informação secreta persistente pode ser registrada como `Informação reservada do NARRADOR`.

O antigo modelo-base que preenchia capacidades por natureza, como `Humano [1]` ou `Demônio [3]`, foi rejeitado. NPCs usam exatamente as mesmas mecânicas e escalas que qualquer outro personagem.

### `sistema/protocolo-de-criacao.md`
Destinos principais:
- `criacao.md`;
- `calibracao.md`;
- `ficha.md`.

Regras preservadas:
- conceito antes da mecânica;
- protagonista criado conceitualmente antes da calibração;
- não inventar campos apenas para preencher ficha;
- revisão mecânica posterior;
- personagens apresentados ao jogador revisados antes do protagonista;
- protagonista por último para evitar efeito-régua;
- essa ordem protege o processo e não autoriza comparação ou balanceamento entre fichas;
- calibração conservadora;
- aprovação da ficha antes de tratá-la como final.

### `sistema/informacao-e-descoberta.md`
Destinos principais:
- `pericias.md`;
- `atributos.md`.

Foram extraídas apenas definições de capacidade:
- perícia representa repertório e conhecimento já conquistado;
- graduação de perícias altera o quanto o personagem já domina dentro daquele campo;
- MEN ajuda a perceber padrões, analisar, testar hipóteses e conectar informação;
- MEN não substitui conhecimento especializado nem cria informação inexistente.

As regras de cadeia de descoberta permanecem em resolução/informação.

### `sistema/organizacao-de-aventura.md`
Usado como fonte de fronteira para `ficha.md`:
- ficha = dossiê consolidado necessário para interpretar o personagem;
- STATUS = estado circunstancial;
- Progressão = consequências causalmente vivas ainda não incorporadas à ficha.

### `sistema/progressao-narrativa.md`
Usado apenas como fronteira:
- não existe XP automático;
- ficha muda quando o personagem realmente muda;
- consequência circunstancial não entra automaticamente em `REL`.

### `sistema/agencia-de-personagens.md`
Usado para confirmar campos de ficha que sustentam agência:
- personalidade;
- história;
- desejos/objetivos;
- medos/limites;
- relações;
- capacidades.

A regra de agência em si continua fora desta pasta.

### `sistema/modo-rpg.md`
Usado somente para confirmar que `CONTROLE` é metadado estrutural da ficha.

O significado operacional de cada categoria de `CONTROLE` pertence à arquitetura de `personas/` e não é redefinido aqui.

## Fronteira com STATUS

Vida atual, Energia ou Mana atual, ferimentos, condições temporárias, efeitos ativos e localização não fazem parte da definição permanente do personagem.

Essas informações mudam rapidamente e pertencem ao STATUS ou à camada de resolução/persistência correspondente.

Se existir um valor máximo ou outra característica estável necessária para definir uma capacidade do personagem, essa origem pode ser definida em outra regra apropriada; o valor atual continua sendo STATUS.

## Organização dos personagens na campanha

A área de sistema define como qualquer personagem é lido e construído, mas as fichas concretas da campanha ficam separadas por função:

```text
aventuras/<campanha>/
├── personagens/
│   └── personagens jogáveis
└── mundo/
    └── npcs/
        └── NPCs persistentes
```

`personagens/` é preparado para personagens efetivamente jogáveis sob `JOGADOR HUMANO` ou `JOGADOR IA`.

NPCs pertencem ao mundo administrado pelo NARRADOR.

A pasta `mundo/npcs/` não precisa existir no início da campanha. O NARRADOR cria essa estrutura e suas fichas quando algum NPC acumular informação que realmente precise de continuidade.

Ter ficha persistente não altera automaticamente `Importância` nem `CONTROLE`.

## Princípio da migração

> **Extrair definição não significa mover toda regra que menciona uma ficha.**

Se um arquivo antigo explica como uma capacidade é usada para resolver uma ação, a definição da capacidade pode vir para `personagem/`, mas a regra de resolução continua em `resolucao/`.

Da mesma forma, uma informação pode depender da ficha sem pertencer a ela. Vida atual, Mana atual, ferimentos e condições consultam capacidades do personagem, mas continuam sendo STATUS.
