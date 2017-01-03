#Conhecendo os poderes da CSS

A CSS tem o poder de deixar as páginas em HTML cheias de estilo. Funciona exatamente assim:
Selecionamos o que queremos estilizar, e então a CSS define como, onde, e até quando colocar esses estilos. 

##Adicionando ao documento

Lembre-se! A CSS não trabalha sozinha, ela precisa ser adicionada ao HTML. Podemos adicionar a CSS em nossa página HTML de três formas:

###Em linha usando o atributo style

```html
<p style="color: #ccc;">Vai na Web</p>
```

###Direto no `<head>`

```html
<head>
	<style>
		p { color: #ccc; }
	</style>
</head>
<body>
	<p>Vai na Web</p>
</body>
```

###Externamente

```html
<head>
	<title>Vai na Web</title>
	<link rel="stylesheet" href="styles.css" />
</head>
```

##Principais seletores

