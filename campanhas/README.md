# Campanhas

Esta pasta é a raiz de **todos os dados vivos das campanhas** do Sistema Narrativo.

As regras ficam em `regras-basicas/`.

Tudo que for verdade específica de uma campanha deve ser salvo dentro de sua própria pasta em `campanhas/<nome>/`.

```text
regras-basicas/
→ regras, procedimentos e modelos

campanhas/<nome>/
→ estado real da mesa
```

## O que pertence à campanha

Podem e devem ser preservados aqui, conforme a estrutura de cada campanha:

- fichas reais;
- personagens;
- estado atual;
- Vida, Mana, condições e recursos;
- conhecimento das personagens;
- relações;
- mundo e cenário;
- acontecimentos estabelecidos;
- processos em andamento;
- prazos;
- eventos futuros já julgados;
- planos e registros do Opositor;
- registros do Narrador;
- capítulos e livro;
- qualquer outra verdade que precise continuar existindo naquela campanha.

> **Se é uma verdade da mesa e não uma regra do sistema, pertence a `campanhas/<nome>/`.**

## Estrutura

Cada campanha ou arquivo de teste deve existir em sua própria subpasta:

```text
campanhas/
├── README.md
├── <nome-da-campanha>/
└── <outra-campanha>/
```

A estrutura interna pode conter áreas como:

```text
campanhas/<nome>/
├── README.md
├── estado/
├── personagens/
├── mundo/
├── mestre/
├── opositor/
└── livro/
```

Nem toda campanha precisa usar exatamente todas essas pastas, mas nenhum dado vivo deve ser deslocado para `regras-basicas/` apenas para ser lembrado.

Os arquivos podem permanecer visíveis e fáceis de localizar para inspeção e ajuste manual.

Restrições como `reservado` indicam somente **quem pode usar aquela informação dentro da ficção**, não quem pode abrir o arquivo no repositório.

## Regra para continuar

Antes de oferecer uma pasta ao jogador como campanha continuável, abrir o `README.md` dela.

```text
CRIAÇÃO: EM ANDAMENTO
→ campanha atual
→ pode retomar a criação pelo checkpoint

CRIAÇÃO: CONCLUÍDA
+ Mesa operacional válida
+ sem marca de incompatibilidade
→ campanha atual
→ pode continuar

TESTE / LEGADO / INCOMPATÍVEL
→ não oferecer como campanha jogável por padrão
→ não continuar silenciosamente
→ migrar somente se o jogador pedir
```

Campanhas já iniciadas no motor atual podem manter referências antigas enquanto a reformulação não for concluída.

## Arquivos presentes

- Corvo Estelar — CRIAÇÃO: EM ANDAMENTO

## Regra final

> **`regras-basicas/` explica como jogar. `campanhas/<nome>/` guarda tudo que aconteceu, existe, está em andamento ou está previsto naquela campanha.**