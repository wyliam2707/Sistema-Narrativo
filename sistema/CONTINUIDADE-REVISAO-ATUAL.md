# Continuidade Atual — Revisão do Sistema

Status: CHECKPOINT PARA NOVO CHAT
Data do checkpoint: 2026-08-21

Este arquivo existe para permitir que a revisão do sistema continue em outro chat sem depender da memória da conversa anterior.

---

## 1. Estado da campanha usada como teste

A campanha **Castelo dos Corvos** está PAUSADA de propósito enquanto o sistema é revisado.

- O Capítulo 14 foi salvo como **Capítulo 14 — Seguir em Frente**.
- Não avançar a ficção automaticamente.
- A campanha está sendo usada apenas como exemplo prático para testar regras do sistema.

Ponto salvo da campanha:
- Corvin dormiu no solar depois de guardar novamente no depósito uma fotografia antiga de Marta e de pessoas da Casa.
- Ravena dormiu no próprio quarto e não presenciou essa despedida.
- O romance, a Casa Blackwood, Marta e demais elementos da campanha continuam canônicos conforme os arquivos da aventura.

---

## 2. Problema identificado durante a campanha

A campanha mostrou que a IA estava misturando funções diferentes:

- às vezes Ravena/Jogadores IA viravam extensões do Narrador;
- às vezes o Narrador protegia demais os planos do protagonista;
- às vezes o Narrador criava resistência artificial apenas para evitar sucesso fácil;
- antagonistas podiam desaparecer porque não existia uma função explicitamente obrigada a pensar oposição;
- intenções do jogador eram ocasionalmente tratadas como resultados garantidos.

A revisão passou a separar essas responsabilidades.

---

## 3. Cinco papéis operacionais e quatro personas da IA

Existem cinco papéis no ciclo:

1. `JOGADOR HUMANO`
2. `JOGADOR IA`
3. `JOGADOR IA EVENTUAL`
4. `OPOSITOR`
5. `NARRADOR`

O `JOGADOR HUMANO` pertence ao usuário.

As quatro personas executadas pela IA são:

- `JOGADOR IA`
- `JOGADOR IA EVENTUAL`
- `OPOSITOR`
- `NARRADOR`

Estrutura criada:

```text
sistema/personas/
├── README.md
├── jogador-humano/
│   └── README.md
├── jogador-ia/
│   └── README.md
├── jogador-ia-eventual/
│   └── README.md
├── opositor/
│   └── README.md
└── narrador/
    └── README.md
```

---

## 4. Ciclo operacional atual

A regra de prioridade máxima foi alterada para:

```text
JOGADOR HUMANO declara
↓
JOGADOR IA declara
↓
JOGADOR IA EVENTUAL é obrigatoriamente avaliado; se ativo, declara
↓
OPOSITOR declara pressão/oposição ou ausência de pressão relevante
↓
NARRADOR resolve
↓
NOVA SITUAÇÃO
```

Regra importante:

> Nenhum slot deve desaparecer por esquecimento.

`Nada a declarar`, `nenhuma ativação relevante` e `nenhuma pressão relevante` são declarações válidas.

---

## 5. Intenção não é resultado

Princípio consolidado durante Castelo dos Corvos:

> **Intenção continua sendo intenção.**

Isso NÃO significa transformar tudo em aleatoriedade.

Uma boa ideia continua sendo boa.
Uma retórica convincente continua enganando quando faz sentido.
Atributos altos, perícias altas, poderes altos, preparação, contexto favorável, reputação, posição e informação continuam sendo decisivos.

Exemplo conceitual:

- boa ideia + capacidade alta + contexto favorável → normalmente funciona;
- boa ideia + oposição forte → disputa real;
- ideia ruim + capacidade alta → pode reduzir o dano, não obrigatoriamente transformar a ideia em boa;
- impossibilidade real → capacidade alta não inventa uma solução inexistente.

O Narrador não deve criar falha aleatória só para preservar incerteza.

---

## 6. Persona OPOSITOR

O `OPOSITOR` reúne duas funções que inicialmente foram consideradas separadas:

1. pressão impessoal do mundo;
2. oposição intencional de agentes, rivais, vilões, facções etc.

Assim, o Opositor pode explorar:

- preço;
- disponibilidade;
- escassez;
- logística;
- burocracia;
- clima;
- distância;
- legislação;
- reputação;
- contratos;
- concorrência;
- espionagem;
- chantagem;
- sabotagem;
- emboscadas;
- política;
- relações;
- informação;
- tempo;
- recursos.

Princípio:

> **O Opositor procura o ponto legítimo de pressão disponível.**

Ele pode usar qualquer gancho causal para iniciar ou ampliar conflito, mas não pode inventar retroativamente uma oposição só porque percebeu que o plano do jogador teria sucesso.

Para oposição intencional, verificar:

1. O agente sabe o suficiente?
2. Possui motivo para agir?
3. Possui meios/recursos/oportunidade?

Se não houver pressão legítima:

`OPOSITOR — nenhuma pressão relevante.`

