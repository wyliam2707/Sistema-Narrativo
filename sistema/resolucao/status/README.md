# Status

Status: APROVADO

Esta pasta reúne condições e consequências temporárias que descrevem **como uma personagem está agora**.

Traços descrevem características consolidadas da personagem. Status descreve aquilo que está acontecendo no presente e pode entrar, mudar ou sair conforme a ficção.

> **Status define a condição. Poderes e outras fontes definem como ela é aplicada. Persistência registra o que continua ativo.**

---

## 1. Famílias nocivas

As famílias atuais são:

- **Sentidos:** Ofuscado → Cego / Surdo / Mudo → Privado;
- **Contenção:** Lento → Imóvel → Paralisado;
- **Terror:** Abalado → Apavorado → Aterrorizado;
- **Exaustão:** Fatigado → Exausto → Inconsciente;
- **Perturbação:** Desorientado → Confuso → Atordoado;
- **Aflição:** 1 de dano → 1d3 de dano → 1d6 de dano por Turno;
- **Posição:** Caído → Movido → Conduzido;
- **Influência:** Enfeitiçado → Compelido → Dominado;
- **Ruína:** Desprevenido → Exposto → Indefeso;
- **Debilitação:** Fraco → Debilitado → Prostrado.

Cada família possui sua definição em `nocivos/`.

A progressão representa **graus possíveis do mesmo tipo de efeito**. Não é obrigatório sofrer o primeiro estágio antes do segundo ou do terceiro.

---

## 2. Sobreposição na mesma família

Em cada família, apenas o efeito mais forte fica ativo.

```text
efeito mais forte
→ fica ativo

efeito mais fraco com duração menor ou igual
→ é descartado

efeito mais fraco com duração maior
→ continua contando duração, mas fica inativo enquanto o mais forte durar
```

Se dois efeitos tiverem a mesma força, prevalece o que tiver maior duração restante.

Durações **não se somam**.

Uma nova aplicação do mesmo efeito pode renovar sua duração:

> **usar a maior entre a duração restante e a nova duração completa.**

Quando o efeito mais forte terminar, um efeito mais fraco ainda válido pode voltar a ficar ativo.

A origem não muda essa regra: efeitos da mesma família competem mesmo quando vierem de fontes diferentes.

---

## 3. Famílias diferentes coexistem

Efeitos de famílias diferentes podem permanecer ativos ao mesmo tempo.

Exemplo:

```text
Cego
+ Imóvel
+ Fatigado
```

podem coexistir porque pertencem a famílias diferentes.

Isso não autoriza somar penalidades além do limite universal de dados. Quando várias fontes de `+d` ou `-d` se aplicarem à mesma resolução, aplicar as regras normais de cancelamento e limite `±2d` de `../motor-de-disputa.md`.

---

## 4. Ficção e mecânica

Um Status produz somente aquilo que sua definição estabelece e aquilo que decorre evidentemente da situação.

Não inventar penalidades adicionais apenas porque o nome do estado parece grave.

Da mesma forma, não fazer teste para confirmar uma consequência que já esteja determinada pela própria condição.

> **A regra fornece a base objetiva; a ficção fornece as consequências evidentes.**

---

## 5. Agência

Status pode limitar possibilidades e alguns efeitos podem impor comportamento dentro de um escopo explicitamente definido.

Isso não altera o `CONTROLE` estrutural da ficha.

Por exemplo, **Dominado** pode permitir à fonte impor uma ação específica enquanto sua regra estiver válida. Fora desse efeito, a autoridade voluntária normal da personagem permanece com sua persona.

Nenhum Status concede ao NARRADOR autoridade geral para escolher decisões voluntárias que sua regra não tenha removido ou imposto explicitamente.

---

## 6. Turno

Quando um Status usar duração ou aplicação por **Turno** durante combate:

> **Turno = intervalo pessoal da peça afetada, do início de uma vez dela até o início da próxima vez dela.**

A Rodada é global; o Turno é pessoal.

```text
posição da peça chega
→ começa seu Turno
→ atravessa o restante da Rodada
→ atravessa o início da Rodada seguinte
→ termina quando a mesma posição chega novamente
```

A regra de Status não cria uma Iniciativa própria nem outra fila de atuação.

A operação temporal pertence a `../../operacao/turnos-de-combate.md`.

---

## 7. Vida não é duplicada nesta pasta

A Vida já possui fontes canônicas especializadas em `../`:

- `../vida.md` — Vida Máxima e Incapacitado;
- `../recuperacao-da-vida.md` — recuperação e Medicina;
- `../combate-e-dano.md` — Dano, RD, Escudo/Barreira e aplicação em Vida.

Não criar outro `status/vida.md` apenas para duplicar essas regras.

---

## 8. Persistência

Status ativos são valores de estado atual.

Quando precisarem sobreviver entre cenas ou retomadas, registrar conforme:

```text
../../persistencia/status.md
../../persistencia/estado-atual.md
```

O arquivo persistente guarda o estado já estabelecido; não recalcula a regra.

---

## 9. Índice

- `nocivos/aflicao.md`
- `nocivos/contencao.md`
- `nocivos/debilitacao.md`
- `nocivos/exaustao.md`
- `nocivos/influencia.md`
- `nocivos/perturbacao.md`
- `nocivos/posicao.md`
- `nocivos/ruina.md`
- `nocivos/sentidos.md`
- `nocivos/terror.md`

## Regra final

> **Dentro da mesma família, vale o efeito mais forte; famílias diferentes coexistem. Quando houver duração por Turno em combate, usar o Turno pessoal definido por `operacao/turnos-de-combate.md`. Status descreve o presente e nunca substitui a regra de aplicação nem a arquitetura de agência.**
