## Identificando divs e spans

Divisões, ou `<div>`, e `<span>` são elementos HTML que atuam como contêineres apenas para fins de estilo. Como recipientes genéricos, eles não vêm com qualquer significado global ou valor semântico. O conteúdo contido dentro de um elemento `<p>` é conhecido e compreendido como um parágrafo. `<div>` e `<span>` não possuem qualquer significado e são simplesmente contêineres.

> #### Elementos Bloco x Elementos em linha
> A maioria dos elementos são ou elementos em linha ou de bloco. Qual é a diferença?
Elementos bloco ocupam todo o espaço horizontal disponível e iniciam uma nova linha no documento. Novos elementos irão começar na próxima linha livre. Elementos bloco podem ser aninhados um dentro do outro e podem envolver elementos inline. Vamos ver mais comumente elementos bloco utilizados para grandes pedaços de conteúdo, tais como parágrafos.

> Elementos em linha, ou inline, ocupam apenas o espaço necessário e não iniciam uma nova linha. São chamados elementos em linha justamente por aparecer na mesma linha que outros elementos, caso seja possível. Elementos em linha podem ser aninhados um dentro do outro, no entanto, eles não podem envolver elementos bloco. Nós geralmente veremos elementos em linha com pequenos pedaços de conteúdo, como algumas palavras.

Ambos, `<div>` e `<span>`, no entanto, são extremamente úteis na construção de um site, pois eles nos dão a capacidade de aplicar estilos direcionados a uma parte do conteúdo.

A `<div>` é um elemento bloco que é comumente usado para identificar grandes grupos de conteúdo, e que ajuda a construir o layout e o design de uma página web. O `<span>`, por outro lado, é um elemento em linha comumente usado para identificar grupos menores de texto dentro de um elemento bloco.

Nós comumente veremos `<div>` e `<span>` com os atributos class ou id para fins de estilo. Escolher entre o valor do atributo class, id ou nome requer um certo cuidado. Pois queremos escolher um valor que se refira ao conteúdo de um elemento, e não necessariamente a aparência do mesmo.

Por exemplo, se temos uma `<div>` com um fundo laranja que contém links de mídias sociais, o nosso primeiro pensamento pode ser dar ao `<div>` uma classe com o valor de laranja. O que acontece se futuramente esse fundo laranja mudar para azul? Possuir a classe laranja não faz mais sentido. Uma escolha mais sensível para a classe seria “social”, pois se refere ao conteúdo da `<div>`, não o estilo.

```html
<!-- Divisão -->
<div class="social">
  <p>Posso ser encontrado em ...</p>
  <p>Além disso, eu tenho um perfil no ...</p>
</div>

<!-- Span -->
<p>Logo estaremos <span class="tooltip">escrevendo HTML</span> com o melhor deles </p>
```

> #### Comentários em HTML e CSS
> O código anterior inclui pontos de exclamação dentro do HTML, e continua correto. Aqueles que não são elementos, são comentários.

> HTML e CSS nos dão a possibilidade de deixar comentários no nosso código e qualquer conteúdo embrulhado dentro de um comentário não será exibido na página web. Comentários ajudam a manter nossos arquivos organizados, nos permitem definir lembretes, e fornecem uma maneira de gerir de forma mais eficaz o nosso código. Comentários tornam-se especialmente úteis quando existem várias pessoas trabalhando nos mesmos arquivos.

> Comentários HTML começam com `<!--` e terminam com `-->`. Comentários CSS começam com `/*` e terminam com `*/`.



