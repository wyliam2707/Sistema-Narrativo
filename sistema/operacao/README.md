# Operação

Status: APROVADO

Esta pasta responde à pergunta:

> **Em que ordem o sistema é aplicado enquanto o RPG está rodando?**

`operacao/` não cria uma segunda versão das regras. Ela organiza **quando cada área entra em cena**.

## Estrutura canônica

```text
operacao/
├── README.md
└── ciclo-de-cena.md
```

- `README.md` — porta de entrada e roteador da operação.
- `ciclo-de-cena.md` — sequência operacional completa de uma janela significativa de cena.

Quando houver dúvida sobre ordem de atuação, abertura de nova janela, interrupção ou devolução de controle, consultar `ciclo-de-cena.md`.

## Imagem mental

A operação usa a mesma imagem de `../personas/`:

```text
JOGADORES
→ defesa das próprias peças.

OPOSITOR
→ promotoria.

NARRADOR
→ juiz.
```

O ciclo essencial é:

```text
JOGADORES declaram
↓
OPOSITOR apresenta movimento, gancho, pressão ou oposição
↓
NARRADOR JULGA
↓
NARRADOR NARRA A SENTENÇA
↓
NARRADOR REGISTRA
↓
NOVA SITUAÇÃO
```

> **O NARRADOR não move a disputa. Consultar fatos faz parte de JULGAR, não constitui uma etapa de iniciativa própria.**

## O que esta pasta coordena

`operacao/` coordena:

- quando uma declaração é necessária;
- quando uma intenção anterior continua suficiente;
- quando o JOGADOR IA ou JOGADOR IA EVENTUAL precisa decidir;
- quando o OPOSITOR pode puxar um gancho ou apresentar oposição;
- quando o NARRADOR deve julgar;
- até onde a sentença pode ser narrada sem roubar nova decisão;
- quando uma nova janela precisa abrir;
- quando o resultado precisa ser registrado.

## Roteamento para as outras áreas

```text
como criar campanha?             → ../criacao/
quem é / do que é capaz?         → ../personagem/
quem decide?                     → ../personas/
como preservar vontade própria?  → ../agencia/
como calcular o resultado?       → ../resolucao/
como apresentar a cena?          → ../narracao/
o que permanece e onde salvar?   → ../persistencia/
como aplicar tudo em sequência?  → operacao/
```

Não copiar para `operacao/` fórmulas de resolução, ficha, estilo narrativo ou regras de persistência já definidas nessas áreas.

## Registro do resultado

O NARRADOR registra somente o que a sentença tornou verdadeiro.

O retrato operacional principal da campanha é:

```text
campanhas/<nome>/estado/atual.md
```

Pontas disponíveis ao OPOSITOR podem ficar em:

```text
campanhas/<nome>/mestre/ganchos-do-opositor.md
```

Fatos estáveis pertencem a `mundo/`, mudanças estáveis de personagem à ficha quando cabíveis, e história ocorrida a `livro/` conforme `../persistencia/`.

Não criar automaticamente arquivos paralelos de STATUS, Progressão, cronologia ou checklist apenas porque esses conceitos aparecem durante uma resolução.

## Arquivos legados

Os arquivos antigos:

```text
../modo-rpg.md
../checklist-do-narrador.md
```

permanecem preservados temporariamente para revisão histórica, mas **não são fonte operacional**.

Seu conteúdo útil já foi absorvido pelo ciclo atual ou pelas áreas canônicas correspondentes. Quando uma formulação desses arquivos contradizer `operacao/`, `personas/`, `agencia/`, `resolucao/`, `narracao/` ou `persistencia/`, ignorar a formulação antiga.

Eles só devem ser removidos numa etapa posterior de limpeza, após confirmação explícita.

## Porta de entrada do sistema

```text
NOVA CAMPANHA
→ sistema/criacao/README.md

CONTINUAR
→ campanhas/<nome>/README.md
```

`sistema/00-LEIA-PRIMEIRO.md` continua sendo o roteador geral.

## Regra final

> **Operação não decide quem vence nem inventa conteúdo. Ela garante que cada cadeira fale na hora certa, que o juiz só julgue depois das declarações relevantes e que a sentença pare quando voltar a existir uma decisão real.**