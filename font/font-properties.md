# Trabalhando com fontes

Tipografia transmite uma mensagem

    - negrito
    - tamanho
    - estilo

## Basic Font Properties

* `font-family`
* `font-weight`
* `font-style`
* `font-size`

## Font Family

* Tipo de fonte de um elemento
* Lista de fontes e ordem de prioridade
* Inclui *fallback* font

~~~css
p {
    font-family: "Times New Roman", times, serif; /*fallback*/
}
~~~

* uma fonte `serif` tem dobras pequenas
* uma fonte `sans-serif` não tem essas dobras

## Font Weight

* Peso da fonte
* A diversidade de pesos vai depender da fonte escolhida
~~~css
p {
    font-weight: bold;
}
~~~

## Font Style

* Estilo da Fonte
  * normal
  * italic
  * oblique

* A diversidade de pesos vai depender da fonte escolhida
~~~css
p {
    font-style: italic
}
~~~

## Font Size

* O tamanho da fonte

~~~css
p {
    font-size: 18px;
}
~~~

## Web Fonts

- fontes do sistema x fontes da web
- como usar fontes para web?

    * @font-face
    * @import
    * link

### Referências

<button><a href="https://www.w3.org/TR/css-fonts-3/">W3</a></button> <br>
<button><a href="https://css-tricks.com/snippets/css/using-font-face/">CSS TRICKS</a></button>