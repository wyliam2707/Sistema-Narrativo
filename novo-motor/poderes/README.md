# Poderes

Esta pasta reúne as regras gerais e os arquivos individuais dos **Poderes** do Novo Motor.

Um Poder representa uma ação extraordinária usada deliberadamente para produzir um efeito. A descrição define sua aparência e origem ficcional; o **Hub** define aquilo que ele pode fazer mecanicamente.

---

# Estrutura geral

Um Poder pode possuir **Dano**, **Efeito** ou ambos.

A sequência padrão dos Poderes ofensivos é:

> **Defesa → Dano → Resistência → Efeito**

Nem todo Poder utiliza todas as etapas. Poderes não ofensivos usam apenas as etapas que fizerem sentido para sua própria natureza.

Toda resolução segue a regra universal do sistema: o resultado final sempre conserva **4 dados + Atributo**. Bônus e penalidades modificam a quantidade de dados rolados antes da escolha dos quatro resultados, conforme [../regras-gerais.md](../regras-gerais.md).

---

# Acerto e Defesa por contexto

Quando um Poder precisa atingir ou superar alguém, Acerto e Defesa são resolvidos como uma oposição:

> **4 dados + Atributo de Acerto × 4 dados + Atributo de Defesa**

O Atributo é determinado pela **forma real da ação e da reação**.

- o Acerto usa o Atributo coerente com a maneira como o Poder está sendo aplicado;
- a Defesa usa o Atributo coerente com a maneira como o alvo tenta evitar, bloquear ou resistir à ação;
- não existe escolha automática do maior Atributo apenas para obter vantagem;
- se um Poder possuir uma regra própria explícita de Atributo, essa regra é usada naquele Poder.

Exemplos:

- um ataque dirigido por precisão física pode usar **Controle**;
- uma tentativa de impor força física pode usar **Potência**;
- uma invasão mental pode usar um Atributo de Mente coerente com sua forma;
- esquivar-se normalmente pode usar **Controle**;
- suportar fisicamente algo pode usar **Resistência**;
- resistir a uma agressão mental pode usar **Vontade**.

A origem de um Poder não fixa sozinha o Atributo. Um efeito mágico pode produzir uma ameaça física, e um efeito físico pode exigir uma resposta diferente conforme a ficção.

---

# Defesa

A Defesa é resolvida antes do Dano e da Resistência do Efeito.

## Defesa [Absoluta]

Se a Defesa vencer:

- não há Dano;
- o Efeito é anulado antes da Resistência.

## Defesa [Total]

Se a Defesa vencer:

- não há Dano;
- o Efeito ainda pode seguir para Resistência.

## Defesa [Parcial]

Se a Defesa vencer:

- o alvo sofre metade do Dano;
- o Efeito ainda pode seguir para Resistência.

## Defesa [Nula]

Não existe etapa de Defesa.

Isso não transforma uma ação ficcionalmente impossível em possível. Alvo, alcance e demais condições ainda precisam existir.

---

# Dano

O Dano é aplicado depois da Defesa.

O resultado da Defesa determina se o alvo sofre Dano normal, metade do Dano ou nenhum Dano.

Cada Poder define sua própria progressão de Dano e o Atributo somado quando houver um.

---

# Resistência do Efeito

Quando um Efeito possuir Resistência, a oposição usa os Atributos coerentes com a **natureza do Efeito e com a forma de resistência do alvo**.

> **Não existe uma combinação universal obrigatória de Atributos para todos os Efeitos.**

Use **Potência × Resistência** apenas quando essa oposição realmente representar o que está acontecendo, como em certas formas de contenção ou imposição física.

Outros efeitos podem usar Atributos de Mente ou outras combinações coerentes. Por exemplo, medo sobrenatural pode envolver **Presença × Vontade**, enquanto uma invasão mental pode envolver **Intelecto × Vontade**.

A Resistência só ocorre quando o próprio Poder possuir essa etapa. Ações que já forem tratadas integralmente como uma oposição de combate não recebem uma segunda Resistência por inferência.

## Efeito [Total]

Se a Resistência vencer, o Efeito é anulado.

## Efeito [Parcial]

Se a Resistência vencer, o Efeito é reduzido em uma posição da progressão.

Se o primeiro estágio for reduzido, nenhum Efeito é aplicado.

## Efeito [Nula]

Não existe etapa de Resistência.

---

# Distâncias narrativas

As distâncias são categorias narrativas. Os valores em metros são referências médias, não uma régua rígida.

