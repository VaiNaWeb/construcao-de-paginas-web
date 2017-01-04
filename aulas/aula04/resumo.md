#Evoluindo minha página com mais HTML

- Sites são um conjunto de páginas conectadas, ou linkadas, umas às outras. Quando vamos construir um site, precisamos organizar bem nossos arquivos. Vamos fazer isso através de pastas.

- Na internet, temos várias e várias páginas conectadas umas às outras. A criação do hiperlink foi uma das responsáveis por tornar a web tão maravilhosa como ela é. Foi assim que conseguimos começar a facilmente conectar páginas. 

- Criar links em nossa página pode ser muito útil. Vamos agora aprender a criá-los. Qualquer coisa que aparece entre a abertura e fechamento de tags <a> é a parte que será um link clicável na página. Exemplos:

```html
<p>Esse é um exemplo de palavra <a href="http://www.vainaweb.com.br"> clicável </a>.</p>
```

```html
<a href="http://www.vainaweb.com.br">
    <img src="http://www.vainaweb.com.br/img/vainaweb.svg" alt="logo"/>
</a>
```

- Existem três tipos de listas: as ordenadas, as não ordenadas e as de definições.

- Listas ordenadas: assim como o nome parece sugerir, são listas nas quais a ordem dos itens importa, e eles podem ser enumerados.

```html
<ol>
    <li>Caneta</li>
    <li>Lápis</li>
    <li>Borracha</li>
    <li>Tesoura</li>
    <li>Papel</li>
</ol>
```

<ol>
    <li>Caneta</li>
    <li>Lápis</li>
    <li>Borracha</li>
    <li>Tesoura</li>
    <li>Papel</li>
</ol>

- Listas não ordenadas: nessas, os itens não são enumerados e podem estar acompanhados apenas de um símbolo.

```html
<ul>
    <li>Caneta</li>
    <li>Lápis</li>
    <li>Borracha</li>
    <li>Tesoura</li>
    <li>Papel</li>
</ul>
```
<ul>
    <li>Caneta</li>
    <li>Lápis</li>
    <li>Borracha</li>
    <li>Tesoura</li>
    <li>Papel</li>
</ul>

- Listas de definição: aqui os itens são definidos.

```html
<dl>
    <dt>Caneta</dt>
        <dd>Azul, com tinta</dd>
    <dt>Lápis</dt>
        <dd>De madeira</dd>
</dl>
```

<dl>
    <dt>Caneta</dt>
        <dd>Azul, com tinta</dd>
    <dt>Lápis</dt>
        <dd>De madeira</dd>
</dl>

- Criamos uma tabela com a tag `<table>`, uma linha de Table Row, ou `<tr>`. Cada célula de dados será uma Table Data, ou `<td> podemos, se nececessrio, adicionar o atributo rowspan, que vai criar uma expansão de linha nas células. Podemos também usar o atributo colspan e teremos uma expansão de coluna nas células.

```html
<table>
  <tr>
    <th>Nome</th>
    <th>Sobre</th>
  </tr>
  <tr>
    <td>Maria</td>
    <td>Gosta de cachorros</td>
  </tr>
  <tr>
    <td>Rosa</td>
    <td>Solta pipa com os irmãos</td>
  </tr>
</table>
```
<table>
  <tr>
    <th>Nome</th>
    <th>Sobre</th>
  </tr>
  <tr>
    <td>Maria</td>
    <td>Gosta de cachorros</td>
  </tr>
  <tr>
    <td>Rosa</td>
    <td>Solta pipa com os irmãos</td>
  </tr>
</table>
