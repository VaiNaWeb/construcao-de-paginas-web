- Selecionamos o que queremos estilizar, e então algum seletor CSS define como, onde, e até quando colocar esses estilos.

- Podemos adicionar a CSS em nossa página HTML de três formas:

- Adicionadno o CSS em linha usando o atributo style

```html
<p style="color: #f05a20;">Vai na Web</p>
```

- Adicionando CSS direto no `<head>`

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

- Adicionando css externamente: criamos um arquivo chamado estilos.css, e o chamamos no `<head>` do html. Ah! chamamos nosso arquivo de estilos.css, mas você pode criar um arquivo com o nome que quiser e chamo-lo ai, lembre-se de colocar junto ao nome do arquivo a extensão dele, ou seja .css no final.

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

- Sintaxe: A estrutura como ela é escrita.

```css
seletor {
	propriedade: valor;
}

```

Leia mais!<br>
https://code.tutsplus.com/pt/tutorials/the-30-css-selectors-you-must-memorize--net-16048
https://developer.mozilla.org/pt-BR/docs/Web/HTML/HTML5/HTML5_element_list