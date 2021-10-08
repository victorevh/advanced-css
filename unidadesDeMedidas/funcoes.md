# Funções

Em programação, funções são reconhecidas por causar um reaproveitamento de código.

* rgb()
* hsl()
* url()
* calc()

## Exemplo de aplicação

### HTML
~~~html
<div class="box"></div>
~~~
### CSS
~~~CSS
body{
    height: 100vh;
    margin: 0;
}
.box {
    height: calc(100% - 40px);
    width: 400px;
    background-image: url(http://source.unsplash.com/random);
    background-repeat: no-repeat;
    background-position: bottom right;
}
~~~