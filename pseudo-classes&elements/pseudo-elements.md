# Pseudo-elements

Com pseudo-elements nós podemos adicionar elementos HTML pelo próprio CSS

## `::pseudo-element-name`

## Exemplos

* ::before
* ::after
* ::first-line

## `::before` & `::after`

* O conteúdo só é exibido se existir o `content:""`
### HTML
~~~html
<ul>
  <li>Gratidão</li>
  <li>Esperança</li>
  <li>Fé</li>
  <li>Gratidão</li>
  <li>Esperança</li>
  <li>Fé</li>
</ul>
~~~
### CSS
~~~css
li::before {
  content: ">"
}

li::after {
  content: "<"
}
~~~

## `::first-line`

* Pega primeira linha

### HTML
~~~html
<article>
  <h3>Gratidão</h3>
  <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Eaque tempore, impedit officia accusamus quam error quibusdam autem praesentium sed, vel atque, quas iure. Officiis, ut quibusdam aut incidunt itaque voluptas.</p>
  <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Eaque tempore, impedit officia accusamus quam error quibusdam autem praesentium sed, vel atque, quas iure. Officiis, ut quibusdam aut incidunt itaque voluptas.</p>
  <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Eaque tempore, impedit officia accusamus quam error quibusdam autem praesentium sed, vel atque, quas iure. Officiis, ut quibusdam aut incidunt itaque voluptas.</p>
  
</article>
~~~
### CSS
~~~css

p:nth-of-type(2)::first-line {
  font-weight: bold;
}
~~~~

## Referência

https://developer.mozilla.org/en-US/docs/web/CSS/Pseudo-classes
