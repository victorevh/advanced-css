# Combinators

Combinadores, pois eles trabalham para buscar e combinar seletores a fim de aplicar uma estilização

## Descendant combinator

* Identificando por um espaço entre os seletores.
* Busca um elemento dentro de outro

### HTML
~~~html
<body>
    <article>
        <h2>Um título</h2>
    </article>
</body>
~~~
### CSS
~~~css
body article h2 {
    color: red;
}
~~~~

## Child combinator

* Identificado pelo sinal `>` entre dois seletores
* Seleciona somente o elemento que é filho direto do pai
* Elementos depois do filho direto serão desconsiderados 

### HTML

~~~html
<body>
  <div>
    <p>exemplo</p>
      <ul>
    <li>Item 1</li>
  </ul>
  <ul>
      <li>Item 2</li>
  </ul>
  </div>
</body>
~~~
### CSS

~~~css
body > div > ul {
  color: blue;
}
~~~

## Adjacent sibling combinator

* Identificado pelo sinal `+` entre dois seletores
* Seleciona somente o elemento do lado direito que é irmão direto na hierarquia
  
### HTML
~~~html
<h1>
  Título
</h1>

<p>
  Esse é um paragrafo
</p>

<p>
  Esse é mais um paragrafo
</p>

<button> Um botão </button>
<button> Outro Click </button>
~~~

### CSS
~~~css
h1 + p {
  color: red;
}

button + button {
  margin-left: 15px;
  color: red
}
~~~

## General sibling combinator

* Identificado pelo sinal ` ~ ` entre dois seletores
* Seleciona todos os elementos irmãos
  
### HTML
~~~html
<h1>
  Título
</h1>

<p>
  Esse é um paragrafo
</p>

<button> Um botão </button>
<button> Outro Click </button>

<p>
  Esse é mais um paragrafo
</p>
~~~

### CSS
~~~css
h1 ~ p {
    color: red;
}
~~~

## Utilizando combinadores

### HTML
~~~HTML
<ul>
  <li> Aloooo </li>
  <li class="red">Hey</li>
</ul>
~~~
### CSS
~~~css
ul > li[class="red"] {
  color: red;
}
~~~

## Dica

* Seletores muito específicos tendem a causar dificuldades no reuso das regras de estilização dos elementos
* Muitas vezes, um simple uso de classes, torna o trabalho muito mais eficiente.    