O Opositor pode plantar problemas antes do payoff, desde que seus agentes tenham conhecimento, motivo e meios reais para preparar isso.

---

## 7. Persona NARRADOR

O Narrador deve ser neutro.

Ele não existe para:

- proteger o plano do protagonista;
- contrariar o protagonista;
- recuperar dificuldade perdida;
- garantir drama;
- criar ameaça depois de ver que o plano funcionaria.

O Narrador recebe:

- intenções dos jogadores;
- participação do Opositor;
- capacidades;
- posição;
- preparação;
- informação;
- ambiente;
- STATUS;
- efeitos existentes;

E resolve causalmente o resultado.

Princípio:

> **Jogadores querem. O Opositor pressiona. O Narrador arbitra.**

---

## 8. Compartimentação de conhecimento

A mesma IA pode executar várias personas, mas não pode misturar conhecimento entre elas.

```text
Conhecimento do Narrador
≠ conhecimento do Jogador IA
≠ conhecimento do Jogador IA Eventual
≠ conhecimento dos agentes usados pelo Opositor
```

O Opositor não ganha automaticamente acesso a segredos de `mestre/`.

Declarações secretas podem existir operacionalmente sem serem mostradas ao jogador humano. O Narrador só apresenta o que se torna perceptível ou legitimamente descoberto.

---

## 9. Nova arquitetura estrutural

Foi decidido reorganizar o sistema em subpastas para facilitar consulta.

Pastas criadas:

```text
sistema/
├── personas/
├── resolucao/
├── agencia/
├── narracao/
├── persistencia/
└── operacao/
```

Responsabilidades:

- `personas/` → quem decide o quê;
- `resolucao/` → como declarações viram resultados;
- `agencia/` → autonomia, vida fora da câmera, conhecimento separado;
- `narracao/` → como a ficção é apresentada;
- `persistencia/` → estado, cronologia, progressão, fichas, livro e salvamento;
- `operacao/` → checklist, ordem de consulta e execução do sistema.

---

## 10. Migração sem apagar os arquivos antigos

Decisão explícita do usuário:

> **Criar novos arquivos e manter os originais até que eles não sejam mais úteis.**

Foi criado:

`sistema/MIGRACAO-ESTRUTURAL.md`

Regra da migração:

- não mover/apagar um arquivo antigo apenas porque existe uma pasta nova;
- arquivos antigos continuam válidos até uma substituição nova estar escrita, revisada, aprovada e com referências importantes atualizadas;
- estados de migração: `NOVA ESTRUTURA`, `ANTIGA AINDA VÁLIDA`, `EM REVISÃO`, `SUBSTITUÍDA`, `OBSOLETA`.

Arquivos antigos principais ainda marcados como válidos incluem:

- `sistema/README.md`
- `sistema/00-LEIA-PRIMEIRO.md`
- `sistema/ciclo-de-jogadores.md`
- `sistema/agencia-de-personagens.md`
- `sistema/narracao-e-escrita-padrao.md`
- `sistema/modo-rpg.md`
- `sistema/checklist-do-narrador.md`
- `sistema/protocolo-de-fechamento-de-capitulo.md`

---

## 11. Próximo ponto de trabalho — NÃO RESOLVIDO AINDA

A última pergunta antes deste checkpoint foi:

> **“Quanto aos valores numéricos e criação de personagem, onde eles devem ser mantidos?”**

Isso ainda NÃO foi decidido.

Ao abrir o próximo chat, retomar exatamente daqui.

Questões a analisar:

- criação de personagem deve ter uma nova área própria, por exemplo `sistema/personagem/` ou `sistema/ficha/`?
- escala numérica 0–5, atributos, perícias, poderes, sintaxe e regras de ficha pertencem a `resolucao/` ou merecem uma área estrutural própria?
- separar “definição da ficha” de “uso da ficha na resolução” provavelmente evita misturar criação com arbitragem;
- decidir onde ficam modelos/templates de ficha;
- decidir onde ficam regras de NPCs, Jogadores IA e antagonistas na criação de personagens;
- manter o atual `sistema/README.md` como fonte antiga válida enquanto a nova divisão é construída.

Nenhuma estrutura nova para esse ponto deve ser presumida até a discussão continuar.

---

## 12. Ordem sugerida ao retomar

1. Resolver onde ficam **criação de personagem, ficha e valores numéricos**.
2. Ajustar a arquitetura nova se necessário.
3. Refinar `personas/opositor/` em detalhe.
4. Refinar `personas/narrador/`.
5. Depois reconstruir `resolucao/` usando essas personas já estabilizadas.
6. Manter Castelo dos Corvos pausado até o usuário pedir explicitamente para voltar à campanha.

---

## Regra de retomada

Ao iniciar um novo chat para esta revisão:

1. consultar este arquivo;
2. consultar `sistema/MIGRACAO-ESTRUTURAL.md`;
3. consultar `sistema/personas/README.md` e `sistema/ciclo-de-jogadores.md` se a discussão envolver personas/ciclo;
4. não apagar arquivos antigos sem aprovação;
5. retomar pela questão pendente de criação de personagem e valores numéricos.
