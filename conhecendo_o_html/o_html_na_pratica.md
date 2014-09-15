## O HTML na Prática

Atualmente, nosso site da Styles Conference carece de estrutura e conteúdo. Vamos levar algum tempo para aperfeiçoar a nossa home page.

1. Usando nosso arquivo index.html existente, vamos adicionar em um elemento `<header>`. Nosso elemento `<header>` deve incluir nosso elemento `<h1>` existente. Vamos também adicionar um elemento `<h3>` como um slogan para apoiar o nosso elemento `<h1>`. <br><br>
```html
<header>
  <h1>Styles Conference </h1>
  <h3>19 de julho - Goiânia, GO</h3>
</header>
```
2. Depois do nosso elemento `<header>`, vamos adicionar um novo grupo de conteúdo, usando o elemento `<section>`, que apresenta nossa conferência. Vamos começar esta seção com um novo elemento `<h2>` e terminá-la com o nosso parágrafo já existente. <br><br>
```html
<section>
  <h2>Dedicada à construção de sites</h2>
  <p>Todos os anos os mais brilhantes web designers e desenvolvedores front-end se reúnem em Goiânia para discutir as mais recentes tecnologias. Junte-se a nós neste mês de Julho!</p>
</section>
```
3. Após a introdução de nossa conferência, vamos adicionar um outro grupo de conteúdo que apresentam algumas das páginas que estaremos adicionando, especificamente as páginas dos palestrantes, cronograma e localização. Cada uma das páginas que estamos apresentando também deve estar dentro de sua própria seção e incluir um texto de introdução. <br><br>Nós vamos agrupar todos as apresentações dentro de um elemento `<section>`, e cada introdução individual será apresentada dentro de um elemento `<section>` também. Ao todo, teremos três elementos `<section>` dentro de outro elemento `<section>`. <br><br>
```html
<section>
    <section>
        <h5>Palestrantes</h5>
        <h3>Conceituados internacionalmente</h3>
        <p>Vindos de todo o país, são mais de vinte palestrantes nacionais de renome internacional.</p>
    </section>
    <section>
        ...
    </section>
</section>
```
4. Por último, vamos adicionar o nosso autor dentro do elemento `<footer>` no final da nossa página. Para isso vamos usar o elemento `<small>`, que semanticamente representa comentários laterais e letras pequenas, perfeito para Copyright. <br><br> Geralmente, o conteúdo dentro do elemento `<small>` será processado de forma bem pequena, mas o nosso CSS reset vai impedir que isso aconteça. <br><br>
```html
<footer>
    <small>© Styles Conference</small>
</footer>
```

Agora podemos ver a nossa home page começando a ganhar vida.

> #### Resultado
> [http://codepen.io/jlcarvalho/pen/ktomh](http://codepen.io/jlcarvalho/pen/ktomh)

<br>

> #### Codificação de caracteres especiais
> O elemento `<h3>` dentro do nosso elemento `<header>`, bem como o elemento `<small>`dentro do nosso elemento `<footer>`, tem algumas coisas interessantes acontecendo. Especificamente, alguns caracteres especiais dentro desses elementos estão sendo codificados.

> Caracteres especiais incluem vários sinais de pontuação, letras acentuadas e símbolos. Quando digitado diretamente no HTML, eles podem ser mal interpretados ou confundidos com o caracteres errados. Portanto, eles precisam de ser codificados.

> Cada caracter codificado vai começar com um “e” comercial, `&` , e terminam com um ponto e vírgula, `;` . O que fica entre o “e” comercial e o ponto e vírgula é a codificação única de um caracter, seja ele um nome ou codificação numérica.

> Por exemplo, poderíamos codificar a palavra `currículo`, como `curr&iacute;culo`. Dentro da nosso conteúdo temos algumas ocorrências de caracteres especiais, por exemplo dentro de nosso rodapé temos codificado o símbolo de copyright.

> Que tal revisar nosso código e substituir os caracteres especiais pelas suas respectivas codificações? Para referência, uma longa lista de codificações de caracteres pode ser encontrada em [Copy Paste Character](http://copypastecharacter.com/).

Com a nossa página inicial tomando forma, vamos dar uma olhada em como criar hiperlinks para que possamos adicionar páginas adicionais e construir o resto do nosso site.



