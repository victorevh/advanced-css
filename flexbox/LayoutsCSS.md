# Layouts e evolução

Layout tem a ver com a maneira que os elementos estão distribuidos na tela

## Normal flow

Ou Flow Layout é a maneira que os elementos `block` e `inline` ficam na página

~~~html
<p> Texto block com <strong>inline</strong> dentro </p>
~~~

## Tables

É a maneira de tabelas onde a tag `table` recebe um display `table` fazendo com que os elementos internos como `td` e `tr` possam ser usados para montar uma tabela

~~~html
<table>
    <tr>
        <td> Hora </td>
        <td> 20:00 </td>
    </tr>
    <tr>
        <td> Hora </td>
        <td> 20:37 </td>
    </tr>
</table>
~~~

## Tabless

Uso das propriedades `float`, `clean` para que os elemnentos possam mudar de posição na tela.