# Posições 

`<position>`

Representa um conjunto de coordenadas 2D:
- top, right, bottom, left e center

* Usado para alguns tipos de propriedades
* Não confundir com a propriedade `position`

## Exemplo de aplicação

### HTML
~~~html
<div class="box"></div>
~~~
### CSS
~~~CSS
.box {
    height: 300px;
    width: 300px;
    background-image: url(http://source.unsplash.com/random);
    background-repeat: no-repeat;
    background-position: bottom right;
}
~~~