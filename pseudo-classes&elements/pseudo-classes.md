# Pseudo-classes

É um tipo de seletor que irá selecionar um elemento que estiver em um estado específico.

Exemplo: É o primeiro elemento dentro de uma caixa, ou, o elemento está com o ponteiro do mouse em cima dele.

Pseudo-classes começam com 2 pontos seguido do nome da pseudo class `:pseudo-class-name`

## Selecionando elementos com pseudo-classes

* :first-child
* :nth-of-type()
* :nth-child()
  
## `:first-child`
### HTML
~~~html
<ul>
  <li>Gratidão</li>
  <li>Esperança</li>
  <li>Fé</li>
</ul>
~~~

### CSS

~~~css
ul li:first-child {
  font-weight: bold;
  color: red;
}
~~~

## `:nth-of-type()`

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
article p:nth-of-type(2) {
  font-weight: bold;
  font-size: 18px;
}
~~~~

## `:nth-child`

### Nesse caso ele só seleciona o segundo elemento `<p>` filho de `<article>`

## CSS
~~~css
article p:nth-child(2) {
  font-weight: bold;
  font-size: 18px;
}
~~~

## `:nth-child()`  (odd e even)
### Filho sim filho não (impar ou par)

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
~~~CSS
ul li:nth-child(even) {
  color: gray;
  background: blue;
}
~~~
## Ações do usuário

* :hover
* :focus

### HTML
~~~html
<a href="#">Clique aqui</a>
<input type="text">
~~~

### CSS
~~~css
a:hover {
  color: red;
}

input:focus {
  border-color: blue;
  outline: ;
}
~~~

## Atributos

* :disabled
* :required

### HTML
~~~html
<a href="#">Clique aqui</a>
<input type="text" disabled>
~~~

### CSS
~~~css
input:disabled {
  background-color: red;
}

## Referência

https://developer.mozilla.org/en-US/docs/web/CSS/Pseudo-classes

