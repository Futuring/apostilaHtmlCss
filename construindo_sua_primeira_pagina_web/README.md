# Construindo sua Primeira Página Web

Antes da invenção da Internet, não existiam Websites, e os livros impressos em papel eram a principal fonte de informação. E levava um tempo considerável para se conseguir encontrar a informação que você procurava.

Hoje você pode abrir um navegador web, abrir o Google e procurar facilmente. Qualquer bit de informação imaginável repousa em suas mãos. E há grandes chances de alguém em algum lugar ter construído um site com a informação que você precisa.

Através deste livro eu pretendo lhe mostrar como construir seus próprios sites usando as tecnologias mais utilizadas da plataforma web: HTML, CSS e JavaScript.

Antes de começarmos a nossa jornada para aprender a construir sites com HTML, CSS e JavaScript, é importante entender as diferenças entre as linguagens, a sintaxe de cada uma e alguma terminologia comum.

## O que são HTML, CSS e JavaScript?

O HTML , HyperText Markup Language, é uma linguagem de marcação utilizada para produzir páginas na web. Documentos HTML podem ser interpretados por navegadores. O HTML fornece a estrutura e significado do conteúdo das páginas web, definindo o que é o conteúdo como, por exemplo, cabeçalhos, parágrafos ou imagens.

O CSS , ou Cascading Style Sheets, é uma linguagem de folhas de estilo utilizada para definir a apresentação de documentos escritos em uma linguagem de marcação, como HTML ou XML. Seu principal benefício é prover a separação entre o formato e o conteúdo de um documento.

O JavaScript, ou simplesmente JS, é uma linguagem de programação do lado cliente, ou seja, é processada pelo próprio navegador. Com o JavaScript podemos criar efeitos especiais para nossas páginas na Web, além de podermos proporcionar uma maior interatividade com nossos usuários.

