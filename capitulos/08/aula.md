# HTML Semântico

Há elementos no HTML que conhecemos como elementos de caixa, ou containers. Usamos elas normalmente para agrupar nossos elementos. Houve uma época em que construíamos essas caixas simplesmente com uma tag chamada `<div>`, e ainda usamos ela eventualmente.

Com a chegada do HTML5, ganhamos algumas tags com significado semântico, e passamos a usar não somente `div`. Isso foi muito  importante para os navegadores e usuários, consequentemente isso facilitou também a nossa vida enquanto desenvolvedor. Agora temos uma tag `<header>` para cabeçalho, uma tag `<footer>` para rodapé e mais algumas:

`<section>` Define uma seção<br>
`<nav>` Define um menu com links de navegação<br>
`<article>` Pode definir um artigo, um comentário enviado pelo usuário etc<br>
`<aside>` Define um conteúdo reservado dentro página.<br>
`<header>` Define o cabeçalho de uma página ou seção.<br>
`<footer>` Define o rodapé de uma página ou seção. <br>
`<main>` Define o conteúdo principal ou importante no documento. Deve existir apenas um.<br>

![asset](01.png)

Existem seis níveis diferentes de títulos: `H1` é o mais importante,` h6` é o menos importante. Em HTML, o texto para cabeçalhos é escrito dentro dos elementos de título: `<h1>`, `<h2>`, `<h3>`, `<h4>`, `<h5>` ou `<h6>`.

Exemplo:

```html
<h1>Eu sou o título mais importante!</h1>
<h2>Eu sou um pouco menos importante</h2>
<h3>Eu sou um pouco menos importante</h3>
<h4>Eu sou um pouco menos importante</h4>
<h5>Eu sou um pouco menos importante</h5>
<h6>Eu sou o menos importante</h6>
```

<h1>Eu sou o título mais importante!</h1>
<h2>Eu sou um pouco menos importante</h2>
<h3>Eu sou um pouco menos importante</h3>
<h4>Eu sou um pouco menos importante</h4>
<h5>Eu sou um pouco menos importante</h5>
<h6>Eu sou o menos importante</h6>

# Evoluindo minha página com mais HTML

## Conectando páginas

Sabemos que nossos sites são um conjunto de páginas conectadas, ou linkadas, umas às outras. Agora vamos compreender melhor como isso acontece. Quando vamos construir um site, precisamos organizar bem nossos arquivos; vamos fazer isso através de pastas.

## Criando links

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

## Listando coisas

Existem três tipos de listas: as ordenadas, as não ordenadas e as de definições.

### Ordenadas

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

### Não ordenadas

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

### De definição

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

## Criando tabelas

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
  <tr>
    <td>João</td>
    <td>Adora gatos</td>
  </tr>
  <tr>
    <td>Ana</td>
    <td>Gosta de árvores</td>
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
  <tr>
    <td>João</td>
    <td>Adora gatos</td>
  </tr>
  <tr>
    <td>Ana</td>
    <td>Gosta de árvores</td>
  </tr>    
</table>
