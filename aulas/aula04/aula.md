#Evoluindo minha página com mais HTML

##Conectando páginas

Sabemos que nossos sites são um conjunto de páginas conectadas, ou linkadas, umas às outras. Agora vamos compreender melhor como isso acontece. Quando vamos construir um site, precisamos organizar bem nossos arquivos; vamos fazer isso através de pastas.

##Criando links

Na internet, temos várias e várias páginas conectadas umas às outras. A criação do hiperlink foi uma das responsáveis por tornar a web tão maravilhosa como ela é. Foi assim que conseguimos começar a facilmente conectar páginas. 

Criar links em nossa página pode ser muito útil, vamos agora aprender a criá-los. Qualquer elemento que aparece entre a abertura e o fechamento de tags <a> é a parte que será um link clicável na página. Exemplo:

```html
<p>Esse é um exemplo de palavra <a href="http://www.vainaweb.com.br"> clicável </a>.</p>
```

Qualquer coisa mesmo, não somente textos. Nós podemos deixar imagens clicáveis também!

```html
<a href="http://www.vainaweb.com.br">
    <img src="http://www.vainaweb.com.br/img/vainaweb.svg" alt="logo">
</a>
```

##Listando coisas

Existem três tipos de listas: as ordenadas, as não ordenadas e as de definições.

###Ordenadas

Assim como o nome parece sugerir, são listas em que a ordem dos itens importa, e eles podem ser enumerados.

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

###Não ordenadas

Nesta, os itens não são enumerados e podem estar acompanhados apenas de um símbolo.

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

###De definição

Neste tipo de lista, os itens são definidos.

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

##Criando tabelas

Criamos uma tabela com a tag `<table>` uma linha de Table Row, ou `<tr>`. Cada célula de dados será uma Table Data, ou `<td>` podemos, se nececessário, adicionar o atributo rowspan, que vai criar uma expansão de linha nas células. Podemos também usar o atributo colspan e teremos uma expansão de coluna nas células.

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
