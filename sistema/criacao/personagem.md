# Criação e Revisão de Personagens

Status: APROVADO

Este arquivo define **o procedimento para construir e revisar uma ficha** durante a criação da campanha.

Ele complementa `README.md`. As definições estáveis da personagem pertencem a `../personagem/`; este arquivo apenas organiza como essas definições são propostas, aprovadas e registradas.

> **`criacao/` conduz o processo. `personagem/` define o conteúdo da ficha.**

## Princípio central

A ficha nasce completa em estrutura e mínima em conteúdo.

Antes da revisão, preencher somente:

```text
NOME
IMPORTÂNCIA
CONTROLE
```

Se alguma dessas informações já foi fornecida, não perguntar novamente.

O modelo da ficha pertence a `../personagem/ficha.md`. O significado operacional de `CONTROLE` pertence a `../personas/`.

## Método de criação assistida

```text
base disponível
→ proposta coerente
→ correção do JOGADOR HUMANO
→ reapresentação quando necessária
→ aprovação explícita
→ persistência do bloco aprovado
```

A proposta pode usar Conceito, versão canônica escolhida, fatos já discutidos, relações estabelecidas e blocos anteriores aprovados.

> **Proposta não é fato. Somente conteúdo aprovado entra na ficha.**

## Campo desconhecido

Nunca usar `[0]` como marcador de pendência.

```text
Controle [ ] → ainda não definido
Controle [0] → valor mecanicamente definido
```

Perícia ainda não escolhida simplesmente não aparece.

## Ordem da revisão

Cada ficha é revisada em cinco blocos:

```text
1 - Identidade e Conceito
2 - Patamar, Atributos e Perícias
3 - Poderes e capacidades
4 - Traços, Recursos e relações
5 - Conferência final
```

Em todos os blocos:

```text
propor
→ discutir/corrigir
→ aprovar
→ salvar somente o aprovado
→ avançar
```

### Bloco 1 — Identidade e Conceito

Revisar somente o que for relevante para reconhecer e interpretar a personagem, como:

- nome real;
- idade;
- aparência;
- estilo;
- origem/natureza;
- Conceito;
- descrição.

### Bloco 2 — Patamar, Atributos e Perícias

Usar as fontes:

```text
calibração  → calibracao.md
Patamar     → ../personagem/patamar.md
Atributos   → ../personagem/atributos.md
Perícias    → ../personagem/pericias.md
```

Aplicar:

```text
Pontos de Atributo = Patamar × 4
Limite inicial = Patamar + 2
máximo permanente = [7]
```

Definir os seis Atributos e registrar apenas Perícias realmente pertencentes à personagem.

Depois de aprovados os Atributos permanentes, calcular:

```text
Vida Máxima → ../resolucao/vida.md
Mana Máxima → ../resolucao/mana.md
```

### Bloco 3 — Poderes e capacidades

Registrar quais Poderes pertencem ao arsenal funcional da personagem.

A posse pertence a `../personagem/poderes.md`; a mecânica concreta e os Hubs pertencem a `../resolucao/poderes/`.

Não criar Poder para ação comum já coberta por Atributos, equipamento ordinário e ficção.

### Bloco 4 — Traços, Recursos e relações

Usar:

```text
Traços      → ../personagem/tracos.md e ../personagem/tracos/
Relações    → ../personagem/relacoes.md
RECURSOS    → ../personagem/ficha.md
```

Vícios e Corrupções usam a economia definida em `../personagem/patamar.md`.

Informações já aprovadas reaparecem automaticamente; não perguntar de novo.

### Bloco 5 — Conferência final

Revisar a ficha inteira e completar apenas informações úteis para interpretação e continuidade, como:

- personalidade e tendências;
- desejos/objetivos;
- medos/limites;
- conhecimento relevante;
- história consolidada relevante.

Conferir:

- Conceito × Patamar coerentes;
- pontos e limites de Atributos válidos;
- Perícias sem graduação;
- Vida/Mana derivadas corretamente;
- Poderes sem grau genérico `[1–5]`;
- ausência de ENERGIA universal;
- ausência de campos inventados ou não aprovados.

A regra sobre o que merece permanecer na ficha pertence a `../persistencia/relevancia-da-ficha.md`.

## Salvamento durante a revisão

Cada bloco aprovado é persistido antes de avançar.

Conteúdo em discussão, alternativas rejeitadas e rascunhos não entram como cânone.

O destino concreto da ficha depende de `estrutura-da-campanha.md` e das regras de `../persistencia/`.

## Pareamento

Depois que todas as fichas iniciais com agência estiverem aprovadas, aplicar `pareamento.md` antes de definir a situação inicial.

## Estado de aprovação

Durante a revisão:

```text
Status: PENDENTE DE REVISÃO
```

Depois do Bloco 5 aprovado:

```text
Status: APROVADO
```

## Alterações posteriores

Depois que a criação terminou, mudanças permanentes deixam de ser procedimento de criação e passam a seguir `../persistencia/atualizacao-de-ficha.md`.

## Regra final

> **Criação organiza proposta, aprovação e salvamento. As regras que dizem o que Patamar, Atributos, Perícias, Poderes e Traços são permanecem em `personagem/`.**
