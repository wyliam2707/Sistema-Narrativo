# Sistema Narrativo

Este repositório separa **o motor do RPG** dos **dados concretos de cada campanha**.

## Estrutura atual

- `sistema/` — regras universais, criação, mecânica, agência, resolução, narração, persistência e operação.
- `campanhas/` — campanhas criadas pelo fluxo atual.
- `aventuras/` — material legado; permanece preservado e não é migrado automaticamente.
- `exemplo/` — material demonstrativo usado apenas como referência.

## Regra fundamental

> **O sistema ensina como criar e operar. A campanha guarda o que foi criado e o que aconteceu.**

Nada específico de uma campanha deve ser gravado como regra universal em `sistema/`.

---

# Como iniciar

Se este repositório for fornecido a um narrador humano ou IA com uma instrução como `inicie`, `vamos jogar`, `abra este sistema` ou equivalente:

1. ler `sistema/00-LEIA-PRIMEIRO.md`;
2. perguntar ao jogador apenas:

> **Nova campanha ou continuar uma campanha existente?**

Não exigir código especial de inicialização. O próprio endereço deste repositório pode servir como porta de entrada.

## NOVA CAMPANHA

Abrir:

```text
sistema/criacao/README.md
```

Esse é o processo canônico atual para criação de novas campanhas.

A nova campanha é criada em:

```text
campanhas/<nome-da-campanha>/
```

A criação registra seu próprio checkpoint no `README.md` da campanha e segue as regras definidas em `sistema/criacao/`.

> **NOVA CAMPANHA → `sistema/criacao/README.md`**

## CONTINUAR CAMPANHA

Consultar as campanhas existentes em:

```text
campanhas/
```

Depois que o jogador escolher uma campanha, abrir:

```text
campanhas/<nome>/README.md
```

O `README.md` da própria campanha indica onde consultar seu conteúdo e, se a criação ainda estiver em andamento, de onde retomá-la.

Não pedir ao jogador que reconte informações que os arquivos da campanha já fornecem.

> **CONTINUAR → `campanhas/<nome>/README.md`**

## Material legado

Campanhas antigas ainda armazenadas em `aventuras/` permanecem preservadas.

Não apagar, mover, converter ou reestruturar esse material automaticamente.

Documentos antigos de sistema completamente substituídos só podem ser removidos durante limpeza após revisão e confirmação explícita. As referências atuais estão nas subpastas de `sistema/`.

---

## Consultar exemplo prático

Para consultar o exemplo demonstrativo, abrir `exemplo/README.md` e seguir sua própria ordem de leitura.

O exemplo é somente referência. Não deve ser listado como campanha existente, continuado automaticamente nem copiado para uma campanha real.

---

## Comandos administrativos

Operações de manutenção ficam separadas do fluxo normal de jogo.

Para exclusão de campanha e demais procedimentos administrativos, consultar:

```text
sistema/operacao/comandos-administrativos.md
```

Nenhuma exclusão pode atingir `sistema/`, a raiz do repositório ou outra campanha por consequência indireta.

---

## Continuidade

Para iniciar ou continuar uma campanha, as fontes persistentes da própria campanha prevalecem sobre memória vaga de conversas anteriores.

> **O link abre o sistema. O sistema pergunta Nova ou Continuar. Os arquivos dizem o resto.**