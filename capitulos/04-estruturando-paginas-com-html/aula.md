# Estruturando páginas com HTML

O HTML usa um conjunto predefinido de elementos para identificar os diversos tipos de conteúdo. Os elementos contém uma ou mais tags que abrangem ou expressam um determinado conteúdo. Cada tag funciona como uma etiqueta que diz ao navegador qual elemento está escrito ali e como ele deve interpretá-lo. Por isso, cada tag tem seu significado e deve ser usada corretamente.

Uma tag começa com o sinal de menor &lt; e termina com o sinal de maior &gt;. Certifique-se de sempre fechar cada tag, pois, embora algumas tags especiais sejam fechadas por padrão, a maior parte delas não é.

Exemplo:

```markup
<p>Olá, eu sou um parágrafo.</p>
```

Algo importantate sobre as tags HTML é que elas devem dizer exatamente o que é o conteúdo entre sua tag de abertura e fechamento. Devemos marcar com as tags quais partes do conteúdo são parágrafos, títulos, listas, etc, chamamos isso de Semântica.

Nossa estrutura HTML contém vários elementos diferentes e, como vimos anteriormente, alguns elementos até estão dentro de outros elementos, como se guardássemos uma caixa dentro de outra caixa e dentro dela colocássemos outra caixa, e outra caixa... Confuso, não é?

Imaginar a cena das caixas já pode ter sido confuso para muita gente, assim como para o navegador diante de elementos dispostos dessa forma. Para que isso não aconteça, nós aninhamos nossos elementos, ou seja, usamos esses espaçamentos nas linhas para indicar que um elemento está dentro de outro. Exemplo:

```markup
<section>
    <p>Olá, eu sou um parágrafo.</p> 
</section>
```

Para construir uma página, marcamos todos os conteúdos com as tags. Há algumas tags principais que compõem uma página padrão. Toda página na web tem uma tag html, head e body. A tag `html` indica elementos em html, dentro dela temos `<head>`, que significa cabeça, e `<body>`, que significa corpo.

Fazendo uma analogia ao corpo humano, na cabeça temos as coisas que não vemos, coisas que pensamos e que são importantes para nosso funcionamento. Mas as coisas do nosso corpo são as partes de nós que podem ser vistas. Assim é no HTML, as coisas que ficam na `head` são importantes, mas não são vistas diretamente no navegador, o nosso conteúdo precisa ser visto, então ele deve ficar na `body`.

Um exemplo de elemento importante mas não precisa ser visto diretamente na página é o `title`. Veremos outros no decorrer deste módulo.

```markup
<html>
    <head>
        <title>Título</title>
    </head>
    <body>
        <p>Olá mundo!</p>
    </body>
</html>
```

Há vários [elementos](https://developer.mozilla.org/pt-BR/docs/Aprender) diferentes, continue conhecendo mais alguns!

