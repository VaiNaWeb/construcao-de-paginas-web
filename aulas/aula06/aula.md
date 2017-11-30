# Adicionado Áudio, Imagens, Vídeos
    
Quando tudo começou a web era formada principalmente por textos simples, mas essa não é mais a nossa realidade. Navegando na internet encontramos muitos tipos de conteúdo diferentes, além de textos, incluimos em nossas páginas imagens, músicas, vídeos, e até mesmo conteúdo de outras páginas da web.

Hoje, podemos usar livremente imagens, áudio, vídeo e iframes sabendo que esse conteúdo, nossos navegadores modernos oferecem suporte a todas essas coisas muito bem.

## Adicionando imagens

Para incluir imagens em nossa página, precisamos mencioná-las através do elemento `<img>` e adicionar um caminho para a imagem que queremos. Dentro da tag de abertura deste elemento, adicionaremos um atributo que especifica onde obter a imagem que queremos incluir. 

Atributos são informações que podemos acrescentar a elementos que ajudam a realizar atividades específicas; vamos aprender mais  sobre eles no decorrer do curso.

Um elemento `<img>` sempre terá um atributo src e um alt. Note, nesse exemplo usamos uma URL com a imagem que queremos mostrar dentro do src. O atributo alt é serve para mostrar uma descrição da imagem, isso é importante para manter acessibilidade.

Ah! Um elemento `<img>` é um daqueles elementos especiais que não precisam de tag de fechamento. Exemplo:

```html
<img src="http://www.vainaweb.com.br/img/vainaweb.svg" alt="logo do vai na web">
```

## Adicionando áudio

Para adicionar arquivos de áudio usamos o elemento `<audio>`. Assim como acontece com o elemento `<img>`, o elemento `<audio>` aceita um URL de origem especificado pelo atributo src. Ao contrário do elemento `<img>`, o elemento `<audio>` precisa das tags de abertura e de fechamento.

```html
<audio src="https://raw.githubusercontent.com/VaiNaWeb/primeiros-passos-na-web/master/aulas/aula06/assets/Sour_Tennessee_Red_Sting.mp3" controls="controls"></audio>
```

Vários outros atributos podem acompanhar o atributo src no elemento `<audio>`. Os mais populares incluem reprodução automática, controles, loop e pré-carregamento.

Os atributos de reprodução automática, controles e loop são atributos booleanos. Booleanos retornam true ou false, em HTML, se um atributo booleano estiver presente ele já significa true e retorna a funcionalidade. Logo, não precisamos atribuir valores, basta adiciona-lo. 

Por padrão, o elemento `<audio>` não é exibido em uma página. Se o atributo de reprodução automática estiver presente no elemento `<audio>`, nada aparecerá na página, mas o arquivo de áudio será executado automaticamente após o carregamento. Exemplo:
    
```html
<audio src="https://raw.githubusercontent.com/VaiNaWeb/primeiros-passos-na-web/master/aulas/aula06/assets/Sour_Tennessee_Red_Sting.mp3" controls="controls" autoplay></audio>
```

Um outro atributo booleano que pode ser usado também é o download, veja um exemplo usando ele em um link:

```html
<audio src="https://raw.githubusercontent.com/VaiNaWeb/primeiros-passos-na-web/master/aulas/aula06/assets/Sour_Tennessee_Red_Sting.mp3" controls>
  <a href="https://raw.githubusercontent.com/VaiNaWeb/primeiros-passos-na-web/master/aulas/aula06/assets/Sour_Tennessee_Red_Sting.mp3" download>Baixar</a> arquivo de áudio.
</audio>
```

## Adicionando vídeo

Para adicionar vídeo usamos o elemento `<video>`. Os mesmos atributos src, reprodução automática, controles, loop, que funcionam no áudio funcionam no vídeo também.

É recomendado incluir sempre o atributo booleano dos controles, a menos que haja uma boa razão para não permitir que os usuários comecem, parem ou reproduzam o vídeo.

Como os vídeos ocupam espaço na página, não faz mal especificar suas dimensões, o que é mais comumente feito com propriedades de largura e altura em CSS. Especificar um tamanho, como as imagens, ajuda o navegador a renderizar vídeos mais rapidamente e permite usar o espaço certo para que o vídeo seja exibido.

Uma propriedade também interessante de colocar é o type, que indica qual o tipo do arquivo que você está querendo mostrar, ele funciona no áudio e também no vídeo.

```html
<video src="https://raw.githubusercontent.com/VaiNaWeb/primeiros-passos-na-web/master/aulas/aula06/assets/vnwcpx.mp4" type="video/mp4" autoplay loop width="426" height="240">
</video>
```
Em muitas páginas, como no Youtube, as pesssoas preferem mostrar uma imagem de fundo ao vídeo, podemos adicionar essa imagem usando o atributo poster e como valor a URL da imagem que queremos mostrar.

```html
<video src="https://raw.githubusercontent.com/VaiNaWeb/primeiros-passos-na-web/master/aulas/aula06/assets/vnwcpx.mp4" type="video/mp4" poster="https://raw.githubusercontent.com/VaiNaWeb/primeiros-passos-na-web/master/aulas/aula06/assets/imgfallback.jpg
" width="426" height="240" controls>
</video>
```

## Adicionando iframes

## Figuras e legendas
