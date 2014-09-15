## Conhecendo o HTML

Embora estejamos começando com o HTML você provavelmente irá encontrar termos novos e algumas vezes estranhos. Com o tempo você vai se tornar mais e mais familiarizado com todos eles, mas os três termos mais comuns do HTML são: elementos, marcações e atributos.

### Elementos

Elementos são designadores que definem a estrutura e o conteúdo dos objetos dentro de uma página. Alguns dos elementos mais utilizados incluem títulos, parágrafos, listas e muitos mais.

Os elementos são identificadas pelo uso dos caracteres < (menor que) e > (maior que) em torno do nome do elemento. Assim, um elemento será parecido com o seguinte:

```html
<a>
```

### Marcações

O uso de < (menor que) e > (maior que) em torno de um elemento cria o que é conhecido como uma marcação ou tag, em inglês. Tags ocorrem mais comumente em pares de abertura e fechamento.

Uma tag de abertura marca o início de um elemento. Trata-se de um sinal de menor seguido pelo nome de um elemento e depois pelo sinal de maior; por exemplo, `<div>`.

A tag de fechamento marca o fim de um elemento. Trata-se de um sinal de menor seguido por uma barra e o nome do elemento e então pelo sinal de maior; por exemplo, `</div>`.

O conteúdo que cai entre a tag de abertura e a de fechamento é o conteúdo desse elemento. Um link de âncora, por exemplo, terá uma tag de abertura de `<a>` e uma tag de fechamento de `</a>`. O conteúdo entre essas duas tags será o conteúdo dessa âncora.

Logo, a marcação de uma âncora se parecerá com o seguinte:

```html
<a> ... </a>
```

### Atributos

Atributos são propriedades usadas para fornecer informações adicionais sobre um elemento. São atributos comuns o atributo `id`, que identifica um elemento; o atributo `class`, que classifica um elemento; o atributo `src`, que especifica uma fonte de conteúdo embutido; e o atributo `href`, que fornece uma referência de hiperlink para um recurso vinculado.

Os atributos são definidos dentro da tag de abertura, após o nome de um elemento. Geralmente atributos possuem um nome e um valor. O formato para esses atributos consiste no nome do atributo seguido por um sinal de igual e, em seguida, um valor de atributo citado. Por exemplo, um elemento `<a>` incluindo um atributo href seria parecido com o seguinte:

```html
<a href="http://futuring.com.bt/"> Futuring </a>
```

> #### Resultado
> [http://codepen.io/jlcarvalho/pen/qweFC](http://codepen.io/jlcarvalho/pen/qweFC)

O código anterior exibirá o texto "Futuring" na página da web e levará os usuários a http://futuring.com.br/ após clicarem no texto "Futuring". O elemento âncora é declarado com as tags de abertura `<a>` e fechamento `</a>` que englobam o texto, e o atributo de referência de hiperlink e valor são declarados com `href=”http://futuring.com.br"` na tag de abertura.

![Sintaxe do HTML](http://learn.shayhowe.com/assets/images/courses/html-css/building-your-first-web-page/html-syntax-outline.png)

Agora que você já conhece o que são os elementos, tags e atributos do HTML, vamos começar a criar nossa primeira página web. Se algo parecer novo aqui, não se preocupe, nós esclareceremos à medida que avançamos.
