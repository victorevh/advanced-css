# Combinators

Combinadores, pois eles trabalham para buscar e combinar seletores a fim de aplicar uma estilização

## Descendant combinator

* Identificando por um espaço entre os seletores.
* Busca um elemento dentro de outro

## HTML
~~~html
<body>
    <article>
        <h2>Um título</h2>
    </article>
</body>
~~~
## CSS
~~~css
body article h2 {
    color: red;
}
~~~~