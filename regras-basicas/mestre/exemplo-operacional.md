# Exemplo Operacional do Mestre

Status: REFORMULAÇÃO / NÃO IMPLEMENTADO

Este arquivo demonstra como a persona `NARRADOR` usa o manual durante uma janela real.

O objetivo não é criar uma cena canônica. É mostrar o procedimento.

## Situação inicial

Fatos já estabelecidos:

```text
- Helena está em casa.
- Helena foi envenenada sem saber.
- o veneno produz seu primeiro efeito em 1 hora.
- Raul está dormindo em outro cômodo.
- nenhuma força adversarial está presente no local.
```

Registro relevante:

```text
veneno
→ primeiro efeito em 1 hora.
```

## Declarações

```text
JOGADOR HUMANO — Helena
→ vou passar a tarde estudando os documentos.

JOGADOR IA — Raul
→ continuo dormindo.

JOGADOR IA EVENTUAL
→ nenhuma personagem assumida nesta janela.

OPOSITOR
→ o veneno registrado produz efeito em 1 hora.
```

A janela está completa.

## 1. Separar intenção de fato

```text
Helena pretende
→ estudar a tarde inteira.

Raul pretende
→ continuar dormindo.

Opositor
→ não criou ação nova.
→ fiscalizou um prazo já registrado.
```

Fatos relevantes:

```text
Helena pode estudar.
Raul está dormindo.
O veneno existe.
O prazo vence em 1 hora.
```

## 2. Possibilidade

Estudar é possível.

Continuar dormindo é possível.

O efeito do veneno já foi estabelecido como automático.

Nenhuma impossibilidade nova existe.

## 3. Disputa

Não existe disputa entre estudar e dormir.

O veneno não está tentando uma decisão voluntária contra Helena; seu efeito já pertence ao estado da ficção.

Portanto, não existe teste apenas porque o momento é importante.

Se a regra específica do veneno exigir resistência, aplicar essa regra quando o prazo chegar.

## 4. Tempo

A intenção de Helena cobre várias horas.

Mas existe um prazo anterior:

```text
1 hora
→ veneno produz efeito.
```

O Mestre não pode narrar a tarde inteira.

A sentença só pode avançar até esse ponto.

## 5. Estabelecer a sentença antes de narrar

O Mestre estabelece:

```text
- Helena estuda durante 1 hora.
- Raul continua dormindo durante esse período.
- após 1 hora, o prazo do veneno chega.
- o efeito aplicável do veneno ocorre conforme sua regra.
- a condição de Helena muda.
- a intenção original de estudar a tarde inteira pode ser interrompida pelo novo estado.
```

Se o efeito exigir nova escolha, a sentença termina ali.

## 6. Narração

Possível apresentação:

Helena espalha os documentos pela mesa e começa pelos relatórios mais antigos. A casa permanece quieta; do outro cômodo, Raul não dá sinal de ter acordado.

A primeira hora passa entre anotações, páginas marcadas e comparações repetidas.

Então a mudança vem de repente.

Uma pressão incômoda se forma no estômago, seguida por uma onda de fraqueza que sobe pelos braços. As letras diante dela perdem nitidez por um instante.

Ela ainda está sentada diante dos documentos, mas a tarde já não é mais a mesma.

## 7. Parada

O Mestre para porque a nova condição pode mudar a próxima decisão voluntária de Helena.

```text
NOVA SITUAÇÃO
→ abrir nova janela
```

Não continua automaticamente:

```text
"Helena decide deitar."
"Helena chama Raul."
"Helena tenta descobrir o que aconteceu."
```

Essas são novas decisões da cadeira correspondente.

## 8. Registro

Depois da sentença, registrar apenas o que precisa persistir.

Exemplo:

```text
- passou 1 hora.
- primeiro efeito do veneno ocorreu.
- condição atual de Helena foi alterada conforme a regra do veneno.
- Raul continua dormindo, se isso ainda for relevante.
```

A intenção de estudar a tarde inteira não é registrada como concluída porque foi interrompida antes.

---

# Segundo exemplo — disputa de percepção

## Declarações

```text
JOGADOR IA — A
→ tento sair da sala sem ser percebida pelo guarda.

OPOSITOR — Guarda
→ permaneço atento à porta.
```

## Julgamento

```text
possível?
→ sim.

disputa?
→ sim.

Furtividade contra Percepção
→ teste obrigatório.
```

A resolução segue `0.1-resolucao.md`:

```text
2d6 + Furtividade - Percepção + situação
```

Suponha que o resultado final seja **9**.

```text
7–9
→ sucesso com consequência
```

O Mestre precisa determinar o significado concreto antes de escrever.

Exemplo possível, se coerente com a situação:

```text
- A consegue sair da sala.
- o guarda percebe movimento tarde demais para impedir a saída imediata.
- ele não identifica todos os detalhes da fuga.
```

O sucesso principal não pode ser retirado, e a consequência deve nascer do risco concreto da tentativa furtiva.

## Narração

A abre a porta apenas o bastante para passar pelo vão e desliza para o corredor.

Por um segundo, funciona.

O guarda vira o rosto quando ela já está alguns passos adiante. Ele não vê de onde exatamente ela saiu, mas vê o bastante para saber que alguém acabou de cruzar o corredor.

A vantagem do silêncio terminou.

## Parada

Se agora existe uma nova decisão para A e para o guarda, abrir nova janela.

---

# Terceiro exemplo — resultado evidente

```text
JOGADOR
→ pego o copo que está diante de mim.
```

Fatos:

```text
- copo ao alcance.
- mãos livres.
- nenhuma oposição.
- nenhuma condição impede o movimento.
```

Julgamento:

```text
possível
→ sim.

disputa
→ não.

incerteza real
→ não.

resultado
→ evidente.
```

Narração:

```text
Ela pega o copo.
```

Não existe motivo para rolagem, cálculo ou dramatização adicional.

## Regra final

> **O exemplo operacional deve ser lido como modelo de raciocínio: primeiro fatos e declarações, depois possibilidade, disputa e incerteza, depois sentença, depois prosa, depois parada e Registro.**
