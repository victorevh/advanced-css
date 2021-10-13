# Seletores

Conecta um elemento HTML com o CSS a fim de alterar o elemento.

## Tipos

* Element selector
    - Todos os elementos HTML

* ID Selector
    - Um elemento que tenha um atributo `id`.
    - Cada id deverá ser único.

* Class selector
    - Os elementos que contenha um atributo `class`.
    - Podemos ter uma ou mais classes.

* Attribute selector
    - Um elemento que tenha um atributo específico.

* Pseudo-class selector
    - Elementos em um estado específico

## Múltiplos

Você poderá selecionar múltiplos elementos e aplicar alguma regra CSS para todos eles.

Usamos uma separação por vírgulas para isso

## Element selector

### HTML
~~~HTML
<h1>Título da página</h1>
<p>Conteúdo da minha página</p>
~~~

### CSS
~~~ CSS
h1 {
  color: blue;
  font-size: 60px;
}

p {
  color: green
}
~~~

## ID Selector

### HTML
~~~HTML
<h1 id="title">Título da página</h1>
<p id="content">Conteúdo da minha página</p>
~~~

### CSS
~~~ CSS
#title {
  color: yellow;
  font-size: 60px;
}

#contenet {
  color: orange
}
~~~

## Class selector

### HTML
~~~HTML
<h1 id="title" class="red big">Título da página</h1>
<p id="content" class="red">Conteúdo da minha página</p>
~~~

### CSS
~~~ CSS

.red {
    color: red;
}

.big {
    font-size: 3em;
}
~~~

## Attribute selector

### HTML
~~~html
<h1 id="title" class="red big" title="Algum titulo">Título da página</h1>
<p id="content" class="red">Conteúdo da minha página</p>
~~~

### CSS
~~~ CSS
[title] {
  color: orange;
}
~~~

## Pseudo-class selector
### HTML
~~~html
<h1 id="title" class="red big" title="Algum titulo">Título da página</h1>
<p id="content" class="red">Conteúdo da minha página</p>
~~~

### CSS
~~~CSS
p:hover {
  color: red;
}

h1:hover {
  color: red;
}
~~~

## Múltiplos Seletores

### HTML
~~~html
<h1 id="title" class="red big" title="Algum titulo">Título da página</h1>
<p id="content" class="red">Conteúdo da minha página</p>
<strong class="red">AQUI</strong>
~~~

### CSS

~~~css
p, h1, .red {
  color: red;
}
~~~

