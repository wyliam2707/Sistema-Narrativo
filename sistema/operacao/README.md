# Operação

Status: REFERÊNCIA PRINCIPAL

Esta pasta reúne as regras que respondem à pergunta:

> **O que precisa ser verificado enquanto o RPG está rodando para que o sistema seja aplicado corretamente?**

## Responsabilidades desta área

Esta pasta concentra:

- ordem das declarações;
- ordem de consulta;
- quando abrir nova janela de resolução;
- quando o OPOSITOR movimenta o cenário;
- quando o NARRADOR consulta fichas, regras, cenário e situação;
- quando interromper a resolução e devolver controle ao jogador;
- quando registrar consequências;
- quando revisar agentes fora da câmera;
- prevenção de conflitos entre regras de áreas diferentes.

## Arquivo principal

- [`ciclo-de-cena.md`](ciclo-de-cena.md) — ordem operacional atual das personas em uma janela de cena, incluindo declarações dos jogadores, movimento do OPOSITOR, julgamento do NARRADOR e registro do resultado.

Quando houver conflito sobre a ordem das personas ou o ciclo de uma janela, `ciclo-de-cena.md` é a referência atual.

## Porta de entrada

`sistema/00-LEIA-PRIMEIRO.md` é o roteador operacional atual do sistema.

Ele não é mais tratado como uma fonte histórica subordinada a arquivos antigos. Sua função é encaminhar a IA para as áreas atuais sem reintroduzir regras já substituídas.

Fluxo de entrada:

```text
NOVA CAMPANHA
→ sistema/criacao/README.md

CONTINUAR
→ campanhas/<nome>/README.md
```

## Arquivos antigos ainda úteis para migração

Os documentos abaixo permanecem preservados apenas nos pontos ainda não substituídos:

- `../modo-rpg.md`;
- `../checklist-do-narrador.md`.

Eles não prevalecem contra `ciclo-de-cena.md`, `../personas/`, `../persistencia/` ou outra regra nova explicitamente aprovada.

O ciclo antigo já foi removido após substituição por `ciclo-de-cena.md` e `../personas/`.

## Registro do resultado

Quando a operação manda registrar STATUS, Progressão ou outra consequência, a persistência concreta segue `../persistencia/README.md` e a estrutura definida em `../criacao/estrutura-da-campanha.md`.

Na campanha atual, o retrato operacional é:

```text
campanhas/<nome>/estado/atual.md
```

Não criar automaticamente arquivos separados de STATUS, Progressão ou cronologia apenas porque esses conceitos existem no sistema.

## Princípio

`operacao/` não duplica regras de personagem, resolução, agência, narração, criação ou persistência.

Ela funciona como camada de execução e roteamento:

```text
como criar campanha?          → criacao/
quem é / do que é capaz?      → personagem/
quem decide?                  → personas/
quem move o cenário?          → personas/opositor/
como age sozinho?             → agencia/
o que acontece?               → resolucao/
como mostrar?                 → narracao/
o que permanece e onde salvar?→ persistencia/
como aplicar tudo?            → operacao/
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
