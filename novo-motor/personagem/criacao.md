# Criação e Revisão de Personagens

Status: EM DESENVOLVIMENTO

Este arquivo descreve o fluxo atual de criação e revisão de personagens dentro do `novo-motor/`.

A regra principal continua sendo:

> **Proposta não é fato. Só salvar depois da aprovação explícita do jogador.**

## Ordem atual de construção

A ficha é construída por blocos, seguindo a ordem visual definida em `ficha.md`:

```text
1. Descrição
2. Atributos
3. Perícias
4. Referências
5. Ataques
6. Poderes
7. Recursos
8. Personalidade
9. Histórico e conhecimento
```

O jogador pode corrigir qualquer bloco antes de aprová-lo. Uma correção pontual altera apenas o que foi pedido, salvo quando a mudança exigir consequência direta em outro campo.

## 1. Descrição

Registrar:

```text
Nome: Codinome — Nome real
Importância:
Controle:
Idade:
Peso:
Altura:
Descrição visual:
```

`Descrição visual` registra apenas aquilo que pode ser percebido olhando o personagem.

Não incluir aqui personalidade, intenção, medo, desejo ou explicação psicológica.

## 2. Atributos

Usar os seis Atributos atuais:

```text
Corpo - Força [ ] | Destreza [ ] | Agilidade [ ]
Mente - Intelecto [ ] | Percepção [ ] | Presença [ ]
```

A escala definitiva e o procedimento de calibração permanecem sujeitos ao desenvolvimento do novo motor.

## 3. Perícias

Usar a lista fixa atual de 8 Perícias comuns e 8 somente treinadas.

```text
Comuns
Esportes [ ] | Exploração [ ] | Expressão [ ] | Sociedade [ ]
Investigação [ ] | Crime [ ] | Ofícios [ ] | Idiomas [ ]

Somente treinadas
Arcano [ ] | Ocultismo [ ] | Natureza [ ] | Medicina [ ]
Engenharia [ ] | Ciência [ ] | Tecnologia [ ] | História [ ]
```

Perícias cobrem exploração, conhecimento e interação com o mundo. Combate não pertence a esse bloco.

## 4. Referências

Consolidar os valores estáveis de consulta rápida:

```text
Vida [ ] | Energia [ ] | Deslocamento: ... | Visão: ...
Defesas - Esquiva [ ] | Vontade [ ] | Fortitude [ ] | RD: ...
```

Não registrar aqui Vida atual, Energia atual, condições ou outros estados temporários.

As fórmulas definitivas de Defesas ainda serão fechadas em `../resolucao/`.

## 5. Ataques

Registrar uma linha para cada forma básica de ataque:

```text
Luta [ ] / arma / dano / crítico / alcance
Disparo [ ] / arma / dano / crítico / alcance
Magia [ ] / arma ou efeito / dano / crítico / alcance
```

Essas linhas devem servir como consulta pronta durante conflito.

## 6. Poderes

Na ficha principal, registrar apenas os nomes dos Poderes disponíveis.

```text
## Poderes
- Teleporte
- Escudo Arcano
- Petrificação
```

Os detalhes completos serão mantidos em arquivos próprios e consultados somente quando o Poder for escolhido para uso.

O formato definitivo desses arquivos ainda será definido.

## 7. Recursos

Registrar apenas meios, infraestrutura, acesso ou bens realmente relevantes para possibilidades futuras.

Não transformar o bloco em inventário de objetos comuns.

## 8. Personalidade

Registrar:

```text
Descrição mental:
Desejos:
Medos:
Vínculos:
```

Este bloco deve ser suficiente para orientar a interpretação do personagem por jogador humano ou jogador IA.

## 9. Histórico e conhecimento

Registrar:

```text
Histórico relevante:
Conhecimento relevante:
```

`Histórico relevante` guarda fatos passados que ainda afetam a interpretação presente.

`Conhecimento relevante` guarda aquilo que o personagem sabe e que pode alterar suas decisões.

## Salvamento

Durante a criação assistida:

```text
base disponível
→ proposta
→ discussão
→ correção
→ aprovação explícita
→ salvamento
```

Conteúdo ainda em discussão não deve ser persistido como regra ou fato definitivo.

## Campo indefinido

Campo ainda não definido permanece vazio.

Nunca usar zero apenas para representar pendência.

```text
Força [ ]  → ainda não definido
Força [0]  → valor real definido como zero
```

## Arquivos antigos ainda não revisados

Outros arquivos copiados para `novo-motor/personagem/` podem ainda conter regras do motor anterior. Quando houver conflito com este arquivo, `ficha.md`, `atributos.md`, `pericias.md`, `poderes.md` e `organizacao-visual.md`, considerar esses arquivos atuais como referência do novo modelo até que o restante seja revisado explicitamente.
