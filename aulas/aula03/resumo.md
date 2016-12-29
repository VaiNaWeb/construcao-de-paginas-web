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