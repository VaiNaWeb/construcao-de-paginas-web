# Como páginas da Web são construídas

* Cada tag funciona como uma etiqueta, que diz ao navegador qual elemento está escrito ali e como ele deve interpretar.

* A tag <html> indica que dentro dela haverá elementos em html, dentro dela temos <head> que significa cabeçalho e <body> que significa corpo.

* Uma tag começa com o sinal de menor ("<") e termina com o sinal de maior (">"). Há algumas raras exceções.

* Como se guardássemos uma caixa dentro de outra caixa, e dentro dela colocássemos outra caixa e outra caixa... Assim, criamos elementos dentro de elementos, e, para não confundir o navegador, aninhamos nossos elementos.

* Exemplo de estrutura básica em html:

```html
<!DOCTYPE html>
<html>

	<head>
		<title> </title>
	</head>

	<body>

		<p>Olá mundo!</p>
		
	</body>

</html>
```

## Tags do html5

`<section>` Define uma seção<br>
`<nav>` Define um menu com links de navegação<br>
`<article>` Pode definir um artigo, um comentário enviado pelo usuário, etc<br>
`<aside>` Define um conteúdo reservado dentro página.<br>
`<header>` Define o cabeçalho de uma página ou seção.<br>
`<footer>` Define o rodapé de uma página ou seção. <br>
`<main>` Define o conteúdo principal ou importante no documento. Deve existir apenas um.<br>

## Títulos

```html
<h1>Eu sou o título mais importante!</h1>
<h2>Eu sou um pouco menos importante</h2>
<h3>Eu sou um pouco menos importante</h3>
<h4>Eu sou um pouco menos importante</h4>
<h5>Eu sou um pouco menos importante</h5>
<h6>Eu sou o menos importante</h6>
```

Um elemento `<img>` sempre terá um atributo src e um alt. Ah! Um elemento `<img>` é um daqueles elementos especiais que não precisam de tag de fechamento, ela já se auto fecha.

Exemplo:

```html
<img src="http://www.vainaweb.com.br/img/vainaweb.svg" alt="logo do vai na web"/>
```

Leia mais!<br>
https://developer.mozilla.org/pt-BR/docs/Aprender<br>
https://developer.mozilla.org/pt-BR/docs/Web/HTML/HTML5/HTML5_element_list<br>
http://jlcarvalho.github.io/guia-frontend/<br>
https://diveintohtml5.com.br/