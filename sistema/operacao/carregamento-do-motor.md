# Carregamento e Recarregamento do Motor

Status: APROVADO

Este arquivo define **como uma IA forma e renova sua compreensão operacional do sistema usando somente os arquivos do repositório**.

Ele não cria regras mecânicas novas. Sua função é impedir que uma sessão longa passe a depender de lembranças incompletas, resumos antigos ou contexto de conversa que já não represente o motor atual.

> **Arquivo canônico é memória permanente. Modelo mental é cache operacional.**

## 1. Princípio central

A IA deve manter uma compreensão global do motor para jogar com fluidez, mas essa compreensão nunca substitui os arquivos.

```text
ARQUIVOS ATUAIS EM sistema/
→ fonte canônica

MODELO MENTAL DA IA
→ representação operacional temporária
→ acelera consulta
→ pode envelhecer
→ nunca prevalece sobre o arquivo atual
```

Se houver diferença entre lembrança, resumo interno e fonte atual:

> **a fonte canônica atual prevalece.**

## 2. Primeiro carregamento é obrigatório

Quando uma IA recebe o repositório para iniciar o RPG sem contexto anterior, ela não deve perguntar imediatamente qual campanha jogar.

Antes da primeira pergunta ao JOGADOR HUMANO:

```text
1. ler README.md da raiz
→ 2. ler sistema/00-LEIA-PRIMEIRO.md
→ 3. ler integralmente e de forma recursiva todos os arquivos atuais dentro de sistema/
→ 4. reconstruir o modelo mental do motor
→ 5. somente então perguntar:
   Nova campanha ou continuar uma campanha existente?
```

A leitura integral inicial inclui as oito áreas:

```text
criacao/
personagem/
personas/
agencia/
operacao/
resolucao/
narracao/
persistencia/
```

Não é necessário carregar `aventuras/` ou campanhas concretas para aprender as regras universais.

> **Primeiro aprende o motor. Depois pergunta qual mesa será aberta.**

## 3. O que significa reconstruir o modelo mental

Depois da leitura integral, a IA deve ser capaz de localizar e distinguir, sem misturar responsabilidades:

- quem possui autoridade sobre cada decisão;
- como personagens e personas se relacionam;
- como funciona o fluxo fora de combate;
- como funciona o fluxo de combate;
- quando existe resolução mecânica;
- onde estão as regras de Atributos, Perícias, Poderes, Trama, Vida, Mana, Status e demais capacidades;
- como Hubs são apresentados ao JOGADOR HUMANO;
- como o NARRADOR julga e apresenta a sentença;
- onde cada verdade persistente deve ser salva;
- como reconstruir a Mesa operacional de uma campanha.

Reconstruir não significa escrever uma segunda versão das regras nem criar um resumo concorrente dentro do repositório.

O modelo mental existe apenas para **navegar melhor pelas fontes atuais**.

## 4. Durante o capítulo

Depois do carregamento integral, não é necessário reler `sistema/` inteiro a cada ação.

Durante o jogo:

```text
modelo mental
→ orienta qual regra procurar

situação simples e regra segura
→ aplicar normalmente

detalhe capaz de alterar resultado, custo, duração, autoridade ou consequência
+ qualquer dúvida real
→ consultar novamente o arquivo canônico responsável
```

Nunca reconstruir uma regra pela lembrança quando a fonte responsável puder ser consultada.

> **Memória agiliza. Arquivo confirma.**

## 5. Recarregamento obrigatório após fechar capítulo

Sempre que `../persistencia/fechamento-de-capitulo.md` concluir o salvamento de um capítulo, executar um **recarregamento completo do motor antes de qualquer nova ficção**.

A ordem é:

