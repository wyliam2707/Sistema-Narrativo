# Narração

Status: APROVADO

Esta pasta responde à pergunta:

> **Como um acontecimento já julgado é apresentado como cena?**

`narracao/` cuida da forma. Ela não decide quem age, não altera resultado, não cria oposição e não redefine persistência.

## Estrutura canônica

```text
narracao/
├── README.md
├── apresentacao-da-cena.md
├── fala-e-interioridade.md
├── ritmo-e-descricao.md
├── dramatizacao-e-resumo.md
└── exemplo-de-estilo.md
```

### `apresentacao-da-cena.md`

Usar para:

- transformar sentença em ficção;
- manter clareza causal e espacial;
- apresentar somente informação perceptível;
- manter mecânica fora da prosa;
- respeitar o limite de parada definido por `../operacao/`.

### `fala-e-interioridade.md`

Usar para:

- `[Nome] — fala`;
- `[Nome, pensa] — pensamento`;
- diferença entre interioridade no RPG ao vivo e no livro;
- voz individual;
- subtexto;
- prevenção de vazamento de conhecimento interno.

### `ritmo-e-descricao.md`

Usar para:

- terceira pessoa próxima;
- parágrafos e ritmo;
- descrição seletiva;
- atmosfera;
- ação clara;
- cotidiano;
- romance e vínculos;
- humor.

### `dramatizacao-e-resumo.md`

Usar para decidir:

- o que precisa ser vivido em cena;
- o que pode ser resumido;
- quando sair do resumo e voltar à dramatização;
- como direção narrativa altera ênfase sem alterar fatos;
- como condensar sem atravessar decisões ainda abertas.

### `exemplo-de-estilo.md`

Referência neutra para calibrar ritmo, terceira pessoa próxima, descrição seletiva, diálogo, subtexto e alternância entre dramatização e resumo.

Não cria regra nova. Quando o exemplo divergir de uma regra canônica, prevalece a regra canônica.

## Relação com as outras áreas

```text
quem decide?                 → ../personas/
o que realmente acontece?    → ../resolucao/
quando parar ou abrir janela? → ../operacao/
o que permanece?             → ../persistencia/
como mostrar?                → narracao/
```

> **Narração apresenta a sentença. Não participa da disputa.**

## Direção narrativa da campanha

O padrão desta pasta é herdado por toda campanha.

A direção narrativa local registrada no `README.md` da campanha pode complementar ou alterar escolhas de estilo como tom, foco, ritmo, humor, romance, sensualidade e atmosfera.

Ela não altera agência, fatos, resolução ou consequência.

> **A campanha define o estilo local; o sistema fornece o padrão herdado.**

## RPG ao vivo e Livro

```text
RPG AO VIVO
→ apresenta somente aquilo que a situação e a perspectiva permitem.
→ preserva decisões ainda pertencentes à mesa.
→ não revela automaticamente interioridade das outras peças.

LIVRO
→ consolida depois o que realmente aconteceu.
→ pode reconstruir transições e ampliar interioridade sem mudar o cânone.
```

As regras de consolidação do Livro pertencem a `../persistencia/`.

## Arquivos legados na raiz

Os arquivos antigos:

```text
../narracao-e-escrita-padrao.md
../exemplo-de-estilo.md
```

permanecem preservados temporariamente como legado.

O exemplo já possui cópia canônica dentro desta pasta. As regras operacionais de narração agora pertencem aos arquivos de `narracao/`.

Formulações antigas que contradigam `personas/`, `operacao/`, `resolucao/`, `persistencia/` ou estes arquivos devem ser ignoradas.

Os arquivos antigos só devem ser removidos após confirmação explícita.

## Regra final

> **README roteia. Arquivos especializados guardam as regras. Narração mostra com clareza aquilo que já foi decidido sem tomar para si decisões que pertencem a outras cadeiras.**