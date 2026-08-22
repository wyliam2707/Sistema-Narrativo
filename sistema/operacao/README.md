# Operação

Esta pasta reúne as regras que respondem à pergunta:

> **O que precisa ser verificado enquanto o RPG está rodando para que o sistema seja aplicado corretamente?**

## Estado da migração

A estrutura nova está sendo construída sem apagar os arquivos antigos.

Enquanto uma regra ainda não tiver sido reescrita e aprovada nesta pasta, o arquivo antigo correspondente em `sistema/` continua válido apenas nos pontos ainda não substituídos pela arquitetura nova.

## Responsabilidades desta área

Esta pasta concentra, progressivamente:

- ordem das declarações;
- ordem de consulta;
- quando abrir nova janela de resolução;
- quando o OPOSITOR movimenta o cenário;
- quando o NARRADOR consulta fichas, regras, cenário e situação;
- quando interromper a resolução e devolver controle ao jogador;
- quando registrar STATUS, Progressão e preparações;
- quando revisar agentes fora da câmera;
- prevenção de conflitos entre regras de áreas diferentes.

## Arquivos aprovados nesta área

- [`ciclo-de-cena.md`](ciclo-de-cena.md) — ordem operacional das personas em uma janela de cena, incluindo declarações dos jogadores, movimento do OPOSITOR, julgamento do NARRADOR e registro do resultado.

## Arquivos antigos ainda como fonte de migração

- `../modo-rpg.md` — procedimento operacional antigo; continua fonte para pontos ainda não migrados.
- `../checklist-do-narrador.md` — checklist antigo; continua fonte para pontos ainda não migrados.
- `../00-LEIA-PRIMEIRO.md` — orientação geral antiga de entrada no sistema.

Quando houver conflito sobre a ordem das personas ou o ciclo de uma janela, `ciclo-de-cena.md` é a regra atual aprovada.

## Princípio

`operacao/` não deve duplicar regras de personagem, resolução, agência, narração ou persistência.

Ela funciona como camada de execução e roteamento:

```text
quem é / do que é capaz? → personagem/
quem decide?             → personas/
quem move o cenário?     → personas/opositor/
como age sozinho?        → agencia/
o que acontece?          → resolucao/
como mostrar?            → narracao/
o que permanece?         → persistencia/
como aplicar tudo?       → operacao/
```

O ciclo-base pode ser lembrado assim:

```text
JOGADORES movem suas peças
↓
OPOSITOR move o cenário
↓
NARRADOR organiza
↓
NARRADOR consulta
↓
NARRADOR julga
↓
NARRADOR apresenta e registra
↓
NOVA SITUAÇÃO
```

> **Operação lembra o que consultar e em que ordem agir; não redefine silenciosamente as outras áreas.**
