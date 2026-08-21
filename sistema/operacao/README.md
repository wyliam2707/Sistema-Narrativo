# Operação

Esta pasta reúne as regras que respondem à pergunta:

> **O que precisa ser verificado enquanto o RPG está rodando para que o sistema seja aplicado corretamente?**

## Estado da migração

A estrutura nova está sendo construída sem apagar os arquivos antigos.

Enquanto uma regra ainda não tiver sido reescrita e aprovada nesta pasta, o arquivo antigo correspondente em `sistema/` continua válido.

## Responsabilidades desta área

Esta pasta deverá concentrar, progressivamente:

- modo RPG;
- checklist operacional;
- ordem de consulta;
- quando abrir nova janela de resolução;
- quando revisar agentes fora da câmera;
- quando atualizar STATUS;
- quando consultar fichas, estado, progressão e material reservado;
- prevenção de conflitos entre regras de áreas diferentes.

## Arquivos antigos ainda em uso

- `../modo-rpg.md` — procedimento operacional atual.
- `../checklist-do-narrador.md` — checklist atual.
- `../00-LEIA-PRIMEIRO.md` — orientação geral de entrada no sistema.

## Princípio

`operacao/` não deve duplicar regras de resolução, agência ou narração.

Ela funciona como camada de execução e roteamento:

```text
quem decide?        → personas/
como age sozinho?   → agencia/
o que acontece?     → resolucao/
como mostrar?       → narracao/
o que permanece?    → persistencia/
como aplicar tudo?  → operacao/
```

> **Operação lembra o que consultar; não redefine silenciosamente as outras áreas.**
