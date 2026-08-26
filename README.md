# Sistema Narrativo

Este repositório separa **o sistema do RPG** dos **dados concretos de cada campanha**.

## Estrutura atual

- `sistema/` — única fonte canônica das regras atuais, criação, personagens, personas, agência, operação, resolução, narração e persistência.
- `campanhas/` — campanhas criadas pelo fluxo atual ou arquivos explicitamente marcados como teste/incompatíveis.
- `aventuras/` — arquivo legado de campanhas antigas; não faz parte do fluxo normal e não é fonte de regras.

## Regra fundamental

> **O sistema ensina como criar e operar. A campanha guarda o que foi criado e o que aconteceu.**

Nada específico de uma campanha deve ser gravado como regra universal em `sistema/`.

---

# Execução autossuficiente por IA

Este repositório deve ser suficiente para uma IA executar o RPG **sem depender de memória de conversas anteriores, prompt privado, configuração externa ou conhecimento não registrado**.

Ao receber somente o repositório e uma instrução como `inicie`, `vamos jogar`, `abra este sistema` ou equivalente:

```text
1. ler este README
→ 2. ler sistema/00-LEIA-PRIMEIRO.md
→ 3. perguntar: Nova campanha ou continuar uma campanha existente?
→ 4. seguir somente as fontes canônicas indicadas pelos arquivos
```

Não exigir código especial de inicialização.

Não pedir ao jogador que reconte informação que já exista em fonte canônica da campanha.

Se a plataforma possuir apenas **uma única IA**, isso não impede o jogo. As personas podem ser executadas sequencialmente pela mesma IA, desde que permaneçam separadas por autoridade e escopo conforme:

```text
sistema/personas/instanciacao-da-mesa.md
sistema/personas/escopo-de-consulta.md
```

Instanciar uma persona não exige criar um processo, bot ou agente externo. Significa manter uma cadeira operacional separada e obedecer ao contexto permitido para ela.

> **Nenhuma capacidade externa além da leitura e aplicação destes arquivos é requisito do sistema.**

---

# Como iniciar

Depois de ler `sistema/00-LEIA-PRIMEIRO.md`, perguntar ao jogador apenas:

> **Nova campanha ou continuar uma campanha existente?**

## NOVA CAMPANHA

Abrir:

```text
sistema/criacao/README.md
```

Esse é o processo canônico atual para criação de novas campanhas.

A nova campanha é criada em:

```text
campanhas/<nome-da-campanha>/
```

A criação registra seu próprio checkpoint no `README.md` da campanha e segue as regras definidas em `sistema/criacao/`.

A primeira cena é proibida antes da aprovação de:

```text
sistema/criacao/start-da-campanha.md
```

> **NOVA CAMPANHA → `sistema/criacao/README.md`**

## CONTINUAR CAMPANHA

Consultar primeiro:

```text
campanhas/README.md
```

Oferecer para continuação somente campanhas que não estejam explicitamente marcadas como **teste, legado ou incompatíveis com o motor atual**.

Depois que o jogador escolher uma campanha válida, abrir:

```text
campanhas/<nome>/README.md
```

O `README.md` da própria campanha define:

- se a criação está em andamento ou concluída;
- onde retomar;
- quais personagens têm agência;
- a Mesa operacional, quando a campanha já recebeu START;
- onde consultar o estado atual.

### Criação ainda em andamento

```text
CRIAÇÃO: EM ANDAMENTO
→ retomar pelo checkpoint
→ sistema/criacao/README.md
→ não abrir cena antes do CHECK DE START
```

### Campanha já iniciada

```text
CRIAÇÃO: CONCLUÍDA
→ reinstanciar Mesa operacional
→ conferir escopos das personas
→ ler estado/atual.md
→ consultar somente fichas e fontes necessárias
→ retomar a cena
```

Não recriar personagens, fatos ou relações que já estejam registrados.

> **CONTINUAR → `campanhas/<nome>/README.md`**

## Campanha marcada como incompatível

Se uma pasta dentro de `campanhas/` estiver explicitamente marcada como teste antigo ou incompatível:

```text
não usar como exemplo do motor atual
→ não continuar automaticamente
→ não converter silenciosamente
→ migrar somente mediante pedido explícito do jogador
```

---

## Arquivo legado

`aventuras/` guarda campanhas produzidas por versões anteriores da arquitetura.

Por padrão:

- não listar seu conteúdo como campanha atual;
- não usar suas fichas, estrutura ou mecânicas como exemplo das regras atuais;
- não migrar, mover, reestruturar ou continuar automaticamente;
- consultar somente quando o jogador pedir explicitamente para recuperar, examinar ou migrar material legado.

As regras atuais pertencem exclusivamente a `sistema/`.

---

## Comandos administrativos

Operações de manutenção ficam separadas do fluxo normal de jogo.

Para exclusão de campanha e demais procedimentos administrativos, consultar:

```text
sistema/operacao/comandos-administrativos.md
```

Nenhuma exclusão pode atingir `sistema/`, a raiz do repositório ou outra campanha por consequência indireta.

---

## Prioridade das fontes

Durante execução normal:

```text
regra universal atual
→ sistema/

fato concreto da campanha
→ campanhas/<nome>/

memória da IA ou conversa anterior
→ nunca prevalece sobre fonte canônica registrada
```

Se um arquivo de campanha contradizer claramente o motor atual por estar marcado como legado/incompatível, ele não deve ser usado numa campanha nova nem continuado silenciosamente.

## Continuidade

Para iniciar ou continuar uma campanha atual, as fontes persistentes da própria campanha prevalecem sobre memória vaga de conversas anteriores.

> **O link abre o sistema. O sistema pergunta Nova ou Continuar. Os arquivos dizem o resto.**
