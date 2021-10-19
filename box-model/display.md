## `display: block` vs `display: inline`

- Como as caixas se comportam em relação às outras caixas
- Comportamento externo das caixas
  
**block** | **inline**
----------|------------
Ocupa toda a linha, colocando o próximo elemento abaixo desse | Elemento ao lado do outro
`width` e `height` são respeitados | `width` e `height` não funcionam
`padding`, `margin`, `border` irão funcionar normalmente. | Somente valores horizontais de `margin`, `padding` e `border`

## A maioria dos conteúdos por padrão são block

Ex:.

block: `<p> <div> <section>`, todos os heading `<h1> <h2>....` <br>
inline: `<a>` `<strong>` `<span>` `<em>` 

### HTML
~~~html
<div>
  block
</div>
<span>
  inline
</span>
~~~

* Observe que a tag `<span>` tem seu comportamento por padrão `inline`, ignorando todas os valores de altura.

### CSS
~~~css
div {
  height: 100px;
  border: 1px solid red;
  width: 10px;
  display: inline;
}
span {
  height: 100px;
  border: 1px solid red;
  width: 10px;
  display: block;
}
~~~

* Quando utilizo o `display: block;` na classe de `span` eu inverto a lógica padrão, e ai sim as declarações de altura são respeitadas.

~~~css
div {
  margin: 30px;
}
span {
  margin: 30px;
}
~~~

* Observe que ao declarar a margin na `div` o elemento abre 30px de margin tanto para a altura quanto para as laterais pois o elemento por padrão é `display: block;`.
* O mesmo não acontece com a margin declarada no `span` pois como o elemento é `display: inline;` ele só abre margem para as laterais.