# Descobrindo o poder dos estilos com CSS

Vamos descobrir como deixar as páginas em HTML cheias de estilo usando CSS e seus poderes. Funciona exatamente assim: selecionamos o que queremos estilizar e, então, algum seletor CSS define como, onde e até quando colocar esses estilos.

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

## As cores na web

Aprenderemos como colocar cores na web. Há alguns [sistemas de cores](https://tableless.com.br/sobre-cor-e-webdesign/) que precisamos conhecer para entender como adiciona-las em nossas folhas de estilo.

## RGB

Monitores são pretos e iluminados por vários pontinhos de luz. Vamos somando pontinhos vermelhos, verdes, e azuis até chegar na cor.

É formada por três pares de números, formados por três dígitos. Quanto mais alto o número mais clara é a cor. Em CSS, um quarto número representa o canal alpha.

```css
p {
    color: rgb(0, 0, 255, 0.5);
}
```

## Hexadecimais

Compostos por uma combinação de três conjuntos de pares formados a partir de número e letras de A a F. Quanto mais alto o número mais clara é a cor.

Cada par é responsável por uma cor, assim como o RGB, Vermelho, verde e azul. Ou seja #ff0000 é o vermelho, e o #00ff00 é o verde e #0000ff é o azul.

```css
p {
    color: #ff0000;
}
```
## Ferramentas legais

http://lokeshdhakar.com/projects/color-thief/<br>
http://moviesincolor.com/<br>
https://color.adobe.com/pt/create/color-wheel/<br>
https://www.w3schools.com/colors/colors_picker.asp?colorhex=F0F8FF<br>

Essa foi apenas uma introdução sobre como adicionamos os estilos. Vamos conhecer novas propriedades nas próximas aulas e entender como elas funcionam, até lá, não deixem de praticar.