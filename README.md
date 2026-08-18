# Sistema Narrativo

Este repositório separa **o motor do RPG** dos **dados de cada aventura**.

## Estrutura

- `sistema/` — regras universais, linguagem de fichas, agência de personagens, criação e operação de aventuras.
- `aventuras/` — cada aventura concreta, com personagens, mundo, relações, Progressão, estado atual, cronologia, diretrizes e história canônica.

## Regra fundamental

> **O sistema ensina como criar e operar. A aventura registra o que foi criado e o que aconteceu.**

Nada específico de uma campanha deve ser gravado como regra universal em `sistema/`.

---

# Como iniciar

Se este repositório foi fornecido a um narrador humano ou IA com uma instrução como `inicie`, `vamos jogar`, `abra este sistema` ou equivalente:

1. ler `sistema/00-LEIA-PRIMEIRO.md`;
2. perguntar ao jogador apenas:

> **Nova campanha ou continuar uma campanha existente?**

Não exigir código especial de inicialização. O próprio endereço deste repositório pode servir como porta de entrada.

---

## Se o jogador escolher NOVA CAMPANHA

Abrir:

` sistema/protocolo-de-criacao.md `

O protocolo começa perguntando o nome da campanha, cria sua estrutura em `aventuras/<nome>/` e conduz quatro etapas conceituais:

1. Cenário;
2. Protagonista;
3. Personagens relevantes;
4. Início da história.

Cada etapa é organizada e salva como **PENDENTE DE REVISÃO** antes da próxima.

Somente depois das quatro etapas começa a revisão que aplica atributos, perícias, poderes e demais regras mecânicas.

> **Conceito primeiro. Mecânica depois.**

---

## Se o jogador escolher CONTINUAR

Consultar `aventuras/` e listar as campanhas realmente existentes.

Depois que o jogador escolher uma campanha:

1. ler o `README.md` daquela aventura;
2. verificar `criacao.md`, se existir;
3. se a criação ainda estiver em andamento, retomar do ponto registrado;
4. se a criação estiver concluída, carregar as fontes indicadas pela aventura;
5. ler `estado/atual.md` para descobrir o ponto exato de continuação;
6. continuar sem pedir ao jogador que reconte onde parou quando os arquivos já contêm essa informação.

Nunca inventar campanhas que não estejam em `aventuras/`.

---

## Comandos administrativos

Operações de manutenção que podem destruir dados ficam separadas do fluxo normal de jogo.

Para apagar definitivamente uma campanha, consultar:

` sistema/comandos-administrativos.md `

O comando definido é:

```text
APAGAR CAMPANHA: <nome exato da campanha>
```

A exclusão nunca é imediata: o sistema deve localizar a campanha e exigir depois a confirmação exata:

```text
CONFIRMAR EXCLUSÃO: <nome exato da campanha>
```

Nenhuma operação de exclusão pode atingir `sistema/`, a raiz do repositório ou outra campanha.

---

## Continuidade

Para iniciar ou continuar qualquer aventura, as fontes persistentes da campanha prevalecem sobre memória vaga de conversas anteriores.

> **O link abre o sistema. O sistema pergunta Nova ou Continuar. Os arquivos dizem o resto.**