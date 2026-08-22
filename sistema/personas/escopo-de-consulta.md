# Escopo de Consulta das Personas

Status: APROVADO

Este documento define **quais informações cada persona deve receber para exercer sua função durante o jogo**.

A regra existe para impedir contaminação de contexto entre personas executadas pela mesma IA.

> **Uma persona não consulta toda a campanha apenas porque tecnicamente poderia fazê-lo. Ela recebe somente o contexto necessário para sua função naquele momento.**

## Acesso técnico não é acesso operacional

Todos os arquivos podem estar no mesmo repositório e o JOGADOR HUMANO pode tecnicamente abri-los quando quiser.

Isso não significa que todas as personas da IA recebem ou podem usar todos esses arquivos durante sua atuação.

> **Separação de persona é separação de contexto e autoridade, não mecanismo técnico de segurança.**

A existência de uma informação no GitHub não a torna automaticamente disponível a uma persona ou personagem.

## Princípio do menor contexto suficiente

Antes de executar uma persona, fornecer apenas o conjunto de informações necessário para responder à pergunta própria daquela função.

```text
JOGADOR IA
→ O que meu personagem quer fazer com aquilo que sabe?

JOGADOR IA EVENTUAL
→ Este personagem eventual está ativo e, se estiver, o que quer fazer?

OPOSITOR
→ Que fio do cenário pode se mover agora ou ser preparado para depois?

NARRADOR
→ Dadas as declarações e os fatos relevantes, o que realmente acontece?
```

Informação sem relação com essa pergunta não precisa entrar no contexto da persona.

# JOGADOR IA

O JOGADOR IA recebe a visão do personagem que controla.

## Pode receber

- ficha do personagem;
- STATUS do personagem;
- personalidade, objetivos, desejos, medos e limites;
- relações relevantes vistas daquele personagem;
- `Conhecimento atual relevante` da ficha;
- acontecimentos que o personagem presenciou ou aprendeu legitimamente;
- situação atual conforme percebida por ele;
- regras necessárias para declarar sua ação;
- informações de mundo que sua história, formação ou experiência justificam.

## Não recebe automaticamente

- `mestre/` completo;
- ficha secreta de NPC;
- planos futuros do OPOSITOR;
- pensamentos privados de outros personagens;
- fatos ocorridos fora de sua percepção e nunca comunicados;
- preparação secreta que ainda não descobriu;
- resultado futuro da resolução;
- Livro multiperspectivo completo.

O Livro pode ser usado como fonte de recuperação apenas por meio dos trechos que correspondam a acontecimentos legitimamente conhecidos pelo personagem.

> **O JOGADOR IA não finge ignorar informação que recebeu por engano; o ideal é que essa informação nunca entre em seu contexto operacional.**

# JOGADOR IA EVENTUAL

Quando ativo, segue o mesmo princípio do JOGADOR IA.

Recebe somente:

- ficha do personagem eventual;
- STATUS e situação relevantes;
- conhecimento legítimo desse personagem;
- relações e objetivos próprios;
- regras necessárias;
- informação percebida na cena ou recebida legitimamente fora dela.

Vários personagens eventuais não formam mente coletiva. O contexto de cada um deve permanecer separado quando seus conhecimentos forem diferentes.

Quando não houver personagem eventual ativo, a persona não precisa receber fichas ou segredos apenas para confirmar sua inatividade.

# OPOSITOR

O OPOSITOR recebe **material operacional para mover o cenário**, não a campanha inteira.

## Pode receber

Conforme a situação:

- Progressão relevante;
- ganchos ainda vivos;
- planos de NPCs que possam avançar;
- preparações já validadas;
- NPCs disponíveis para movimentação;
- consequências antigas que ainda podem reagir;
- fatos do cenário necessários para avaliar movimento;
- passagem de tempo relevante;
- situação atual;
- oportunidades já abertas;
- sementes futuras autorizadas que estejam aguardando momento ou condição.

Esse material pode vir de `mestre/`, Progressão, mundo, STATUS ou outros registros da campanha, mas somente na extensão necessária para a função do OPOSITOR.

## Não recebe automaticamente

