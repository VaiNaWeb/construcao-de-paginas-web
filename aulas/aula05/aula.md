Antes, construíamos essas caixas simplesmente com uma tag chamada `<div>`. Imagine que um menu era chamado de div, um rodapé era chamado de div, uma seção era chamada de div... isso era bastante confuso. Com a chegada do HTML5, que vamos estudar neste curso, ganhamos algumas tags com significado semântico, o que foi bastante importante para os navegadores e usuários e facilitou, claro, a nossa vida de desenvolvedor também. Agora temos uma tag `<header>` para cabeçalho, uma tag `<footer>` para rodapé e mais algumas:

`<section>` Define uma seção<br>
`<nav>` Define um menu com links de navegação<br>
`<article>` Pode definir um artigo, um comentário enviado pelo usuário etc<br>
`<aside>` Define um conteúdo reservado dentro página.<br>
`<header>` Define o cabeçalho de uma página ou seção.<br>
`<footer>` Define o rodapé de uma página ou seção. <br>
`<main>` Define o conteúdo principal ou importante no documento. Deve existir apenas um.<br>

![asset](assets/01.png)

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
