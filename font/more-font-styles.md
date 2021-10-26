# Atribuindo mais estilos para as fontes

<button style="background-color: black; color: white;"><a style="color: white;" href="https://developer.mozilla.org/en-US/docs/Learn/CSS/Styling_text/Fundamentals">Docs: Developer Mozilla</a></button>

## `font-variant`

* variações na apresentação da fonte

~~~css
p {
    font-variant: small-caps;
}
~~~

<button style="background-color: black; color: white;"><a style="color: white;" href="https://developer.mozilla.org/en-US/docs/Web/CSS/font-variant">Docs: font-variant</a></button>

## `font-stretch`

* alargamento ou encolhimento da fonte
* aceita palavra-chaves como: `expanded`, `condensed`, `normal`
* aceita porcentagens de 50% a 200%

~~~css
P {
    font-stretch: expanded;
}
~~~

<button style="background-color: black; color: white;"><a style="color: white;" href="https://developer.mozilla.org/en-US/docs/Web/CSS/font-stretch">Docs: font-stretch</a></button>

## `letter-spacing`

* Espaços entre caracteres

~~~css
p {
    letter-spacing: 4px;
}
~~~

<button style="background-color: black; color: white;"><a style="color: white;" href="https://developer.mozilla.org/en-US/docs/Web/CSS/letter-spacing">Docs: letter-spacing</a></button>

## `word-spacing`

* Espaço entre as palavras

~~~css
p {
    word-spacing: 4px;
}
~~~~
<button style="background-color: black; color: white;"><a style="color: white;" href="https://developer.mozilla.org/en-US/docs/Web/CSS/word-spacing">Docs: word-spacing</a></button>

## `line-height`

* Espaços entre linhas
* Pode ser com unidades ou sem unidades de medida
* Comuns: 1.5 ou 2

~~~css
p {
    line-height: 1.6;
}
~~~

<button style="background-color: black; color: white;"><a style="color: white;" href="https://developer.mozilla.org/en-US/docs/Web/CSS/line-height">Docs: line-height</a></button>

## `text-transform`

* Transformação do texto

~~~css
p {
    text-transform: uppercase; /* capitalize | lowercase | none */
}
~~~

<button style="background-color: black; color: white;"><a style="color: white;" href="https://developer.mozilla.org/en-US/docs/Web/CSS/text-transform">Docs: text-transform</a></button>

## `text-decoration`

* Aparencia decorativa de um texto
* line: underline | overline | line-through
  * podemos aplicar mais de 1 valor
* style: wavy | dotted | double | dashed | solid
* color: `<color>` values

~~~css
p {
    text-decoration: underline wavy red; /* shorthand */
}
~~~

<button style="background-color: black; color: white;"><a style="color: white;" href="https://developer.mozilla.org/en-US/docs/Web/CSS/text-decoration">Docs: text-decoration</a></button>

## `text-align`

* Alinhamento de um texto

~~~css
p {
    text-align: center; /* left | right | center | justify */
}
~~~

<button style="background-color: black; color: white;"><a style="color: white;" href="https://developer.mozilla.org/en-US/docs/Web/CSS/text-align">Docs: text-align</a></button>

## `text-shadow`

* Sompra aplicada a um texto
* Permite múltiplos valores

~~~css
p {
    text-shadow: 1px 1px 1px red,
                2px 2px 1px green; /* offset-x | offset-y | blur-radius | color */
}
~~~

<button style="background-color: black; color: white;"><a style="color: white;" href="https://developer.mozilla.org/en-US/docs/Web/CSS/text-shadow">Docs: text-shadow</a></button>

## `Shorthand`

* `font-style`, `font-variant`, `font-weight`, `font-stretch`, `font-size`, `line-height`, e `font-family`.

~~~css
p {
    /* -style, - variant, -weight, -stretch, -size, line-height, e -family. */
    font: italic normal bold normal 3em/1.5 Helvetica, Arial, sans-serif;
}
~~~~