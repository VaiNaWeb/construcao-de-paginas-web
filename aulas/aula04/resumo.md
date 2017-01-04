#Evoluindo minha página com mais HTML

- Sites são um conjunto de páginas conectadas, ou linkadas, umas as outras. Quando vamos construir um site, precisamos organizar bem nossos arquivos, vamos fazer isso através de pastas.

- Na internet, temos várias e várias páginas conectadas umas as outras. A criação do hiperlink foi um dos responsáveis por tornar a web tão maravilhosa como ela é, foi assim que conseguimos começar a facilmente conectar páginas. 

- Criar links em nossa página, pode ser muito útil, vamos agora aprender a cria-los. Qualquer coisa que aparece entre a abertura e fechamento de tags <a> é a parte que será um link clicável na página. Exemplos:

```html
<p>Esse é um exemplo de palavra <a href="http://www.vainaweb.com.br"> clicável </a>.</p>
```

```html
<a href="http://www.vainaweb.com.br">
    <img src="http://www.vainaweb.com.br/img/vainaweb.svg" alt="logo"/>
</a>
```

- Existem três tipos de listas: as ordenadas, não ordenadas e de definições.

- Listas ordenadas: assim como o nome parece sugerir, são listas onde a ordem dos itens importam, e podem ser enumerados.

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

- Listas não ordenadas: nessa, os itens não são enumerados, e podem estar acompanhados apenas de um símbolo.

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

- Listas de definição: onde os itens são definidos.

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

- Criamos uma tabela com a tag `<table>` uma linha de Table Row, ou `<tr>`. Cada célula de dados será uma Table Data, ou `<td>` Podemos se nececessrio adicionar o atributo rowspan, que vai criar uma expansão de linha nas células. Podemos também usar o atributo colspan e teremos uma expansão de coluna nas células.

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

Leia mais!<br>
https://developer.mozilla.org/pt-BR/docs/Web/HTML/HTML5/HTML5_element_list