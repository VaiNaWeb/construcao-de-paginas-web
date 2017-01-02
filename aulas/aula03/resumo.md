##Como nos comunicamos através da Internet

* Quando dois computadores estão conectados à Internet eles podem conversar uns com os outros.

* O navegador pede os arquivos que contém os códigos do site - que estão armazenados no servidor - através do endereço. O servidor então envia os arquivos de volta para que o navegador possa interpretar seu código e exibir a página na tela.

* Um servidor é um computador especial que contém arquivos de páginas da web. Seu computador em casa ou na escola não é um servidor, porque ele não está conectado diretamente à Internet. Nós nos conectamos à Internet através de um Provedor de Serviços de Internet.

##Como páginas da Web são construídas

* A HTML é a linguagem base de uma página da Web. É ela quem cria a estrutura das nossas páginas, que podem conter textos, imagens, vídeos, e dar vida a tantos sites fantásticos que conhecemos hoje.

* Um documento em HTML é composto por uma estrutura formada por TAGS, que são marcações para identificar os diversos tipos de conteúdos e ainda organiza-los de forma semântica.

* Até então as páginas já tinham uma estrutura, e podiam ser acessadas, mas as pessoas começaram a pensar em como torna-las mais amigáveis e estéticamente bonitas, e isso era muito difícil de fazer somente com HTML. Algum tempo depois, nasceu a Folha de Estilos em Cascata, a CSS, que veio para deixar as nossas páginas literalmente cheias de estilo.

* Algum tempo depois foi criada a linguagem Javascript que serve para muitas coisas, como validar valores de um formulário para garantir que são aceitáveis antes de serem enviados ao servidor por exemplo, e coisas bem mais complexas.

* A HTML usa um conjunto pré-definido de elementos para identificar os diversos tipos de conteúdo. Os elementos, contém uma ou mais tags que contém ou expressam um determinado conteúdo.

* Cada tag funciona como uma etiqueta, que diz ao navegador qual elemento está escrito ali e como ele deve interpretar.

* A tag <html> indica que dentro dela haverá elementos em html, dentro dela temos <head> que significa cabeçalho, e <body> que significa corpo.

* Uma tag começa com o sinal de menor ("<") e termina com o sinal de maior (">"). Certifique-se sempre de fechar cada tag, pois embora algumas tags especiais sejam fechadas por padrão, a maior parte delas não são.

* Como se guardassemos uma caixa, dentro de outra caixa, e dentro dela colocássemos outra caixa, e outra caixa... Assim criamos elementos dentro de elementos, e para não confundir o navegador aninhamos nossos elementos, aninhar significa dar esses espaços. 

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

##Tags do html5

`<section>` Define uma seção<br>
`<nav>` Define um menu com links de navegação<br>
`<article>` Pode definir um artigo, um comentário enviado pelo usuário, etc<br>
`<aside>` Define um conteúdo reservado dentro página.<br>
`<header>` Define o cabeçalho de uma página ou seção.<br>
`<footer>` Define o rodapé de uma página ou seção. <br>
`<main>` Define o conteúdo principal ou importante no documento. Deve existir apenas um.<br>

##Títulos

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
http://jlcarvalho.github.io/guia-frontend/
