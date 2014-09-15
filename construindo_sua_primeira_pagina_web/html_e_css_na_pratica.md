## HTML e CSS na Prática

Voltando ao site de nossa conferência, vamos adicionar um pouco mais de CSS.

1. Dentro da nossa pasta “Styles Conference”, vamos criar uma nova pasta chamada `assets`. Onde vamos guardar todos os arquivos estáticos do nosso site, tais como nossas folhas de estilo, imagens, vídeos, e assim por diante. Para as nossos folhas de estilo, vamos adicionar outra pasta chamada `stylesheets` dentro da pasta `assets`.
2. Usando o nosso editor de texto, vamos criar um novo arquivo chamado main.css e salvá-lo dentro da pasta `stylesheets` que acabamos de criar.
3. Ao abrir nosso arquivo index.html em um navegador web, podemos ver que os elementos `<h1>` e `<p>` possuem seus próprios estilos CSS padrão. Especificamente, cada um deles tem um tamanho de letra única e de espaçamento em torno deles. Usando o CSS Reset do Eric Meyer, podemos remover esses estilos, permitindo que cada um deles seja estilizado a partir da mesma base. Para fazer isso vá ao site do Eric, copie o CSS reset, e cole-o no topo de nosso arquivo `main.css`.
4. Com o nosso arquivo `main.css` começando a tomar forma, vamos ligá-lo ao nosso arquivo `index.html`. Abrindo o arquivo `index.html` em nosso editor de texto, vamos adicionar o elemento `<link>` dentro do nosso elemento `<head>`, logo após o elemento `<title>`.
5. Como vamos estar fazendo referência a uma folha de estilo dentro do elemento `<link>`, precisamos adicionar o atributo de relação, `rel`, com o valor `stylesheet`.
6. Nós também devemos incluir uma referência de hiperlink, usando o atributo `href`, ao nosso arquivo main.css. Lembre-se, nosso arquivo `main.css` é salvo na pasta `stylesheets`, que está dentro da pasta `assets`. Portanto, o valor do atributo `href` é o caminho para o nosso arquivo `main.css`, que é `assets/stylesheets/main.css`.

```html
<head>
  <meta charset="utf-8">
  <title> Styles Conference </title>
  <link rel="stylesheet" href="assets/stylesheets/main.css">
</head>
```

Hora de conferir nosso trabalho e ver se o nosso HTML e CSS estão se dando bem. Ao abrir o nosso arquivo `index.html` (ou atualizar a página, se ele já estiver aberto) dentro de um navegador veremos os resultados ligeiramente diferentes de antes.
