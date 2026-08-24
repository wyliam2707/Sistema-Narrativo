# Personagem — Novo Motor

Status: EM DESENVOLVIMENTO

Esta pasta contém a versão experimental da estrutura de personagens do `novo-motor/`.

Ela foi copiada originalmente de `sistema/personagem/`, mas está sendo revisada separadamente. Nada aqui altera automaticamente o sistema canônico.

> **Quando houver conflito, os arquivos já revisados abaixo têm precedência dentro do `novo-motor/`.**

## Arquivos já alinhados ao novo modelo

- `ficha.md` — ficha-base consolidada atual;
- `atributos.md` — seis Atributos: Força, Destreza, Agilidade, Intelecto, Percepção e Presença;
- `pericias.md` — lista atual de 8 Perícias comuns e 8 somente treinadas, sem combate;
- `poderes.md` — ficha lista apenas nomes; detalhes são consultados sob demanda em arquivos próprios;
- `organizacao-visual.md` — ordem e apresentação visual atual da ficha;
- `criacao.md` — fluxo atual de criação e revisão por blocos.

## Estrutura atual da ficha

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

### Descrição

Inclui identificação e metadados:

```text
Nome: Codinome — Nome real
Importância:
Controle:
Idade:
Peso:
Altura:
Descrição visual:
```

### Atributos

```text
Corpo - Força [ ] | Destreza [ ] | Agilidade [ ]
Mente - Intelecto [ ] | Percepção [ ] | Presença [ ]
```

### Perícias

Perícias representam exploração, conhecimento e interação com o mundo.

Combate fica separado em `Luta`, `Disparo` e `Magia`.

### Referências

Reúne capacidades estáveis de consulta rápida:

```text
Vida [ ] | Energia [ ] | Deslocamento: ... | Visão: ...
Defesas - Esquiva [ ] | Vontade [ ] | Fortitude [ ] | RD: ...
```

`Referências` não é o estado momentâneo da cena.

### Ataques

```text
Luta [ ] / arma / dano / crítico / alcance
Disparo [ ] / arma / dano / crítico / alcance
Magia [ ] / arma ou efeito / dano / crítico / alcance
```

### Poderes

A ficha registra apenas os nomes dos Poderes. O conteúdo completo de cada Poder será mantido em arquivo próprio e consultado apenas quando necessário.

### Recursos

Registra meios, infraestrutura, acesso ou bens realmente relevantes, sem virar inventário comum.

### Personalidade

```text
Descrição mental:
Desejos:
Medos:
Vínculos:
```

### Histórico

```text
Histórico relevante:
Conhecimento relevante:
```

Esses dois campos ajudam um jogador IA a interpretar o personagem sem usar informação que ele não deveria conhecer.

## Arquivos ainda herdados do motor anterior

Os demais arquivos desta pasta ainda podem conter conceitos, nomes, escalas ou procedimentos do motor anterior.

Eles permanecem como material de referência experimental até revisão explícita.

Não usar uma regra herdada para sobrescrever uma decisão já registrada nos arquivos atuais acima.

## Separação do sistema canônico

O conteúdo canônico continua em:

```text
sistema/personagem/
```

A migração do novo motor para `sistema/` só deve acontecer depois de decisão explícita e revisão final.
