# Adicionando Áudio, Imagens, Vídeos

Quando tudo começou a web era formada principalmente por textos simples, mas essa não é mais a nossa realidade. Navegando na internet encontramos muitos tipos de conteúdo diferentes, além de textos, incluimos em nossas páginas imagens, músicas, vídeos, e até mesmo conteúdo de outras páginas da web.

Hoje, podemos usar livremente imagens, áudio, vídeo e iframes sabendo que esse conteúdo, nossos navegadores modernos oferecem suporte a todas essas coisas muito bem.

## Adicionando imagens

Para incluir imagens em nossa página, precisamos mencioná-las através do elemento `<img>` e adicionar um caminho para a imagem que queremos. Dentro da tag de abertura deste elemento, adicionaremos um atributo que especifica onde obter a imagem que queremos incluir.

Atributos são informações que podemos acrescentar a elementos que ajudam a realizar atividades específicas; vamos aprender mais sobre eles no decorrer do curso.

Um elemento `<img>` sempre terá um atributo src e um alt. Note, nesse exemplo usamos uma URL com a imagem que queremos mostrar dentro do src. O atributo alt é serve para mostrar uma descrição da imagem, isso é importante para manter acessibilidade.

Ah! Um elemento `<img>` é um daqueles elementos especiais que não precisam de tag de fechamento. Exemplo:

```markup
<img src="http://www.vainaweb.com.br/img/vainaweb.svg" alt="logo do vai na web">
```

## Adicionando áudio

Para adicionar arquivos de áudio usamos o elemento `<audio>`. Assim como acontece com o elemento `<img>`, o elemento `<audio>` aceita um URL de origem especificado pelo atributo src. Ao contrário do elemento `<img>`, o elemento `<audio>` precisa das tags de abertura e de fechamento.

```markup
<audio src="https://raw.githubusercontent.com/VaiNaWeb/primeiros-passos-na-web/master/aulas/aula06/assets/Sour_Tennessee_Red_Sting.mp3" controls="controls"></audio>
```

Vários outros atributos podem acompanhar o atributo src no elemento `<audio>`. Os mais populares incluem reprodução automática, controles, loop e pré-carregamento.

Os atributos de reprodução automática, controles e loop são atributos booleanos. Booleanos retornam true ou false, em HTML, se um atributo booleano estiver presente ele já significa true e retorna a funcionalidade. Logo, não precisamos atribuir valores, basta adiciona-lo.

Por padrão, o elemento `<audio>` não é exibido em uma página. Se o atributo de reprodução automática estiver presente no elemento `<audio>`, nada aparecerá na página, mas o arquivo de áudio será executado automaticamente após o carregamento. Exemplo:

```markup
<audio src="https://raw.githubusercontent.com/VaiNaWeb/primeiros-passos-na-web/master/aulas/aula06/assets/Sour_Tennessee_Red_Sting.mp3" controls="controls" autoplay></audio>
```

Um outro atributo booleano que pode ser usado também é o download, veja um exemplo usando ele em um link:

```markup
<audio src="https://raw.githubusercontent.com/VaiNaWeb/primeiros-passos-na-web/master/aulas/aula06/assets/Sour_Tennessee_Red_Sting.mp3" controls>
  <a href="https://raw.githubusercontent.com/VaiNaWeb/primeiros-passos-na-web/master/aulas/aula06/assets/Sour_Tennessee_Red_Sting.mp3" download>Baixar</a> arquivo de áudio.
</audio>
```

## Adicionando vídeo

Para adicionar vídeo usamos o elemento `<video>`. Os mesmos atributos src, reprodução automática, controles, loop, que funcionam no áudio funcionam no vídeo também.

É recomendado incluir sempre o atributo booleano dos controles, a menos que haja uma boa razão para não permitir que os usuários comecem, parem ou reproduzam o vídeo.

Como os vídeos ocupam espaço na página, não faz mal especificar suas dimensões, o que é mais comumente feito com propriedades de largura e altura em CSS. Especificar um tamanho, como as imagens, ajuda o navegador a renderizar vídeos mais rapidamente e permite usar o espaço certo para que o vídeo seja exibido.

Uma propriedade também interessante de colocar é o type, que indica qual o tipo do arquivo que você está querendo mostrar, ele funciona no áudio e também no vídeo.

```markup
<video src="https://raw.githubusercontent.com/VaiNaWeb/primeiros-passos-na-web/master/aulas/aula06/assets/vnwcpx.mp4" type="video/mp4" autoplay loop width="426" height="240">
</video>
```

Em muitas páginas, como no Youtube, as pesssoas preferem mostrar uma imagem de fundo ao vídeo, podemos adicionar essa imagem usando o atributo poster e como valor a URL da imagem que queremos mostrar.

```markup
<video src="https://raw.githubusercontent.com/VaiNaWeb/primeiros-passos-na-web/master/aulas/aula06/assets/vnwcpx.mp4" type="video/mp4" poster="https://raw.githubusercontent.com/VaiNaWeb/primeiros-passos-na-web/master/aulas/aula06/assets/imgfallback.jpg
" width="426" height="240" controls>
</video>
```

## Adicionando iframes

Podemos incorporar outra página HTML em nossa página. Isso é feito usando o elemento `<iframe>`. O elemento `<iframe>` aceita o URL de outra página HTML dentro do valor do atributo src.

Muitas páginas usam o elemento `<iframe>` para incorporar mídia em uma página de um site externo, como Google Maps, YouTube e alguns outros. Exemplo usando o Google Maps:

```markup
<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3676.4405739120457!2d-43.287196449289794!3d-22.860177841883633!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x997c7b48e047c7%3A0x75e759ff43f554c9!2sEDUCAP!5e0!3m2!1spt-BR!2sbr!4v1480440475641" width="100%" height="300" frameborder="0" style="border:0" allowfullscreen></iframe>
```

## Figuras e legendas

Usamos o elemento `<figure>` para envolver algum conteúdo autônomo, muitas vezes na forma de mídia, como imagens, vídeos, ilustrações, etc. Mais de um item de conteúdo, como imagens múltiplas ou vídeos, pode estar contido no elemento `<figure>` de cada vez.

```markup
<figure>
  <img src="http://www.vainaweb.com.br/img/vainaweb.svg" alt="Logo do Programa VaiNaWeb">
</figure>
```

É possvel adicionar uma legenda ao elemento `<figure>`, com o elemento `<figcaption>`. O `<figcaption>` pode aparecer na parte superior, inferior ou em qualquer lugar dentro do elemento `<figure>` mas deve aparecer somente uma vez. Quando é usado, o elemento `<figcaption>` servirá como legenda para todo o conteúdo no elemento `<figure>`. Exemplo:

```markup
<figure>
  <img src="http://www.vainaweb.com.br/img/vainaweb.svg" alt="Logo do Programa VaiNaWeb">
  <figcaption>Logo do Programa VaiNaWeb.</figcaption>
</figure>
```

