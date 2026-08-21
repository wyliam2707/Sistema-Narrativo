# Mapa de Origem — Área Personagem

Status: EM REVISÃO

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
| 10. Armadura, proteção e defesa | RESOLUÇÃO | não migrado, salvo `EQP` como campo de ficha |
| 11. Cura, estabilização e recuperação | RESOLUÇÃO | não migrado |
| 12. Energia | STATUS / RESOLUÇÃO | não migrado |
| 13. Equipamento relevante | PERSONAGEM + PERSISTÊNCIA | `ficha.md`; alterações temporárias continuam fora da ficha |
| 14. Condições temporárias | STATUS | não migrado |
| 15. Relações | PERSONAGEM + PERSISTÊNCIA | `relacoes.md` |
| 16. Social | RESOLUÇÃO | não migrado como regra de ficha |
| 17. Importância de personagens | PERSONAGEM | `npcs.md` |
| 18. NPCs rápidos — modelo-base | PERSONAGEM | `npcs.md` |
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
- não balancear personagens entre si.

### `sistema/modelos.md`
Destinos principais:
- `tracos.md`;
- `ficha.md`;
- `npcs.md`.

Regras preservadas:
- TRAÇOS qualitativos;
- campo desconhecido fica em branco;
- `[0]` é valor real;
- ficha Central;
- ficha Relevante;
- antagonista reservado;
- Figurante/inimigo comum.

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
- ficha = características estáveis;
- STATUS = estado temporário;
- Progressão = consequências causalmente vivas.

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

## Princípio da migração

> **Extrair definição não significa mover toda regra que menciona uma ficha.**

Se um arquivo antigo explica como uma capacidade é usada para resolver uma ação, a definição da capacidade pode vir para `personagem/`, mas a regra de resolução continua em `resolucao/`.
