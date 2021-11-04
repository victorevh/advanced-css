## Background

- Define um fundo para o nosso elemento
- Sua área de atuação é a caixa toda
- Por padrão, é transparente

### Exemplos

- Usar cores sólidas
- Usar imagens
- Controlar
    - a posição das imagens,
    - se elas se repetem ou não
    - o tamanho delas na caixa
- Usar cor e imagens juntas
- Usar gradiente

## `background-color`

* Cor de fundo de um elemento

### Exemplo

~~~css
div {
    height: 100px;
    border: 7px dashed red;

    background-color: rgb(55, 100, 50);

    /* Gradient */

    background: linear-gradient(270deg, red, yellow, green);  /* radial-gradient */
}
~~~

## `background-image`

* Fundo com imagem

## `background-repeat` 

* Repetir imagem de fundo
  * `no-repeat | repeat y | repeat x`

## `background-position`

* Posição da imagem
  * `left | center | right`
  * `top | bottom`

## `background-size`

* Tamanho da imagem de fundo
  * `contain | cover | % | px | em` 

## `background-origin` `background-clip`
  
* Origem do fundo
  * `border-box | content-box | padding-box`

## `background-attachment`

* Escolhe se o fundo vai permitir o scroll ou se vai ficar fixo
  * `fixed | scroll`
### Exemplos

~~~css
div {
    height: 100px;
    border: 7px dashed red;
    padding: 16px

    background-image: url(https://); 
    background-repeat: no-repeat;
    background-position: right bottom;
    background-size: 50% 50%; /* Altura vs largura */
    background-origin: content-box;
    background-clip: content-box;
    background-attachment: scroll;

    /* shorthand */

    background: rgb(55, 100, 50) url(https://)  no-repeat right top / 50px border-box content-box scroll;


}
~~~

## Múltiplos backgrounds

* Também é possivel utilizar múltiplos backgrounds

~~~css
main {
  background: radial-gradient(rgba(255,255,255,0), rgba(255,0,0, 0.2)), url(https://) no-repeat right top / 50px border-box content-box fixed;
}
~~~