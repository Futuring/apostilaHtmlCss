## Conhecendo a CSS

Além dos termos de HTML, existem alguns termos comuns de estilo CSS que você irá se familiarizar nos próximos dias. Esses termos são seletores, propriedades e valores. Tal como acontece com a terminologia HTML, quanto mais você trabalhar com CSS, mais esses termos se tornaram comuns para você.

### Seletores

Os elementos adicionados a uma página web podem ser estilizados utilizando CSS. Um seletor designa exatamente qual elemento ou elementos dentro do nosso HTML serão estilizados. Seletores podem possuir uma combinação de diferentes “filtros” para selecionar elementos únicos, tudo depende de quão específico queremos ser. Por exemplo, nós podemos querer selecionar todos os parágrafos em uma página ou selecionar apenas um parágrafo específico em uma página.

Seletores são geralmente especificados pelo valor de um atributo, como o valor de um id ou class, ou especificar o tipo de elemento, como `<h1>` ou `<p>`.

Dentro do CSS, selectores são seguidos por chaves, `{}` , que abrangem os estilos que serão aplicados ao elemento selecionado. O seletor aqui tem como alvo todos os elementos `<p>`.

```css
p { }
```

### Propriedades

Uma vez que um elemento é selecionado, uma propriedade determina os estilos que serão aplicados a esse elemento. Os nomes das propriedades ficam dentro de um seletor, dentro das chaves, `{}` , e imediatamente antes de dois pontos, `:` . Existem inúmeras propriedades que podemos usar, como `background`, `color`, `font-size`, `height`, e `width`, e novas propriedades são muitas vezes adicionados conforme a necessidade da comunidade. No código a seguir estamos definindo as propriedades `color` e `font-size` a serem aplicadas a todos os elementos `<p>`.
```css
p {
  color : ;
  font-size : ;
}
```

### Valores

Até agora, nós selecionamos um elemento com um seletor e determinamos o estilo que gostaríamos de aplicar através das propriedades. Agora podemos determinar o comportamento dessa propriedade com um valor. Os valores podem ser identificados como o texto entre os dois pontos, `:` e o ponto e vírgula, `;` . Aqui estamos selecionando todos elementos `<p>` e definindo o valor da propriedade `color` para ser `orange` e o valor da propriedade `font-size` para ser `16 pixels`.

```css
p {
  color : orange ;
  font-size : 16px ;
}
```

Revisando, no CSS nosso conjunto de regras começa com o seletor, que é imediatamente seguido por chaves. Dentro destas chaves existem declarações que consistem em pares de propriedade e valor. Cada declaração começa com uma propriedade, que é seguido por dois pontos, o valor da propriedade, e, finalmente, um ponto e vírgula.

É uma prática comum indentar os pares de propriedade e valor dentro das chaves. Como em HTML, essas indentações ajudam a manter nosso código organizado e legível.

![Sintaxe do CSS](http://learn.shayhowe.com/assets/images/courses/html-css/building-your-first-web-page/css-syntax-outline.png)

___

Conhecer alguns termos comuns e a sintaxe geral do CSS é um grande começo, mas temos mais alguns itens para aprender antes de irmos mais além. Antes nós precisamos aprender como trabalhar com seletores CSS.
