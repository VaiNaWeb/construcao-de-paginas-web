#Introdução ao HTML e CSS

##Como nos comunicamos através da Internet

Quando dois computadores estão conectados à Internet eles podem conversar uns com os outros.

O conteúdo de um site é organizado dentro de um conjunto especial de regras que os computadores entendem; Tipo de como falar em uma linguagem secreta, codificada.

Nós já aprendemos que podemos usar o Github Pages, e nossas páginas ficam disponíveis e podem ser acessadas em qualquer computador. Isso, porque nossas páginas ficam armazenadas nos servidores do Github. Toda vez que pedimos ao navegador para acessar nossa página, o servidor do Github nos envia rapidamente uma cópia dos arquivos dessa página para que ela possa ser interpretada através do navegador.

Explicando de forma mais clara, o navegador pede os arquivos que contém os códigos do site - que estão armazenados no servidor - através do endereço. O servidor então envia os arquivos de volta para que o navegador possa interpretar seu código e exibir a página na tela.

Um servidor é um computador especial que contém arquivos de páginas da web. Seu computador em casa ou na escola não é um servidor, porque ele não está conectado diretamente à Internet. Nós nos conectamos à Internet através de um Provedor de Serviços de Internet.

Por isso, um site que você escreve no seu computador, até que você o hospede em um servidor, não pode ser visto por outras pessoas em um computador diferente.

##Como páginas da Web são construídas

No final dos anos 80 um físico chamado Tim Berners-Lee, começou a idealizar como cientistas poderiam compartilhar documentos através da rede.

Em 1990 Tim sugeriu um padrão para construção de documentos com hipertextos, e assim logo nasceu a Linguagem de Marcação de Hipertexto, a HTML, que evoluiu muito até chegar na versão atual.

Você pode imaginar um site como um grande livro, onde páginas e mais páginas são ligadas umas as outras, e durante os capítulos podemos colocar atalhos para outras páginas, diferente do livro, não precisamos folhear, tudo está ao alcance de um clique. Assim como o conteúdo de um livro, nossos sites contém textos, que são organizados com os elementos em HTML, que vamos aprender, e os nossos navegadores já conhecem muito bem.

###HTML estrutura páginas

A HTML é a linguagem base de uma página da Web. É ela quem cria a estrutura das nossas páginas, que podem conter textos, imagens, vídeos, e dar vida a tantos sites fantásticos que conhecemos hoje. Um documento em HTML é composto por uma estrutura formada por TAGS, que são marcações para identificar os diversos tipos de conteúdos e ainda organiza-los de forma semântica.

###CSS estiliza

Até então as páginas já tinham uma estrutura, e podiam ser acessadas, mas as pessoas começaram a pensar em como torna-las mais amigáveis e estéticamente bonitas, e isso era muito difícil de fazer somente com HTML. Algum tempo depois, em 1996 nasceu a Folha de Estilos em Cascata, a CSS, que veio para deixar as nossas páginas literalmente cheias de estilo!

###JS cria interações

Tudo continuou evoluindo maravilhosamente rápido, e algum tempo depois foi criada a linguagem Javascript que serve para muitas coisas, como validar valores de um formulário para garantir que são aceitáveis antes de serem enviados ao servidor por exemplo, e coisas bem mais complexas que vamos ver mais adiante no curso.

##Estrutura básica HTML

Já aprendemos o que é e para que serve, agora vamos conhecer suas principais TAGs, que compõem a estrutura básica de um documento em HTML.

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

A HTML usa um conjunto pré-definido de elementos para identificar os diversos tipos de conteúdo. Os elementos, contém uma ou mais tags que contém ou expressam um determinado conteúdo.

Cada tag funciona como uma etiqueta, que diz ao navegador qual elemento está escrito ali e como ele deve interpretar, por isso, cada tag tem seu significado e deve ser usado corretamente. A tag <html> indica que dentro dela haverá elementos em html, dentro dela temos <head> que significa cabeçalho, e <body> que significa corpo.

Uma tag começa com o sinal de menor ("<") e termina com o sinal de maior (">"). Certifique-se sempre de fechar cada tag, pois embora algumas tags especiais sejam fechadas por padrão, a maior parte delas não são.

Exemplo:

```html
<p>Olá eu sou um parágrafo.</p>
```

Nossa estrutura HTML contém vários elementos diferentes, e como vimos anteriormente, alguns elementos até estão dentro de outros elementos. Como se guardassemos uma caixa, dentro de outra caixa, e dentro dela colocássemos outra caixa, e outra caixa... Confuso, não é?

Imaginar a cena das caixas já pode ter sido confuso para muita gente, e para o navegador poderia ser também. Para que isso não aconteça, nós aninhamos nossos elementos, ou seja, usamos esses espaçamentos nas linhas para indicar que um elemento está dentro de outro. Exemplo:

```html
<section>
	<p>Olá eu sou um parágrafo.</p> 
</section>
```
Construíamos essas caixas simplesmente com uma tag chamada `<div>`. Imagine que um menu era chamado de div, um rodapé era chamado de div, uma seção era chamada de div, isso era bastante confuso. Com a chegada do HTML5, que vamos estudar nesse curso, ganhamos algumas tags com significado semântico, o que foi bastante importante para os navegadores, usuários e facilitou claro a nossa vida de desenvolvedor também. Agora temos uma tag `<header>` para cabeçalho, uma tag `<footer>` para rodapé, e mais algumas:

`<section>` Define uma seção<br>
`<nav>` Define um menu com links de navegação<br>
`<article>` Pode definir um artigo, um comentário enviado pelo usuário, etc<br>
`<aside>` Define um conteúdo reservado dentro página.<br>
`<header>` Define o cabeçalho de uma página ou seção.<br>
`<footer>` Define o rodapé de uma página ou seção. <br>
`<main>` Define o conteúdo principal ou importante no documento. Deve existir apenas um.<br>

Existem seis níveis diferentes de títulos, `H1` é o mais importante,` h6` é o menos importante. Em HTML, o texto para cabeçalhos é escrito dentro dos elementos de título: `<h1>`, `<h2>`, `<h3>`, `<h4>`, `<h5>` ou `<h6>`.

Exemplo:

```html
<h1>Eu sou o título mais importante!</h1>
<h2>Eu sou um pouco menos importante</h2>
<h3>Eu sou um pouco menos importante</h3>
<h4>Eu sou um pouco menos importante</h4>
<h5>Eu sou um pouco menos importante</h5>
<h6>Eu sou o menos importante</h6>
```

Para incluir imagens em nossa página, precisamos chamar-las através do elemento `<img>` e adicionar um caminho para a imagem que queremos. Dentro da tag de abertura deste elemento, adicionaremos um atributo que especifica onde obter a imagem que queremos incluir. Atributos são coisas que podemos acrescentar a elementos que ajudam a fazer coisas bem específicas, vamos aprender mais  sobre eles no decorrer do curso. 

Um elemento `<img>` sempre terá um atributo src e um alt. Ah! Um elemento `<img>` é um daqueles elementos especiais que não precisam de tag de fechamento, ela já se auto fecha.

Exemplo:

```html
<img src="http://www.vainaweb.com.br/img/vainaweb.svg"/>
```

Há vários elementos diferentes, continue conhecendo mais alguns!<br>
https://developer.mozilla.org/pt-BR/docs/Aprender<br>
https://developer.mozilla.org/pt-BR/docs/Web/HTML/HTML5/HTML5_element_list
