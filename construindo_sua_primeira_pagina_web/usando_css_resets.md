## Usando CSS Resets

Cada navegador tem seus próprios padrões de estilos para diferentes elementos. Como o Google Chrome exibe cabeçalhos, parágrafos, listas, e assim por diante pode ser diferente da forma como o Internet Explorer faz. Para garantir a compatibilidade cross-browser os CSS resets tornaram-se amplamente utilizados.

Os CSS Resets dá a cada elemento comum do HTML um estilo pré-definido e fornece um estilo unificado para todos os navegadores. Essas redefinições geralmente envolvem a remoção de qualquer dimensionamento, as margens, preenchimentos, ou estilos adicionais removendo os mesmos. Por causa do efeito cascata do CSS essas redefinições devem estar no topo da nossa folha de estilo. Isso garante que esses estilos são lidos em primeiro lugar e que todos os navegadores diferentes estarão trabalhando a partir de uma base comum.

Existem diversos CSS resets disponíveis para uso, todos os quais têm suas vantagens e desvantagens. Um dos mais populares é [CSS Reset deo Eric Meyer](http://meyerweb.com/eric/tools/css/reset/), que foi adaptado para incluir estilos para os novos elementos do HTML5.

Caso você queira uma outra opção existe também o Normalize.css, criado por Nicolas Gallagher. O [Normalize.css](http://necolas.github.io/normalize.css/) não se concentra em remover os estilos adicionais para todos os elementos comuns, mas em vez disso, definir estilos comuns para estes elementos. Ele exige uma maior compreensão do CSS, bem como a consciência do que você gostaria que seus estilos sejam.

> #### Compatibilidade Cross-Browser e testes
> Como mencionado anteriormente, diferentes navegadores tratam elementos de diferentes maneiras. É importante reconhecer o valor da compatibilidade e testes cross-browser. Websites não precisam exatamente da mesma aparência em todos os navegadores, mas eles devem estar, no mínimo, semelhantes. Quais são os navegadores que você deseja dar suporte, e em que grau, é uma decisão que você terá que fazer com base no que é melhor para o seu site.

São muitas coisas a serem estudadas para escrever CSS. A boa notícia é que tudo é possível, e com um pouco de paciência, vamos aprender tudo.
