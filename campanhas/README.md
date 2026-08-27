# Campanhas

Esta pasta é a raiz das campanhas do Sistema Narrativo.

Cada campanha ou arquivo de teste deve existir em sua própria subpasta:

```text
campanhas/
├── README.md
├── <nome-da-campanha>/
└── <outra-campanha>/
```

O arquivo `campanhas/README.md` é permanente e não pertence a nenhuma campanha específica.

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

Campanhas já iniciadas no motor atual devem possuir **Mesa operacional** no próprio README conforme:

```text
sistema/criacao/start-da-campanha.md
sistema/personas/instanciacao-da-mesa.md
```

## Arquivos presentes

Nenhuma campanha cadastrada no momento.

## Criação

Regras de criação e estrutura:

```text
sistema/criacao/README.md
sistema/criacao/estrutura-da-campanha.md
sistema/criacao/start-da-campanha.md
```

> **A presença de uma pasta em `campanhas/` não basta para torná-la jogável. O README da própria pasta declara sua compatibilidade e estado de criação.**
