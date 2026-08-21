# Migração Estrutural do Sistema

Status: EM ANDAMENTO

Este arquivo controla a transição da estrutura antiga, concentrada diretamente em `sistema/`, para a nova organização em subpastas.

## Princípio de migração

> **Nenhum arquivo antigo é apagado, movido ou declarado obsoleto apenas porque existe uma pasta nova.**

A substituição ocorre somente quando a regra nova correspondente:

1. foi escrita;
2. foi revisada;
3. foi aprovada;
4. cobre o comportamento necessário do arquivo anterior;
5. teve referências importantes atualizadas.

Até esse momento, o arquivo antigo continua válido.

## Status possíveis

- `NOVA ESTRUTURA` — arquivo/pasta nova de organização; não substitui regra anterior sozinho.
- `ANTIGA AINDA VÁLIDA` — regra antiga continua canônica/operacional.
- `EM REVISÃO` — existe substituta em desenvolvimento, mas a antiga ainda prevalece em pontos não consolidados.
- `SUBSTITUÍDA` — a regra nova passou a ser a referência principal.
- `OBSOLETA` — arquivo antigo pode ser removido ou arquivado quando não houver mais referências necessárias.

---

## Nova arquitetura

### `personas/`
Status: `NOVA ESTRUTURA` — já possui definições-base próprias.

Responsabilidade: separar os cinco papéis operacionais:

- Jogador Humano;
- Jogador IA;
- Jogador IA Eventual;
- Opositor;
- Narrador.

A pasta já define quatro personas executadas pela IA e mantém o Jogador Humano como papel externo.

### `resolucao/`
Status: `NOVA ESTRUTURA`.

Responsabilidade futura: intenção versus resultado, ciclo, capacidades, dificuldade, social, investigação, combate e demais formas de resolução.

### `agencia/`
Status: `NOVA ESTRUTURA`.

Responsabilidade futura: autonomia, ciclo fora da câmera, conhecimento separado e ativação de jogadores eventuais.

### `narracao/`
Status: `NOVA ESTRUTURA`.

Responsabilidade futura: apresentação da ficção, ritmo, ponto de parada, voz, foco e limites de controle narrativo.

### `persistencia/`
Status: `NOVA ESTRUTURA`.

Responsabilidade futura: estado, STATUS, cronologia, progressão, ficha, livro, material reservado e fechamento de capítulo.

### `operacao/`
Status: `NOVA ESTRUTURA`.

Responsabilidade futura: checklist, modo RPG, ordem de consulta e aplicação das demais áreas.

---

## Mapa inicial — arquivos antigos

| Arquivo antigo | Área futura principal | Status atual |
|---|---|---|
| `README.md` | `resolucao/` + roteamento geral | ANTIGA AINDA VÁLIDA |
| `00-LEIA-PRIMEIRO.md` | `operacao/` | ANTIGA AINDA VÁLIDA |
| `ciclo-de-jogadores.md` | `resolucao/` | ANTIGA AINDA VÁLIDA |
| `agencia-de-personagens.md` | `agencia/` | ANTIGA AINDA VÁLIDA |
| `narracao-e-escrita-padrao.md` | `narracao/` | ANTIGA AINDA VÁLIDA |
| `modo-rpg.md` | `operacao/` | ANTIGA AINDA VÁLIDA |
| `checklist-do-narrador.md` | `operacao/` | ANTIGA AINDA VÁLIDA |
| `protocolo-de-fechamento-de-capitulo.md` | `persistencia/` | ANTIGA AINDA VÁLIDA |

Outros arquivos encontrados durante a revisão devem ser adicionados a esta tabela antes de serem substituídos.

---

## Regra contra duplicação contraditória

Durante a migração pode existir conteúdo semelhante em dois lugares.

Quando isso ocorrer:

1. o mapa acima deve indicar qual arquivo ainda prevalece;
2. a versão nova deve declarar se está em teste ou se já substituiu a antiga;
3. não manter duas regras incompatíveis simultaneamente como igualmente canônicas;
4. correção explícita mais recente do usuário continua tendo prioridade máxima.

---

## Ordem sugerida de revisão

1. `personas/opositor/` — nova função que precisa de definição detalhada.
2. `personas/narrador/` — retirar do Narrador a função de fabricar oposição.
3. `resolucao/` — reconstruir ciclo e resolução com as personas separadas.
4. `personas/jogador-ia/` e `personas/jogador-ia-eventual/` — refinar agência operacional com exemplos práticos.
5. `agencia/` — separar autonomia, conhecimento e ciclo fora da câmera.
6. `operacao/` — reconstruir checklist a partir da arquitetura já estabilizada.
7. `narracao/` e `persistencia/` — migrar regras de apresentação e registro sem alterar comportamento válido.

> **A estrutura nova cresce ao lado da antiga até conseguir substituí-la com segurança.**
