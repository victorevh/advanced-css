## `box-sizing`

Como será calculado o tamanho total da caixa?

- content-box | border-box
  
~~~css
div {
    box-sizing: border-box;
}
~~~

* Observe que sem o `box-sizing: border-box;` essa div ocuparia um total de 140px de largura da tela, pois 100px de largura + 20px a mais em cara lateral somaria os 140px. 

~~~css
div {
  width: 100px;
  height: 100px;
  border: 1px solid red;
  margin: 10%;
  padding: 0 20px;
  
  box-sizing: border-box
}
~~~

* Quando utilizamos o `box-sizing: border-box;` o limite maximo da `div` é definida atraves do `width` e `height` que é de 100px, mesmo com os pixels adicionais do `padding`

* O mais indicado é redefinir todo o conteúdo com o seletor global

~~~css
*{
    box-sizing: border-box;
}
~~~