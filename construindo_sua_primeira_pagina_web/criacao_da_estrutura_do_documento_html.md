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

> #### Resultado
> [http://codepen.io/jlcarvalho/pen/pDCbi](http://codepen.io/jlcarvalho/pen/pDCbi)

O código anterior mostra um documento começando com a declaração de tipo de documento `<!DOCTYPE html>`, seguido pelo elemento `<html>`. Dentro do elemento `<html>` vem os elementos `<head>` e `<body>`. O elemento `<head>` inclui a codificação de caracteres da página através da tag `<meta charset="utf-8">` e o título do documento através do elemento `<title>`. O elemento `<body>` inclui um título através do elemento `<h1>` e um parágrafo através do elemento `<p>`. Como tanto o título quanto o parágrafo são aninhados dentro do elemento `<body>`, eles são visíveis na página web.

Colocar um elemento é dentro de outro elemento é conhecido como aninhar elementos e é uma boa prática para manter a estrutura do documento bem organizado e legível. No código anterior, tanto os elementos `<head>` e `<body>` foram aninhados e indentandos dentro do elemento `<html>`. O padrão de indentação continua conforme novos elementos são adicionados dentro dos elementos `<head>` e `<body>`.

> #### Elementos de fechamento automático

> No exemplo anterior, o elemento `<meta>` tinha apenas uma tag e não incluía uma tag de fechamento. Pos nem todos os elementos possuem de abertura e fechamento. Alguns elementos podem simplesmente receber o seu conteúdo ou o comportamento de atributos dentro de uma única tag. O elemento `<meta>` é um desses elementos. O conteúdo do elemento `<meta>` anterior é atribuído com o uso do atributo charset e seu valor. Outros elementos de fechamento automático são: `<br>`, `<embed>`, `<hr>`, `<img>`, `<input>`, `<link>`, `<param>`, `<source>` e `<wbr>`.

> #### Validação de Código

> Não importa o quão cuidadoso nós somos, ao escrever o nosso código, inevitavelmente cometeremos erros. Felizmente, ao escrever HTML e CSS temos validadores para verificar o nosso trabalho. O W3C tem construído tanto validadores HTML e CSS que analisam o código em busca de erros. Validar nosso código não só ajuda a processar corretamente a página web em todos os navegadores, mas também nos ajuda a conhecer as melhores práticas recomendadas para escrever código.
