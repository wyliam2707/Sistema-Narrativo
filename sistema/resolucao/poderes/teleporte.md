# Teleporte

Poder de movimento que desloca alvos instantaneamente ou cria uma passagem entre dois pontos.

## Hub

**Teleporte [X]**  
**Alcance:** Toque → Próximo → Curto  
**Conjuração:** Cena → Turno → Instante  
**Alvos:** 1 → 2 → 4 → 8  
**Modo:** Direto → Portal  
**Distância:** Longa → Familiar → Conhecida → Descrita → Astral  
**Duração:** Direto = Instante / Portal = Cena

`[X]` é o máximo de Mana que pode ser gasto no uso do Poder.

## Custo

A primeira posição de cada progressão custa `+0 Mana`; cada avanço posterior custa `+1 Mana`.

- **Alcance:** Toque `+0` → Próximo `+1` → Curto `+2`
- **Conjuração:** Cena `+0` → Turno `+1` → Instante `+2`
- **Alvos:** 1 `+0` → 2 `+1` → 4 `+2` → 8 `+3`
- **Modo:** Direto `+0` → Portal `+1`
- **Distância:** Longa `+0` → Familiar `+1` → Conhecida `+2` → Descrita `+3` → Astral `+4`

O custo total é a soma dos avanços escolhidos e nunca pode ultrapassar `[X]`.

## Conjuração

- **Cena:** exige preparação ao longo da Cena antes de produzir o efeito.
- **Turno:** exige preparação durante um intervalo simultâneo completo de até 10 segundos. O efeito é concluído no fechamento daquele Turno se a preparação continuar válida e não tiver sido interrompida.
- **Instante:** o efeito é produzido no instante causal em que for resolvido dentro do Turno ou da cena, sem exigir um intervalo completo de preparação.

`Conjuração` mede tempo necessário para produzir o efeito. Ela não cria iniciativa, fila de atuação ou economia de uma ação por Turno. Interferências durante a preparação seguem `../../operacao/turnos-de-combate.md`.

## Modos

### Direto

Move os alvos selecionados para um destino válido dentro da Distância escolhida.

A duração é **Instante**.

### Portal

Cria uma passagem entre a origem e um destino válido dentro da Distância escolhida.

O Portal permanece aberto durante a **Cena**.

## Alcance e Alvos

**Alcance** determina até onde o usuário pode selecionar os alvos ou estabelecer a origem do Portal.

**Alvos** determina quantos indivíduos podem ser deslocados pelo modo Direto no mesmo uso.

## Alvo involuntário

Tentar teleportar uma criatura contra sua vontade é tratado como **ação de combate**:

> **Acerto × Defesa**

Os Atributos são escolhidos conforme a forma real do Teleporte e da reação do alvo.

Se o usuário vencer, o alvo é teleportado para o destino válido. Se a Defesa vencer, o alvo não é teleportado.

Essa oposição resolve a tentativa inteira. **Não existe uma segunda Resistência depois da Defesa.**

## Distância e referência do destino

A progressão de Distância representa até onde e com que grau de referência o destino pode ser estabelecido.

O Teleporte não adivinha destinos. Para teleportar-se, o usuário precisa conseguir **situar minimamente o destino** no espaço, no mundo ou no plano correspondente.

- **Longa:** qualquer ponto válido dentro do alcance narrativo Longo.
- **Familiar:** um local que o usuário conhece bem por presença frequente ou convivência direta suficiente para reconhecê-lo com segurança.
- **Conhecida:** um local em que o usuário já esteve pelo menos uma vez ou cuja posição conhece exatamente, mesmo sem grande familiaridade.
- **Descrita:** um local em que o usuário nunca esteve, mas cuja posição pode ser estabelecida por uma referência externa suficiente, como mapa, coordenadas, endereço, carta, descrição geográfica ou equivalente. A precisão é limitada pela própria referência: se ela identifica apenas uma região ou construção ampla, o ponto de chegada também será aproximado.
- **Astral:** permite alcançar outro plano, dimensão ou espaço equivalente, mas continua exigindo uma referência válida capaz de identificar esse destino. O usuário não precisa ter visitado o plano, porém não pode viajar para um plano que não consiga referenciar minimamente.

## Precisão e lógica da cena

A precisão do ponto de chegada é limitada pela **qualidade real da referência disponível na ficção**.

> **Conhecer onde fica um lugar não significa conhecer todos os pontos dentro dele.**

Quando a referência identifica apenas uma região, construção, cidade, fortaleza ou outro local amplo, o Teleporte leva para as **proximidades coerentes daquela referência**. A margem pode ser pequena ou chegar a alguns quilômetros quando a informação disponível for ampla ou imprecisa.

O Teleporte não cria conhecimento que o personagem não possui e não transforma uma referência ampla em coordenadas internas exatas.

Exemplos:

- teleportar-se para o **banheiro da própria casa** é plausível quando o personagem conhece aquele ponto de forma familiar e precisa;
- um mapa que apenas mostre onde fica o **castelo do vilão** permite chegar às proximidades do castelo, talvez ainda a alguns quilômetros dele conforme a escala e a precisão do mapa;
- nunca ter estado no castelo não permite escolher automaticamente o pátio, a sala do tesouro, um quarto específico ou qualquer outro ponto interno desconhecido;
- saber que um item está em algum lugar dentro do castelo não cria uma referência suficiente para teleportar-se diretamente até ele;
- se o personagem conhece exatamente uma sala, corredor ou outro ponto interno por experiência própria ou por uma referência suficientemente precisa, esse ponto pode ser um destino válido;
- um mapa planar, coordenada mística, texto ou outra referência capaz de identificar um plano pode permitir **Astral** mesmo sem visita anterior.

> **O Teleporte leva até onde a referência permite. Ele não transforma informação incompleta em precisão perfeita.**

> **Se o destino não puder ser minimamente localizado ou identificado, o Teleporte é impossível.**

A ficção ainda determina se o destino existe, pode ser identificado e é alcançável pelo Poder.
