# Comandos Administrativos de Campanha

Este arquivo define comandos de manutenção que alteram a estrutura persistente das campanhas. Eles não fazem parte da resolução narrativa do RPG.

Operações destrutivas exigem confirmação explícita.

---

## 1. Apagar uma campanha

Comando inicial:

```text
APAGAR CAMPANHA: <nome exato da campanha>
```

Ao receber esse comando, o narrador ou IA **não deve apagar imediatamente**.

Primeiro deve:

1. procurar exatamente `aventuras/<nome da campanha>/`;
2. confirmar que a campanha existe;
3. informar claramente que toda a pasta da campanha será apagada, incluindo personagens, mundo, relações, Progressão, cronologia, estado, capítulos e arquivos de criação;
4. pedir uma segunda confirmação usando o nome exato.

Formato obrigatório da confirmação:

```text
CONFIRMAR EXCLUSÃO: <nome exato da campanha>
```

Somente depois dessa confirmação exata a exclusão pode ser executada.

---

## 2. Proteções obrigatórias

O comando de exclusão deve obedecer a todas estas regras:

- nunca interpretar uma frase comum, reclamação ou comentário como pedido de exclusão;
- exigir o nome exato da campanha;
- exigir uma segunda confirmação explícita;
- atuar somente dentro de `aventuras/<nome>/`;
- nunca apagar `sistema/`;
- nunca apagar a raiz do repositório;
- nunca apagar outra campanha com nome diferente;
- se o nome for ambíguo ou não existir exatamente, não apagar nada;
- se a confirmação não corresponder exatamente à campanha encontrada, não apagar nada.

> **Pedido de exclusão identifica a campanha. Confirmação explícita autoriza a destruição.**

---

## 3. Exemplo

Jogador:

```text
APAGAR CAMPANHA: Sombras de Eldoria
```

Sistema:

```text
Campanha encontrada: Sombras de Eldoria.
Esta operação apagará definitivamente todos os arquivos em aventuras/Sombras de Eldoria/.
Para confirmar, escreva:
CONFIRMAR EXCLUSÃO: Sombras de Eldoria
```

Jogador:

```text
CONFIRMAR EXCLUSÃO: Sombras de Eldoria
```

Somente então a campanha pode ser removida.

---

## 4. Cancelamento

Qualquer resposta diferente da confirmação exata cancela a exclusão.

O jogador também pode escrever:

```text
CANCELAR EXCLUSÃO
```

Nesse caso, nenhuma alteração deve ser feita.

---

## Regra final

> **Nunca destruir uma campanha por inferência. Exclusão definitiva exige comando explícito, campanha encontrada e confirmação explícita com o mesmo nome.**
