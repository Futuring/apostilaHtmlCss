## Construindo a Estrutura

Durante muito tempo a estrutura de uma página web era construída utilizando `<div>`. O problema era que as divisões não forneciam nenhum valor semântico, e era bastante difícil determinar o prppósito dessas divisões. Felizmente o HTML5 introduziu novos elementos estruturais, incluindo os elementos `<header>`, `<nav>`, `<article>`, `<section>`, `<aside>` e `<footer>`.

Todos estes novos elementos têm a intenção de dar um sentido para a organização de nossas páginas e melhorar nossos semântica estrutural. Eles são todos os elementos bloco e não tem qualquer posição implícita ou estilo. Além disso, todos estes elementos podem ser utilizados várias vezes por página, enquanto, refletindo o significado semântico adequado.

Vamos arregaçar as mangas e dar uma olhada.

![Estrutura HTML](http://learn.shayhowe.com/assets/images/courses/html-css/getting-to-know-html/building-structure.png)

### Cabeçalho

O elemento `<header>` é utilizado para identificar o topo de uma página, artigo, seção ou outro segmento de uma página. Em geral, o elemento `<header>` pode incluir um título, o texto introdutório e ainda a navegação.

```html
<header> ... </header>
```

> #### `<header>` vs `<head>` vs Elementos do `<h1>` ao `<h6>`
É fácil confundir o elemento `<header>` com o elemento <head> ou os elementos de título, do `<h1>` ao `<h6>`. Todos eles possuem diferentes significados semânticos e devem ser utilizados de acordo com os seus significados.

> O elemento `<header>` é um elemento estrutural que define o título de um segmento de uma página. Ele se enquadra no elemento `<body>`.

> O elemento `<head>` não é exibido em uma página e é usado para descrever os metadados, incluindo o título do documento e links para arquivos externos. Ele deve ser inserido diretamente no elemento `<html>`.

> Os elementos de título, do `<h1>` ao `<h6>`, são usados para designar vários níveis de títulos de texto em toda a página.

### Navegação

O elemento `<nav>` identifica uma seção de links de navegação principais em uma página. O elemento `<nav>` deve ser reservada apenas para as seções de navegação primárias, tais como a navegação global, uma tabela de conteúdo, links anterior/próximo, ou outros grupos importantes de links de navegação.

Mais comumente, os links incluídos no elemento `<nav>` ligam para outras páginas dentro do mesmo site ou de partes da mesma página web. Outros links não devem ser inseridos dentro do elemento `<nav>`, eles devem usar o elemento âncora, `<a>`.

```html
<nav> ... </nav>
```

### Artigo

O elemento `<article>` é utilizado para identificar uma seção de conteúdo independente, que pode ser distribuído ou reutilizado de forma independente. Nós muitas vezes iremos usar o elemento `<article>` para representar posts, artigos de jornal, conteúdo enviado pelo usuário, e assim por diante.

Antes de utilizar o elemento `<article>`, é preciso determinar se o conteúdo dentro do elemento pode ser replicado em outros lugares, sem qualquer confusão. Se o conteúdo dentro do elemento `<article>` for retirado do contexto da página e colocado, por exemplo, dentro de um e-mail ou obra impressa o conteúdo ainda deve fazer sentido.

```html
<article> ... </article>
```

### Seção

O elemento `<section>` é usado para identificar um agrupamento temático de conteúdo, o que geralmente, mas não sempre, inclui um cabeçalho. O agrupamento de conteúdo dentro do elemento `<section>` pode ser de natureza genérica, mas é útil para identificar todo o conteúdo como relacionados.

O elemento `<section>` é comumente usado para fornecer hierarquia para uma página.

```html
<section> ... </section>
```

### Decidindo entre os elementos `<article>`, `<section>` e `<div>`

Às vezes é bastante difícil decidir qual elemento (`<article>`, `<section>` ou `<div>`) é o melhor elemento para o trabalho com base em seu significado semântico. O truque aqui, como em toda decisão semântica, é olhar para o conteúdo.

Tanto os elementos `<article>` e `<section>` contribuem para a estrutura de um documento e ajudam a delinear um documento. Se o conteúdo está sendo agrupados exclusivamente para fins de estilo e não fornece valor semântico para o documento, utilize o elemento `<div>`.

Se o conteúdo possui semântica e pode ser redistribuído ou utilizado de forma independente, utilize o `<article>` elemento.

Se o conteúdo possui semântica e representa um grupo temático de conteúdo, utilize o elemento `<section>`.

### Aside

O elemento `<aside>` contém conteúdo, como barras laterais, inserções, ou breves explicações, ou seja, tangencialmente relacionadas com o conteúdo que o rodeiam. Quando usado dentro de uma elemento `<article>`, por exemplo, o elemento `<aside>` pode identificar o conteúdo relacionado com o autor do artigo.

Podemos instintivamente pensar em um elemento `<aside>` como um elemento que aparece para o lado esquerdo ou direito da página. Temos que lembrar, porém, que todos os elementos estruturais, incluindo o elemento `<aside>`, são elementos bloco e, como tal, irão aparecer em uma nova linha, ocupando a largura total da página, ou do elemento em que ele está aninhado dentro, também conhecido como seu elemento pai.

```html
<aside> ... </aside>
```

Vamos discutir como mudar a posição de um elemento, colocando o para a direita ou para a esquerda de um grupo de conteúdo, na Lição 5, "Posicionando o Conteúdo".

### Rodapé

O elemento `<footer>` identifica o fechamento ou final de uma página, um artigo, seção ou outro segmento de uma página. Geralmente o elemento `<footer>` é encontrado na parte inferior do seu pai. O conteúdo dentro do elemento `<footer>` deve ser informação relativa e não deve divergir do documento ou seção que está incluído.

```html
<footer> ... </footer>
```

Com elementos estruturais e elementos baseados em texto o nosso conhecimento HTML está realmente começando a fazer sentido. Agora é um bom momento para rever nosso site Styles Conference e ver se podemos melhorar um pouco sua estrutura.
