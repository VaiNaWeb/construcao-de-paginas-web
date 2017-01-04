#Conhecendo CSS e seus poderes

CSS tem o poder de deixar as páginas em HTML cheias de estilo. Funciona exatamente assim:
selecionamos o que queremos estilizar, e então algum seletor CSS define como, onde, e até quando colocar esses estilos. 

##Adicionando ao documento

Lembre-se! A CSS não trabalha sozinha, ela precisa ser adicionada ao HTML. Podemos adicionar a CSS em nossa página HTML de três formas:

###Em linha usando o atributo style

```html
<p style="color: #f05a20;">Vai na Web</p>
```

###Direto no `<head>`

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

###Externamente

Dessa forma, criamos um arquivo chamado styles.css, e o chamamos no `<head>` do html.

```html
<head>
	<title>Vai na Web</title>
	<link rel="stylesheet" href="styles.css" />
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

##Principais seletores

Podemos dar estilo ao diretamente ao próprio elemento do HTML.

###Elemento
```css
p {
	color: #f05a20;
}
```

Ou podemos adicionar um ID ao elemento. É legal de ser usado em elementos que não se repetem.

###Id 
```css
#sobre {
	color: #f05a20;
}

```

Ou podemos ainda adicionar uma classe ao elemento. Muito útil em classes que se repetem ao longo dá página.

###Classe
```css
.sobre {
	color: #f05a20;
}
```