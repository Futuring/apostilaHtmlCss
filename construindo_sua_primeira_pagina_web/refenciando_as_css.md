## Refenciando as CSS

A fim de fazer nosso CSS falar com nosso HTML, precisamos referenciar o arquivo CSS dentro do HTML. A melhor prática para referenciar o nosso CSS é incluir todos os nossos estilos em uma única folha de estilo externa, que é referenciada dentro do elemento `<head>` do nosso documento HTML. Usar uma folha de estilo externa nos permite usar os mesmos estilos em diversas páginas web e rapidamente fazer alterações no site inteiro.

> #### Outras opções para adicionar CSS
> Outras opções para referenciar CSS incluem o uso de estilos internos e inline. Você pode encontrar estas opções por aí, mas são geralmente não recomendadas, pois elas dificultam a manutenção e atualização das páginas web.

Para criar a nossa folha de estilos CSS externa vamos precisar usar nosso editor de texto novamente para criar um novo arquivo de texto simples com a extensão de arquivo .css. Nosso arquivo CSS deve ser guardado dentro da mesma pasta, ou uma subpasta, onde o nosso arquivo HTML está localizado.

Dentro do elemento `<head>` do documento HTML, o elemento <link> é usado para definir a relação entre o arquivo HTML e o arquivo CSS. Por estarmos chamando um arquivo CSS, usamos o atributo rel com o valor stylesheet para especificar o relacionamento deles. Além disso, o atributo href (ou referência de hiperlink) é usado para identificar a localização, ou caminho, do arquivo CSS.

Considere o seguinte exemplo de um elemento `<head>` de um documento HTML que faz referência a uma única folha de estilo externa.

```html
<head>
  <link rel="stylesheet" href="main.css" >
</head>
```

Para que a CSS seja processado corretamente o caminho do valor do atributo href deve correlacionar diretamente onde o nosso arquivo CSS é salvo. No exemplo anterior, o arquivo main.css é armazenado no mesmo local que o arquivo HTML, também conhecido como o diretório raiz.

Se o nosso arquivo CSS está dentro de um subdiretório ou subpasta, o valor do atributo href deve correlacionar a este caminho corretamente. Por exemplo, se o nosso arquivo main.css foi armazenado dentro de um subdiretório chamado stylesheets, a valor do atributo href será stylesheets/main.css, usando uma barra para indicar que está acessando um subdiretório.

Neste ponto as nossas páginas estão começando a ganhar à vida, lenta mas seguramente. Nós não aprofundamos muito no CSS, mas você deve ter notado que alguns elementos têm estilos padrão sem que seja necessário declarar dentro do nosso CSS. Isso acontece pois o navegaodor impõe seus próprios estilos CSS preferenciais para esses elementos. Felizmente, podemos substituir esses estilos com bastante facilidade, que é o que vamos fazer a seguir usando CSS resets.
