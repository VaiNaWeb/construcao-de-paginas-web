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

###HTML estrutura páginas

A HTML é a linguagem base de uma página da Web. É ela quem cria a estrutura das nossas páginas, que podem conter textos, imagens, vídeos, e dar vida a tantos sites fantásticos que conhecemos hoje. Um documento em HTML é composto por uma estrutura formada por TAGS, que são marcações para identificar os diversos tipos de conteúdos e ainda organiza-los de forma semântica.

###CSS estiliza

Até então as páginas já tinham uma estrutura, e podiam ser acessadas, mas as pessoas começaram a pensar em como torna-las mais amigáveis e estéticamente bonitas, e isso era muito difícil de fazer somente com HTML. Algum tempo depois, em 1996 nasceu a Folha de Estilos em Cascata, a CSS, que veio para deixar as nossas páginas literalmente cheias de estilo!

###JS cria interações

Tudo continuou evoluindo maravilhosamente rápido, e algum tempo depois foi criada a linguagem Javascript que serve para muitas coisas, como validar valores de um formulário para garantir que são aceitáveis antes de serem enviados ao servidor por exemplo, e coisas bem mais complexas que vamos ver mais adiante no curso.

##Estrutura básica HTML

Já aprendemos o que é e para que serve, agora vamos conhecer suas principais TAGs, que compõem a estrutura básica de um documento em HTML.

```
<html>

    <head>
	<title></title>
    </head>

    <body>

        <p>Olá mundo!</p>

    </body>

</html>
```

A HTML usa um conjunto pré-definido de elementos para identificar os diversos tipos de conteúdo. Os elementos, contém uma ou mais tags que contém ou expressam um determinado conteúdo. 

Cada tag funciona como uma etiqueta, que diz ao navegador qual elemento está escrito ali e como ele deve interpretar, por isso, cada tag tem seu significado e deve ser usado corretamente. A tag html indica que dentro dela haverá elementos em html, dentro dela temos head que significa cabeçalho, e body que significa corpo.

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

Há vários elementos diferentes, continue conhecendo mais alguns!<br>
https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element