Com esse entendimento da diferença entre HTML, CSS e JavaScript, podemos prosseguir nossos estudos conhecendo o HTML com mais detalhes.

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
___
#### Resultado
[http://codepen.io/jlcarvalho/pen/qweFC](http://codepen.io/jlcarvalho/pen/qweFC)
___

O código anterior exibirá o texto "Futuring" na página da web e levará os usuários a http://futuring.com.br/ após clicarem no texto "Futuring". O elemento âncora é declarado com as tags de abertura `<a>` e fechamento `</a>` que englobam o texto, e o atributo de referência de hiperlink e valor são declarados com `href=”http://futuring.com.br"` na tag de abertura.

![Sintaxe do HTML](http://learn.shayhowe.com/assets/images/courses/html-css/building-your-first-web-page/html-syntax-outline.png)

Agora que você já conhece o que são os elementos, tags e atributos do HTML, vamos começar a criar nossa primeira página web. Se algo parecer novo aqui, não se preocupe, nós esclareceremos à medida que avançamos.

## Criação da estrutura do documento HTML

Documentos HTML são documentos de texto simples salvos com a extensão de arquivo `.html` ao invés de `.txt`. Para começar a escrever HTML, você precisa primeiro de um editor de texto simples que você se sinta confortável usando. Infelizmente isso não inclui o Microsoft Word ou o Pages, pois estes são editores de texto rico. Dois dos mais populares editores de texto simples para escrever HTML, CSS e JavaScript são Dreamweaver e Sublime Text. Existem alternativas como o Notepad++ para Windows e o Atom para Mac.

Todos os documentos HTML têm uma estrutura exigida, que inclui a seguinte declaração e elementos: `<!DOCTYPE html>` , `<html> `, `<head>` e `<body>`.

A declaração do tipo de documento, ou `<!DOCTYPE html>`, informa aos navegadores qual versão do HTML está sendo usado e é colocado no início do documento HTML. Como nós vamos estar usando a última versão do HTML, a nossa declaração de tipo de documento é simplesmente `<!DOCTYPE html>`. Após a declaração do tipo de documento, o elemento `<html>` significa o início do documento.

Dentro do elemento `<html>`, o elemento `<head>` identifica a parte superior do documento, incluindo quaisquer metadados (informações extras sobre a página). O conteúdo dentro do elemento `<head>` não é exibido na página web em si. Em vez disso, podemos incluir o título do documento (que é exibido na barra de título na janela do navegador), links para todos os arquivos externos, ou qualquer outro metadados necessário.

Todo o conteúdo visível dentro da página web ficará dentro do elemento `<body>`. A estrutura comum de um documento HTML fica assim:

```html
<!DOCTYPE html>
<html lang="pt-br">
  <head>
    <meta charset="utf-8">
    <title>Olá Mundo</title>
  </head>
  <body>
    <h1>Olá Mundo</h1>
    <p>Essa é uma página web.</p>
  </body>
</html>
```

___
#### Resultado
[http://codepen.io/jlcarvalho/pen/pDCbi](http://codepen.io/jlcarvalho/pen/pDCbi)
___

O código anterior mostra um documento começando com a declaração de tipo de documento `<!DOCTYPE html>`, seguido pelo elemento `<html>`. Dentro do elemento `<html>` vem os elementos `<head>` e `<body>`. O elemento `<head>` inclui a codificação de caracteres da página através da tag `<meta charset="utf-8">` e o título do documento através do elemento `<title>`. O elemento `<body>` inclui um título através do elemento `<h1>` e um parágrafo através do elemento `<p>`. Como tanto o título quanto o parágrafo são aninhados dentro do elemento `<body>`, eles são visíveis na página web.

Colocar um elemento é dentro de outro elemento é conhecido como aninhar elementos e é uma boa prática para manter a estrutura do documento bem organizado e legível. No código anterior, tanto os elementos `<head>` e `<body>` foram aninhados e indentandos dentro do elemento `<html>`. O padrão de indentação continua conforme novos elementos são adicionados dentro dos elementos `<head>` e `<body>`.

___
#### Elementos de fechamento automático

No exemplo anterior, o elemento `<meta>` tinha apenas uma tag e não incluía uma tag de fechamento. Pos nem todos os elementos possuem de abertura e fechamento. Alguns elementos podem simplesmente receber o seu conteúdo ou o comportamento de atributos dentro de uma única tag. O elemento `<meta>` é um desses elementos. O conteúdo do elemento `<meta>` anterior é atribuído com o uso do atributo charset e seu valor. Outros elementos de fechamento automático são: `<br>`, `<embed>`, `<hr>`, `<img>`, `<input>`, `<link>`, `<param>`, `<source>` e `<wbr>`.

#### Validação de Código

Não importa o quão cuidadoso nós somos, ao escrever o nosso código, inevitavelmente cometeremos erros. Felizmente, ao escrever HTML e CSS temos validadores para verificar o nosso trabalho. O W3C tem construído tanto validadores HTML e CSS que analisam o código em busca de erros. Validar nosso código não só ajuda a processar corretamente a página web em todos os navegadores, mas também nos ajuda a conhecer as melhores práticas recomendadas para escrever código.
___

## Na Prática

Como web designers e desenvolvedores de front-end, temos o luxo de assistir a um grande número de conferências dedicadas ao nosso ofício. Nós vamos fazer a nossa própria conferência, a Styles Conference, e construiremos um site para ela ao longo das próximas lições.
1. Abra o editor de texto e crie um arquivo chamado index.html e salve-o em um local de sua preferência. Recomendo que você crie uma pasta em sua área de trabalho chamada “Styles Conference” e salve o arquivo nela.
2. Dentro do arquivo `index.html` vamos adicionar a estrutura do documento, incluindo o `<!DOCTYPE html>` e os elementos `<html>` , `<head>` e `<body>`.
```html
<!DOCTYPE html>
<html lang="pt-br">
  <head>
  </head>
  <body>
  </body>
</html>
```
3. Dentro do elemento `<head>`, vamos adicionar os elementos `<meta>` e `<title>`. O elemento `<meta>` deve incluir o atributo `charset` adequado e seu valor, enquanto o elemento `<title>` deve conter o título da página, que será "Styles Conference".
```html
<head>
  <meta charset="utf-8">
  <title> Styles Conference </title>
</head>
```
4. Dentro do elemento `<body>`, vamos adicionar os elementos `<h1>` e `<p>`. O elemento `<h1>` deve incluir o título que deseja incluir, vamos usar "Styles Conference" novamente, e o elemento `<p>` deve incluir um simples parágrafo de apresentação de nossa conferência.
```html
<body>
  <h1>Styles Conference</h1>
  <p>Todos os anos os mais brilhantes web designers e desenvolvedores front-end se reúnem em Goiânia para discutir as mais recentes tecnologias. Junte-se a nós neste mês de Julho!</p>
</body>
```
5. Agora é hora de ver o que nós fizemos! Vamos encontrar o nosso arquivo index.html (foi recomendado que o salvasse na pasta “Styles Conference” em sua área de trabalho). Ao clicar duas vezes neste arquivo ele abrirá em um navegador e nós poderemos visualizar o resultado.

___

Agora vamos dar uma olhada em como funciona o CSS. Lembre-se, o HTML irá definir o conteúdo e a estrutura das nossas páginas web, enquanto o CSS irá definir o estilo visual e a aparência de nossas páginas da web.

## Entendimento comum Termos CSS

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



