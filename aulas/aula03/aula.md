#Introdução ao HTML e CSS

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

A HTML usa um conjunto predefinido de elementos para identificar os diversos tipos de conteúdo. Os elementos contém uma ou mais tags que abrangem ou expressam um determinado conteúdo.

Cada tag funciona como uma etiqueta que diz ao navegador qual elemento está escrito ali e como ele deve interpretá-lo. Por isso, cada tag tem seu significado e deve ser usada corretamente. A tag <html> indica elementos em html, dentro dela temos <head>, que significa cabeçalho, e <body>, que significa corpo.

Uma tag começa com o sinal de menor ("<") e termina com o sinal de maior (">"). Certifique-se de sempre fechar cada tag, pois, embora algumas tags especiais sejam fechadas por padrão, a maior parte delas não é.

Exemplo:

```html
<p>Olá, eu sou um parágrafo.</p>
```

Nossa estrutura HTML contém vários elementos diferentes e, como vimos anteriormente, alguns elementos até estão dentro de outros elementos, como se guardássemos uma caixa dentro de outra caixa e dentro dela colocássemos outra caixa, e outra caixa... Confuso, não é?

Imaginar a cena das caixas já pode ter sido confuso para muita gente, assim como para o navegador diante de elementos dispostos dessa forma. Para que isso não aconteça, nós aninhamos nossos elementos, ou seja, usamos esses espaçamentos nas linhas para indicar que um elemento está dentro de outro. Exemplo:

```html
<section>
	<p>Olá, eu sou um parágrafo.</p> 
</section>
```
Antes, construíamos essas caixas simplesmente com uma tag chamada `<div>`. Imagine que um menu era chamado de div, um rodapé era chamado de div, uma seção era chamada de div... isso era bastante confuso. Com a chegada do HTML5, que vamos estudar neste curso, ganhamos algumas tags com significado semântico, o que foi bastante importante para os navegadores e usuários e facilitou, claro, a nossa vida de desenvolvedor também. Agora temos uma tag `<header>` para cabeçalho, uma tag `<footer>` para rodapé e mais algumas:

`<section>` Define uma seção<br>
`<nav>` Define um menu com links de navegação<br>
`<article>` Pode definir um artigo, um comentário enviado pelo usuário etc<br>
`<aside>` Define um conteúdo reservado dentro página.<br>
`<header>` Define o cabeçalho de uma página ou seção.<br>
`<footer>` Define o rodapé de uma página ou seção. <br>
`<main>` Define o conteúdo principal ou importante no documento. Deve existir apenas um.<br>

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

Para incluir imagens em nossa página, precisamos mencioná-las através do elemento `<img>` e adicionar um caminho para a imagem que queremos. Dentro da tag de abertura deste elemento, adicionaremos um atributo que especifica onde obter a imagem que queremos incluir. Atributos são informações que podemos acrescentar a elementos que ajudam a realizar atividades específicas; vamos aprender mais  sobre eles no decorrer do curso.

Um elemento `<img>` sempre terá um atributo src e um alt. Ah! Um elemento `<img>` é um daqueles elementos especiais que não precisam de tag de fechamento.

Exemplo:

```html
<img src="http://www.vainaweb.com.br/img/vainaweb.svg" alt="logo do vai na web">
```

Há vários elementos diferentes, continue conhecendo mais alguns!<br>
https://developer.mozilla.org/pt-BR/docs/Aprender<br>
https://developer.mozilla.org/pt-BR/docs/Web/HTML/HTML5/HTML5_element_list
