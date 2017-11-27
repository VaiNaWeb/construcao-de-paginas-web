# Introdução CSS

Vamos descobrir como deixar as páginas cheias de estilo usando CSS e seus poderes. Funciona exatamente assim: selecionamos o que queremos estilizar e, então, algum seletor CSS define como, onde e até quando colocar esses estilos.

## Adicionando ao documento

Podemos adicionar a CSS em nossa página HTML de três formas:

### Em linha, usando o atributo style

```html
<p style="color: #f05a20;">Vai na Web</p>
```

### Direto no `<head>`

```html
<head>
	<style>
		p { color: #f05a20; }
	</style>
</head>
<body>
	<p>Vai na Web</p>
</body>
```

### Externamente

Dessa forma, criamos um arquivo chamado estilos.css, e o aplicamos no `<head>` do html. Ah! chamamos nosso arquivo de estilos.css, mas você pode criar um arquivo com o nome que quiser e utilizá-lo. Lembre-se de colocar junto ao nome do arquivo a extensão dele, ou seja, .css, no final.

```html
<head>
	<title>Vai na Web</title>
	<link rel="stylesheet" href="estilos.css" />
</head>
<body>
    <p>Vai na Web</p>
</body>
```

```css
p {
	color: #f05a20;
}
```

## Sintaxe

Precisamos compreender a sintaxe que a linguagem usa. Pensar na sintaxe de uma linguagem significa pensar nas relações formais que unem as partes constituintes da sentença, criando uma estrutura. Ou seja, trata-se de pensar na estrutura através da qual ela é escrita.

```css
seletor {
	propriedade: valor;
}
```

Assim podemos fazer com que nossa página fique muito legal. Podemos alterar as cores, tamanhos, formas e até adicionar animações! Nas próximas aulas, vamos conhecer melhor essas e outras propriedades e valores.

## Principais seletores

Precisamos dizer ao CSS qual elemento queremos selecionar e adicionar a ele os estilos que desejamos. Mas, para isso, devemos entender sobre os [seletores](https://code.tutsplus.com/pt/tutorials/the-30-css-selectors-you-must-memorize--net-16048).

### Elemento

Podemos dar estilo diretamente ao próprio elemento do HTML.

```css
p {
	color: #f05a20;
}
```

### Id 

Ou podemos adicionar um ID ao elemento. É legal de ser usado em elementos que não se repetem na página.

```css
#sobre {
	color: #f05a20;
}
```

### Classe

Podemos, ainda, adicionar uma classe ao elemento. Muito útil para as que se repetem ao longo da página.

```css
.sobre {
	color: #f05a20;
}
```
# Modelo de caixa com CSS

Continuando as analogias sobre nossos elementos serem caixas, agora imaginem que eles são realmente caixinhas retangulares. Como se em cada um deles houvesse um retângulo invisível.

Em nossas páginas, nós podemos determinar o tamanho, a altura, o preenchimento, o espaçamento, e até as cores dessas caixas. Assim criamos interessantes e belíssimas composições visuais para sites.

Cada caixa tem uma largura e uma altura, que determinamos usando as propriedades <code>width</code> e <code>height</code>.

```css
.elemento {
    width: 100px;
    height: 100px;
}
```
Além de <code>width</code> e <code>height</code> temos também o <code>padding</code> e o <code>margin</code>. <code>Padding</code> pode aumentar o preenchimento de uma caixa, enquanto <code>margin</code> pode aumentar seu espaçamento.

```css
.elemento {
    width: 100px;
    height: 100px;
    padding: 50px;
    margin: 50px;
}
```
Temos também a propriedade <code>border</code>, que pode servir para aplicar estilo às bordas de uma caixa.
```css
.elemento {
    width: 100px;
    height: 100px;
    padding: 50px;
    margin: 50px;
    border-width: 5px;
    border-style: solid;
    border-color: black;
}
```
## Comportamento de bloco

Há caixas que se comportam em forma de bloco e há caixas que se comportam em forma de linha. Cada elemento já tem esse comportamento definido por padrão, mas podemos alterá-lo também. Basta alterar os valores da propriedade display com <code>inline</code>, ou <code>block</code>.

Elementos que se comportam como bloco, como <code>h1</code>, <code>h2</code>, <code>h3</code>, <code>p</code>, <code>ul</code>, <code>li</code>, ocupam toda a largura de uma página. Assim sendo, se duas caixas que se comportam como bloco forem adicionadas, a primeira vai querer ocupar toda a largura, então a outra aparecerá abaixo dela, ocupando também toda a largura da página.
```css
p {
    display: block;
}
```
Alguns exemplos de elementos que se comportam em forma de linha são a, <code>img</code>, <code>input</code>, <code>label</code>. Eles não tentam ocupar uma largura que não precisam, dessa forma conseguem ser alinhados visualmente em uma única linha.
```css
a {
    display: inline;
}
```
Testem, testem e testem! Explorem sem medo todas as propriedades e valores que foram vistos hoje. Aproveitem todas as possibilidades que eles podem criar. Na dúvida, sintam-se à vontade para usar o inspetor do navegador e ter uma melhor visualização do comportamento dos seus estilos.