- **Si Mesmo** — o próprio usuário.
- **Toque** — contato físico.
- **Próximo** — cerca de 3 m.
- **Curto** — cerca de 20 m.
- **Médio** — cerca de 45 m.
- **Longo** — cerca de 90 m.

Acima de Longo, a distância normalmente depende de um Poder próprio, como Teleporte.

---

# Hub e custo

Um Poder é configurado por seu **Hub**.

`[X]` representa o máximo de **Mana** que pode ser gasto em um único uso daquele Poder. A origem de Mana e de `[X]` será definida na regra central de Mana.

Salvo quando o arquivo do Poder disser o contrário:

- a primeira posição de uma progressão custa `+0`;
- cada avanço seguinte custa `+1`;
- opções ramificadas no mesmo estágio possuem o mesmo custo daquele estágio;
- o custo final é a soma das escolhas;
- o custo nunca pode ultrapassar `[X]`.

Não é necessário repetir esses custos em todos os arquivos de Poder.

Antes de resolver um uso configurável, o Narrador apresenta a configuração e o custo e pergunta apenas:

> **Confirmar uso por X Mana?**

---

# Campos do Hub

Um Poder apresenta apenas os campos necessários à sua função. Entre os campos já utilizados estão:

- Alcance;
- Alvos;
- Área;
- Dano;
- Efeito;
- Defesa;
- Duração;
- Conjuração;
- Referência;
- Tipo;
- Modo;
- Distância;
- Escopo;
- Contra;
- Tamanho;
- Material;
- outras progressões específicas do próprio Poder.

A existência de um campo em um Poder não obriga outros Poderes a possuírem o mesmo campo.

---

# Alvos e Área

Nos Poderes que indicarem **Alvos ou Área**, as duas linhas são modos alternativos de aplicação:

- **Alvos:** escolhe entidades individualmente;
- **Área:** afeta a região determinada conforme a regra do Poder;
- apenas a opção usada entra no custo.

Outros Poderes podem usar Área com função diferente, como busca, percepção ou espaço de uma Ilusão.

## Múltiplos Alvos e Acerto

Quando um único uso de Poder atingir **mais de um Alvo** e exigir uma rolagem de Acerto, o usuário realiza **uma única rolagem de Acerto** para todo o uso.

Cada Alvo resolve sua própria Defesa contra esse mesmo resultado de Acerto.

> **Um uso do Poder = uma rolagem de Acerto; cada Alvo = sua própria Defesa.**

Assim, diferentes Alvos podem sofrer resultados diferentes dentro do mesmo uso: alguns podem ser atingidos e outros podem se defender.

Empates seguem a regra geral de oposição: favorecem quem iniciou a ação.

---

# Chassi padrão dos Poderes de Efeito nocivo

As famílias de Efeito nocivo normalmente usam:

> **Alcance:** Curto → Médio → Longo  
> **Alvos:** 1 → 2 → 4 → 8  
> **Área:** Toque → Próximo → Curto  
> **Dano:** Nenhum → 1d6 → 2d6  
> **Efeito:** progressão da família  
> **Defesa:** Total → Parcial  
> **Resistência do Efeito:** Total → Parcial → Nula  
> **Duração:** Turno → Cena → Hora

Esse chassi é uma base, não uma obrigação quando a natureza do Efeito exigir uma estrutura própria. **Posição**, por exemplo, possui resultados de deslocamento instantâneo e não utiliza Duração comprada.

As famílias atuais são:

- **Sentidos:** Ofuscado → Cego / Surdo / Mudo → Privado;
- **Contenção:** Lento → Imóvel → Paralisado;
- **Terror:** Abalado → Apavorado → Aterrorizado;
- **Exaustão:** Fatigado → Exausto → Inconsciente;
- **Perturbação:** Desorientado → Confuso → Atordoado;
- **Aflição:** 1 de dano → 1d3 de dano → 1d6 de dano por turno;
- **Posição:** Caído → Movido → Conduzido;
- **Influência:** Enfeitiçado → Compelido → Dominado;
- **Ruína:** Desprevenido → Exposto → Indefeso;
- **Debilitação:** Fraco → Debilitado → Prostrado.

---

# Tempo

A terminologia temporal do Novo Motor é:

> **Instante → Turno → Cena → Hora → Dia**

Quando um Poder produz seu efeito imediatamente, use **Instante**. Arquivos antigos que ainda usem “Imediata”, “Instantâneo” ou “Instantânea” devem ser entendidos como versões antigas do mesmo conceito e podem ser padronizados.

---

# Índice dos Poderes

A lista curta para consulta da ficha está em [../ficha/poderes.md](../ficha/poderes.md). Cada regra completa permanece no arquivo individual deste diretório.