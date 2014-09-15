## Usando elementos de texto

Existem muitas formas diferentes de mídia e conteúdo on-line, no entanto, o texto é predominante. Assim, há uma série de elementos diferentes para a exibição de texto em uma página web. Por enquanto, vamos nos concentrar nos elementos mais populares, incluindo cabeçalhos, parágrafos, o texto em negrito para mostrar importância, e itálico para dar ênfase. Mais tarde, dentro do capítulo 6, "Trabalhando com Tipografia", vamos dar uma olhada em como estilizar o texto.

### Títulos

Os títulos são elementos bloco, e eles possuem seis níveis diferentes, do `<h1>` ao `<h6>`. Os títulos ajudam a quebrar rapidamente o conteúdo e estabelecer a hierarquia, e eles são identificadores chave para usuários que lêem uma página. Eles também ajudam os motores de busca a indexar e determinar o conteúdo em uma página.

Os títulos devem ser usados numa ordem que é relevante para o conteúdo de uma página. O título principal de uma página ou seção deve ser marcado com um elemento `<h1>`, e títulos subsequentes devem usar os elementos `<h2>`, `<h3>`, `<h4>`, `<h5>` e `<h6>` caso necessário.

Cada nível de título deve ser usado onde é semanticamente valorizado, e não deve ser usado para colocar o texto em negrito ou grande, pois existem outras maneiras melhores para fazer isso.

Aqui está um exemplo de HTML para todos os diferentes níveis de título e o resultando em uma página web.

```html
<h1> título de nível 1 </h1>
<h2> título de nível 2 </h2>
<h3> título de nível 3 </h3>
<h4> título de nível 4 </h4>
<h5> título de nível 5 </h5>
<h6> título de nível 6 </h6>
```

> #### Resultado
> [http://codepen.io/jlcarvalho/pen/BewLs](http://codepen.io/jlcarvalho/pen/BewLs)

### Parágrafos

Os títulos são muitas vezes seguidos por parágrafos. Parágrafos são definidos usando o elemento bloco `<p>`. Os parágrafos podem aparecer um após o outro. Aqui está um exemplo de como utilizar parágrafos.

```html
<p>Steve Jobs was a co-founder and longtime chief executive officer at Apple. On June 12, 2005, Steve gave the commencement address at Stanford University.</p>

<p>In his address Steve urged graduates to follow their dreams and, despite any setbacks, to never give up–advice which he sincerely took to heart.</p>
```

> #### Resultado
> [http://codepen.io/jlcarvalho/pen/aCqDG](http://codepen.io/jlcarvalho/pen/aCqDG)

### Texto em negrito com relevância

Para fazer com que o texto fique negrito e possua uma forte importância no contexto da página, vamos usar o elemento em linha `<strong>`. Há dois elementos que nos fornecem o texto em negrito: os elementos `<strong>` e `<b>`. É importante entender a diferença semântica entre os dois.

O elemento `<strong>` é semanticamente usado para dar grande importância ao texto, e é, portanto, a opção mais popular para o texto em negrito. O elemento `<b>`, por outro lado, significa semanticamente compensar texto estilisticamente, o que nem sempre é a melhor escolha para o texto que merece certa atenção a mais. Temos de avaliar o significado do texto que desejamos definir como destacado e escolher um elemento de acordo.

Aqui estão as duas opções de HTML para criar texto em negrito:

```html
<!-- Strong -->
<p><strong>Atenção:</strong> animais na pista.</p>

<!-- B -->
<p>Esta receita pede <b>bacon</b> e <b>batatas</b>.</p>
```

> #### Resultado
> [http://codepen.io/jlcarvalho/pen/srbEg](http://codepen.io/jlcarvalho/pen/srbEg)

### Texto em itálico com ênfase

Para colocar o texto em itálico, colocando assim ênfase sobre ele, vamos usar o elemento em linha `<em>`. Tal como acontece com os elementos de texto em negrito, há dois elementos diferentes que irão colocar o texto em itálico, cada um com um significado semântico diferente.

O elemento `<em>` é usado semanticamente para colocar uma ênfase no texto e é, assim, a opção mais popular para texto itálico. A outra opção, o elemento `<i>`, é usada semanticamente para transmitir texto em uma voz alternativa ou tom, quase como se tivesse sido colocado entre aspas. Mais uma vez, teremos de avaliar o significado do texto que queremos colocar em itálico e escolher um elemento de acordo.

Aqui está o código HTML para itálico:

```html
<!-- Ênfase -->
<p>Eu <em>amo</ em> Goiânia!</p>

<!-- Voz ou tom alternativo -->
<p>O nome <i>Shay</i> significa um dom.</p>
```

> #### Resultado
> [http://codepen.io/jlcarvalho/pen/kEvzC](http://codepen.io/jlcarvalho/pen/kEvzC)

Estes elementos em linha são bastante úteis para a construção de nosso conteúdo. Além destes, existem também elementos estruturais. Considerando os elementos baseados em texto identificamos cabeçalhos e parágrafos, elementos estruturais identificam agrupamentos de conteúdo, como cabeçalhos, rodapés, artigos, e assim por diante. Vamos dar uma olhada.
