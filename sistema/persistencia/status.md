# STATUS

Status: APROVADO

STATUS registra **como uma peça está agora**.

Ele não redefine mecânicas nem autoridade. Sua função é preservar valores e condições atuais já estabelecidos.

```text
FICHA
→ quem a peça é

STATUS
→ como ela está neste momento
```

## Conteúdo possível

Quando relevantes:

```text
Vida atual / máxima
Mana atual / máxima
Trama atual, quando aplicável
Status e condições temporárias
Efeitos Ativos
Barreiras
alterações temporárias de Atributo
local / posição relevante
outros estados temporários necessários à continuidade
```

Nem toda peça precisa de todos os campos.

> **STATUS guarda somente o que ainda pode importar agora.**

## Fontes mecânicas

STATUS registra resultados; não os recalcula.

```text
Vida                 → ../resolucao/vida.md
Dano                  → ../resolucao/combate-e-dano.md
recuperação           → ../resolucao/recuperacao-da-vida.md
Mana                  → ../resolucao/mana.md
Trama                 → ../personagem/trama.md
Status mecânicos      → ../resolucao/status/
Poderes/Efeitos       → ../resolucao/poderes/
```

Exemplo:

```text
Vida [18/29]
Mana [9/24]
Trama [27]
Cego — Cena
Barreira [7/15]
```

`ENERGIA` e `Bateria [1–5]` não são campos universais atuais.

## Status mecânicos e condições

As famílias mecânicas pertencem a `../resolucao/status/`.

Aqui se registra apenas aquilo que continua ativo e, quando necessário, duração ou informação operacional suficiente para retomar corretamente.

Não inventar nova penalidade no momento do registro.

## Efeitos ativos

Quando uma manifestação temporária precisa continuar existindo, registrar somente o necessário:

- origem/Poder;
- duração restante;
- configuração ainda relevante;
- alvo ou área;
- Barreira;
- alteração temporária;
- outro dado necessário à continuidade.

## Alterações temporárias de Atributo

Exemplo:

```text
Potência +2 temporário — Cena
Controle -1 temporário — 3 Turnos
```

Essas alterações não recalculam Vida Máxima ou Mana Máxima.

## Local e posição

Registrar apenas no nível necessário para evitar contradição ou alterar futuras decisões/resoluções.

## Entrada, mudança e saída

```text
ENTRA
→ novo estado relevante passa a existir

MUDA
→ valor ou condição atual muda

SAI
→ deixa de existir ou de importar para continuidade
```

Quando algo termina, remover do STATUS em vez de transformá-lo em histórico.

## Onde o STATUS vive

Na campanha, STATUS persistente fica normalmente dentro de:

```text
campanhas/<nome>/estado/atual.md
```

conforme `estado-atual.md`.

Não é necessário criar `status.md` dentro de cada campanha.

## Fronteiras

```text
FICHA
→ capacidades consolidadas

RESOLUÇÃO
→ determina resultados e valores

OPERAÇÃO
→ determina quando atualizar durante o fluxo

PROGRESSÃO
→ consequência passada ainda causalmente viva

LIVRO
→ histórico do que aconteceu
```

Autoridade sobre declarações pertence a `../personas/`.

> **STATUS não explica a regra nem decide o fato; preserva o presente depois que ele foi estabelecido.**

## Regra final

> **STATUS é o retrato atual de uma peça dentro da memória da campanha.**