- toda a pasta `mestre/`;
- toda a biografia de cada NPC;
- pensamentos privados de personagens jogáveis sem relação com o movimento do cenário;
- informações que não podem afetar nenhum gancho disponível;
- Livro completo apenas para procurar alguma coisa aleatoriamente;
- poderes ou recursos não estabelecidos para construir uma resposta sob medida.

O OPOSITOR pode pedir ao NARRADOR contexto adicional quando perceber que um gancho depende de informação que não recebeu.

Exemplo:

```text
OPOSITOR
→ O contato de Trigon feito há três semanas pode avançar agora?
```

O NARRADOR consulta o que falta e informa somente o necessário para validar ou negar o movimento.

# NARRADOR / MESTRE / JUIZ

O NARRADOR recebe **contexto de resolução**, não contexto total por padrão.

## Recebe sempre que relevante

- declarações da janela atual;
- situação atual;
- fichas dos envolvidos;
- regras aplicáveis;
- fatos do cenário necessários;
- posição, tempo, recursos e condições presentes;
- fatos ou preparações que possam legitimamente afetar aquela resolução.

## Consulta sob demanda

Se uma declaração exigir verificar algo ainda não carregado, o NARRADOR consulta especificamente a fonte necessária.

Exemplo:

```text
OPOSITOR
→ Trigon pode mandar um assassino?

NARRADOR consulta apenas o necessário:
- Trigon possui meios?
- possui motivo?
- sabe onde encontrá-los?
- quanto tempo isso leva?
```

Ele não precisa carregar toda a história de Trigon, todos os segredos da campanha ou todos os capítulos do Livro para responder a essa pergunta.

## O que o NARRADOR não faz com contexto extra

Mesmo quando consulta informação reservada para julgar, o NARRADOR não a transfere automaticamente para:

- JOGADOR IA;
- JOGADOR IA EVENTUAL;
- personagem do JOGADOR HUMANO;
- OPOSITOR além do necessário para seu próximo movimento.

Conhecer para julgar não significa distribuir conhecimento.

# JOGADOR HUMANO

O JOGADOR HUMANO não é limitado tecnicamente por este protocolo.

Ele pode abrir o repositório, inclusive material reservado, se decidir fazê-lo.

Durante a interpretação de seu personagem, porém, continua valendo a distinção normal entre:

```text
O HUMANO SABE
≠
O PERSONAGEM SABE
```

O sistema não tenta impor sigilo técnico ao usuário.

# Arquivos e fontes

A regra não exige que cada persona possua uma pasta física exclusiva.

O mesmo arquivo pode ser fonte para mais de uma persona, desde que cada uma receba somente o trecho ou conteúdo pertinente à própria função.

Exemplo:

```text
mestre/npcs/Trigon.md
```

Pode conter muitas informações.

O OPOSITOR pode receber:

```text
- Trigon está esperando resposta há três semanas.
- possui agentes disponíveis.
```

O NARRADOR pode receber, para julgar uma proposta:

```text
- Trigon sabe onde fica a mansão.
- contratar e deslocar um agente leva três dias.
```

O JOGADOR IA de Ravena não recebe nenhum desses fatos enquanto Ravena não tiver forma legítima de conhecê-los.

## Livro multiperspectivo

Como o Livro pode registrar ações secretas, pensamentos e acontecimentos fora da percepção de um personagem, ele **não deve ser carregado integralmente como memória automática de uma persona de jogador**.

Quando for necessário recuperar histórico para um personagem, selecionar somente fatos e passagens compatíveis com aquilo que ele sabe.

O NARRADOR e o OPOSITOR também não precisam consultar o Livro inteiro por padrão; devem buscar nele apenas quando um fato histórico específico for necessário para sua função.

## Informação pedida sob demanda

Uma persona pode identificar que precisa de informação adicional sem ganhar acesso irrestrito às fontes.

Fluxo:

```text
1. A persona identifica a lacuna.
2. Solicita o dado necessário à função.
3. O sistema/NARRADOR consulta a fonte apropriada.
4. Entrega somente o contexto necessário.
5. A persona continua sua atuação.
```

## Regra final

> **Cada persona recebe o menor contexto suficiente para exercer sua função corretamente.**
>
> **JOGADORES recebem a visão de suas peças. OPOSITOR recebe os fios que pode mover. NARRADOR recebe o que precisa para julgar.**
