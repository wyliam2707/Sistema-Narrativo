# Registro Reservado do Opositor

Status: REFORMULAÇÃO / NÃO IMPLEMENTADO

Este arquivo define **a regra e o modelo** do Registro Reservado do Opositor.

Ele não guarda planos reais de nenhuma campanha.

Todo conteúdo vivo deve ser salvo dentro da campanha correspondente:

```text
campanhas/<nome>/opositor/
```

ou em outra subpasta equivalente definida pela estrutura daquela campanha.

```text
regras-basicas/opositor/registro-reservado.md
→ REGRA / MODELO

campanhas/<nome>/opositor/...
→ DADOS REAIS DA CAMPANHA
```

## Visibilidade

`Reservado` não significa escondido no repositório.

Todos os arquivos podem permanecer visíveis, nomeados e fáceis de localizar para inspeção, auditoria e edição manual.

A restrição é somente de **uso dentro do jogo**:

```text
ARQUIVO VISÍVEL
→ pode ser lido e editado pelo responsável pelo sistema.

CONTEÚDO RESERVADO
→ Jogador Humano, Jogador IA e Jogador IA Eventual
   não usam esse conteúdo como conhecimento de suas personagens
   enquanto ele não for descoberto legitimamente na ficção.
```

## Função

O Registro Reservado da campanha existe para que planos, prazos e processos de antagonistas continuem verdadeiros sem depender da memória da IA.

Pode preservar:

- planos de vilões;
- objetivos adversariais;
- alvos;
- preparação em andamento;
- recursos legitimamente disponíveis;
- conhecimento de cada força;
- prazos;
- gatilhos;
- estágios de execução;
- deslocamentos;
- ataques planejados;
- sequestros planejados;
- armadilhas;
- consequências futuras já estabelecidas;
- outros processos internos do lado adversarial.

## Como um plano entra no Registro da campanha

O Opositor declara a intenção do lado adversarial.

```text
OPOSITOR
→ Vilão X começa a preparar um ataque para daqui a 5 dias.
```

O Narrador julga:

```text
possui fundamento?
possui conhecimento?
possui meios?
possui tempo?
possui oportunidade?
```

Se o plano for válido, o Narrador estabelece o processo e o prazo aplicáveis.

Somente então ele passa a ser verdade da campanha e deve ser salvo em:

```text
campanhas/<nome>/opositor/...
```

```text
DECLARAÇÃO DO OPOSITOR
→ NARRADOR julga
→ processo adversarial estabelecido
→ REGISTRO DA CAMPANHA preserva
```

## Modelo de entrada

```text
VILÃO X
Plano: atacar a base dos Titãs
Estado: preparação em andamento
Prazo: ataque em 5 dias
Recursos: [somente os já estabelecidos]
Conhecimento: [somente o que o vilão realmente sabe]

VILÃO Y
Plano: sequestrar Fulano
Estado: preparação em andamento
Prazo: tentativa em 3 dias
```

Esse bloco é apenas um modelo. Os nomes, planos e prazos reais pertencem ao arquivo da campanha.

## Plano não é sucesso

Registrar um plano significa apenas que ele existe e está em andamento.

Não significa que será concluído com sucesso.

O plano pode ser:

- descoberto;
- atrasado;
- interrompido;
- alterado;
- impedido;
- abandonado;
- derrotado por outra ação legítima.

Quando isso acontecer, o Registro da campanha deve ser atualizado para refletir o estado real.

## Passagem do tempo

Um processo adversarial registrado pode continuar fora da cena principal sem precisar ser redeclarado em todas as janelas.

O Opositor volta a agir quando:

- chega uma etapa do plano;
- o prazo vence;
- surge nova decisão adversarial;
- a situação muda;
- aparece nova oportunidade;
- uma força adversarial entra em campo.

## Fiscalização

O Opositor usa o Registro da campanha para impedir que planos e prazos internos sejam esquecidos.

```text
REGISTRO DA CAMPANHA
→ ataque começa hoje.

OPOSITOR
→ traz o prazo para a janela.

NARRADOR
→ verifica o Registro.
→ reconhece a entrada do evento.
```

A fiscalização não cria nem antecipa o fato.

## Conhecimento compartimentado

O Opositor pode conhecer todo o material adversarial necessário para administrar o outro lado da trama.

Esse conhecimento não pertence automaticamente a cada vilão ou NPC.

```text
OPOSITOR SABE
≠
VILÃO SABE
```

Cada peça adversarial só pode agir com o conhecimento que ela própria possui legitimamente.

## Restrição operacional

O conteúdo real pode estar totalmente visível dentro de `campanhas/<nome>/`.

A regra não tenta impedir que o responsável pela campanha o leia.

Ela apenas impede que uma persona use esse conteúdo como conhecimento ficcional sem fundamento.

```text
RESPONSÁVEL PELO SISTEMA LEU O ARQUIVO
≠
PERSONAGEM DESCOBRIU A INFORMAÇÃO
```

Se uma informação adversarial for descoberta legitimamente, o Narrador registra o fato correspondente no local apropriado da própria campanha para a personagem que a descobriu.

## Regra final

> **Este arquivo contém apenas a regra e o modelo. Todo plano, processo, prazo ou conhecimento adversarial real deve ser salvo em `campanhas/<nome>/`. “Reservado” é uma restrição operacional de conhecimento, não ocultação física do arquivo.**