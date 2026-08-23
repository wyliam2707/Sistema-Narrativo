# Comandos Administrativos de Campanha

Status: APROVADO

Este arquivo define operações administrativas que alteram a estrutura persistente das campanhas.

Elas não fazem parte da resolução narrativa do RPG.

> **Operação administrativa não é ficção. Operação destrutiva exige confirmação explícita.**

## Apagar uma campanha

Comando inicial:

```text
APAGAR CAMPANHA: <nome exato da campanha>
```

Esse comando **não autoriza exclusão imediata**.

Antes de apagar:

1. localizar exatamente `campanhas/<nome da campanha>/`;
2. confirmar que a campanha existe;
3. informar que toda a pasta será apagada, incluindo personagens, estado, mundo, material reservado e livro;
4. exigir uma segunda confirmação com o mesmo nome exato.

Formato da confirmação:

```text
CONFIRMAR EXCLUSÃO: <nome exato da campanha>
```

Somente depois dessa confirmação exata a exclusão pode ser executada.

## Proteções obrigatórias

Nunca:

- interpretar frase comum, reclamação ou comentário como pedido de exclusão;
- apagar sem localizar a campanha exata;
- aceitar nome ambíguo como confirmação;
- apagar `sistema/`;
- apagar a raiz do repositório;
- apagar outra campanha por consequência indireta;
- aplicar este comando atual automaticamente a material legado em `aventuras/`.

Se o nome não existir exatamente ou a confirmação não corresponder ao alvo encontrado, não apagar nada.

> **Pedido de exclusão identifica o alvo. Confirmação explícita autoriza a destruição.**

## Cancelamento

Qualquer desistência antes da confirmação encerra a operação sem alteração.

Comando explícito possível:

```text
CANCELAR EXCLUSÃO
```

## Exemplo

```text
JOGADOR
APAGAR CAMPANHA: Sombras de Eldoria

SISTEMA
Campanha encontrada: Sombras de Eldoria.
A operação apagará definitivamente campanhas/Sombras de Eldoria/.
Para confirmar:
CONFIRMAR EXCLUSÃO: Sombras de Eldoria

JOGADOR
CONFIRMAR EXCLUSÃO: Sombras de Eldoria
```

Somente então a exclusão pode ser executada.

## Regra final

> **Nunca destruir uma campanha por inferência. Exclusão definitiva exige alvo exato, existência verificada e confirmação explícita com o mesmo nome.**
