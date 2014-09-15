## Trabalhando com Seletores

Seletores, como mencionado anteriormente, indicam quais elementos HTML estão sendo estilizados. É importante compreender como usar os seletores e como eles podem ser aproveitados. O primeiro passo é se familiarizar com os diferentes tipos de seletores. Vamos começar com os seletores mais comuns: seletores de `tipo`, `class` e `ID`.

### Seletores de Tipo

Seletores de tipo tem como objetivo elementos de seu tipo de elemento. Por exemplo, se queremos selecionar todos os elementos de divisão, `<div`>, podemos usar um seletor de tipo `div`. O código a seguir mostra um seletor de tipo de elementos de divisão, bem como o HTML correspondente que ele seleciona.

```css
div { }
```

```html
<div>...</div>
<div>...</div>
```

### Seletores de Classe

Seletores de classe nos permitem selecionar um elemento baseado no elemento class e valor de seu atributo. Seletores de classe são um pouco mais específicos do que os seletores de tipo, pois selecionam um determinado grupo de elementos, em vez de todos os elementos de um tipo.

Seletores de classe nos permitem aplicar os mesmos estilos a diferentes elementos de uma só vez, usando a mesma classe valor do atributo em vários elementos.

Dentro do CSS as classes são escritas usando um ponto, `.` , seguido pelo valor do atributo `class`. Aqui, o seletor de classe irá selecionar qualquer elemento que contenha o valor do atributo class igual a awesome, incluindo os elementos de divisão e de parágrafo.

```css
.awesome { }
```

```html
<div class="awesome"> ... </div>
<p class="awesome"> ... </p>
```

### Seletores de ID

Seletores de ID são ainda mais específicos do que os seletores de classe, pois eles possuem como alvo apenas um único elemento de cada vez. Assim como seletores de classe usam do valor do atributo `class` de um elemento os seletores ID utilizam o valor do atributo `ID` de um elemento como seletor.

Independentemente de qual tipo de elemento que apareça, o valor do atributo ID só pode ser usado uma vez por página. Quando usados, devem ser reservados para elementos importantes.

No CSS seletores de ID são representados por um símbolo de cerquilha, `#` , seguido do valor do atributo `ID`. Aqui o seletor ID só vai selecionar o elemento que contém o valor do atributo ID `futuring`.

```css
#futuring { }
```

```html
<div id="futuring"> ... </div>
```

### Seletores Adicionais

Os seletores CSS são extremamente poderosos e os que foram descritos aqui são os seletores mais comuns que vamos encontrar. Estes seletores são apenas o começo. Existem ainda diversos seletores avançados que podemos utilizar. Quando você se sentir confortável com esses seletores, não tenha medo de olhar para alguns dos seletores mais avançados.

Tudo bem, as coisas estão começando a fazer sentido. Nós adicionamos elementos a uma página dentro do nosso HTML, e então podemos selecionar aqueles elementos e aplicar estilos a eles usando CSS. Agora vamos ligar os pontos entre o nosso HTML e CSS, fazendo com que essas duas linguagens de trabalho em conjunto.
