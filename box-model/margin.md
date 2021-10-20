## margin
Espaços entre os elementos

- `margin-top` | `margin-right` | `margin-bottom` | `margin-left`
- values: `<lenght>` | `<percentage>` | `auto`
  
~~~css
div{
    /* shorthand */
    margin: 12px 16px 10px 4px; /*top, right, bottom, e left*/
    margin: 12px 16px 0px; /*top, um valor para as laterais e bottom*/
    margin: 8px 16px; /*right e left*/
    margin: 8px; /*um valor para todos os lados*/
}
~~~
* o navegador tem 8px por padrão de margem, logo adicionamos ao seletor global a seguinte declaração zerando a margem
  
~~~css
* {
    margin: 0;
}
~~~
* Cuidado com margin collapsing (top se junta ao bottom)

* Utilizamos essa configuração para fixar o alinhamento do margin
css~~~
div {
    margin: 10px auto;
}