```text
CAPÍTULO SALVO
→ persistência daquele fechamento concluída
→ ficção continua parada

RECARREGAR MOTOR
→ reler README.md da raiz
→ reler sistema/00-LEIA-PRIMEIRO.md
→ reler integralmente todos os arquivos atuais de sistema/
→ reconstruir o modelo mental do zero a partir das fontes atuais
→ abandonar interpretações internas que tenham sido substituídas

RECARREGAR MESA
→ ler README da campanha
→ reconstruir Mesa operacional
→ conferir escopos das personas
→ ler estado/atual.md já atualizado
→ carregar fichas e fontes da campanha necessárias para a continuação

PRONTO
→ somente agora o próximo capítulo pode começar
```

Esse procedimento é obrigatório mesmo que a IA acredite lembrar perfeitamente das regras.

## 6. Mudanças de regra durante um capítulo

Se qualquer arquivo de `sistema/` for alterado durante uma sessão, a recarga pós-capítulo usa sempre a versão atual existente no repositório.

Portanto:

```text
regra antiga lembrada
+ arquivo atual diferente
→ descartar a interpretação antiga
→ reconstruir usando o arquivo atual
```

O fechamento do capítulo funciona também como um **ponto de sincronização do motor**.

## 7. Recarregar campanha não significa reler toda a história

Depois de recarregar `sistema/`, a campanha deve ser reconstruída pelo presente operacional.

Carregar por padrão:

```text
README da campanha
→ checkpoint ou Mesa operacional

estado/atual.md
→ presente da campanha

personagens/
→ fichas necessárias às peças atuais e às personas instanciadas

mundo/ e mestre/
→ somente fontes necessárias conforme situação e escopo de consulta
```

Não reler automaticamente todos os capítulos de `livro/`.

Consultar o Livro apenas quando um fato histórico necessário não estiver suficientemente consolidado nas fontes atuais ou quando uma regra de persistência exigir essa recuperação.

Isso evita transformar histórico completo em contexto permanente sem necessidade.

## 8. Escopo das personas continua valendo

O recarregamento técnico pode ser executado por uma única IA, mas não autoriza contaminação entre cadeiras.

Depois de reconstruir o motor, aplicar novamente:

```text
../personas/instanciacao-da-mesa.md
../personas/escopo-de-consulta.md
```

A IA técnica pode ter lido o sistema inteiro.

Isso não significa que:

- JOGADOR IA recebe segredos de outra personagem;
- JOGADOR IA EVENTUAL forma mente coletiva;
- OPOSITOR transforma informação operacional em conhecimento de NPC;
- NARRADOR entrega material reservado às peças.

> **Recarregar o motor amplia compreensão das regras; não amplia conhecimento ficcional das personagens.**

## 9. Recarregamento não joga

Durante o recarregamento:

- não avançar tempo ficcional;
- não declarar ação;
- não resolver conflito novo;
- não mover gancho;
- não produzir reação de NPC;
- não alterar estado por interpretação;
- não criar capítulo novo.

Ele é uma rotina operacional entre capítulos.

## 10. Recarga extraordinária

Além da recarga obrigatória ao fechar capítulo, a IA pode repetir este procedimento quando:

- a sessão ficar muito longa;
- houver dúvida ampla sobre a arquitetura;
- várias regras tiverem sido modificadas;
- a execução demonstrar sinais de mistura entre versões ou responsabilidades.

Essa recarga extraordinária não exige fechar capítulo, mas também não cria ficção.

## 11. Fluxo cíclico

```text
CARREGAR SISTEMA
→ formar modelo mental
→ carregar campanha
→ jogar capítulo
→ consultar fontes específicas quando necessário
→ fechar e salvar capítulo
→ RECARREGAR SISTEMA INTEGRALMENTE
→ reconstruir modelo mental
→ recarregar presente da campanha
→ próximo capítulo
```

## Regra final

> **Toda IA aprende integralmente `sistema/` antes da primeira pergunta de jogo e reconstrói esse modelo mental depois de cada capítulo salvo. Entre essas recargas, a memória acelera a execução, mas qualquer fonte canônica atual sempre prevalece sobre a lembrança.**
