# Adicionado Áudio, Imagens, Vídeos
    
Quando tudo começou a web era formada principalmente por textos simples, mas essa não é mais a nossa realidade. Navegando na internet encontramos muitos tipos de conteúdo diferentes, além de textos, incluimos em nossas páginas imagens, músicas, vídeos, e até mesmo conteúdo de outras páginas da web.

Hoje, podemos usar livremente imagens, áudio, vídeo e iframes sabendo que esse conteúdo, nossos navegadores modernos oferecem suporte a todas essas coisas muito bem.

## Adicionando imagens

Para incluir imagens em nossa página, precisamos mencioná-las através do elemento `<img>` e adicionar um caminho para a imagem que queremos. Dentro da tag de abertura deste elemento, adicionaremos um atributo que especifica onde obter a imagem que queremos incluir. 

Atributos são informações que podemos acrescentar a elementos que ajudam a realizar atividades específicas; vamos aprender mais  sobre eles no decorrer do curso.

Um elemento `<img>` sempre terá um atributo src e um alt. Note, nesse exemplo usamos uma URL com a imagem que queremos mostrar dentro do src. Ah! Um elemento `<img>` é um daqueles elementos especiais que não precisam de tag de fechamento.

Exemplo:

```html
<img src="http://www.vainaweb.com.br/img/vainaweb.svg" alt="logo do vai na web">
```

## Adicionando áudio

Para adicionar arquivos de áudio usamos o elemento <audio>. Assim como acontece com o elemento <img>, o elemento <audio> aceita um URL de origem especificado pelo atributo src. Ao contrário do elemento <img>, o elemento <audio> precisa das tags de abertura e de fechamento.

```html
<audio src="https://raw.githubusercontent.com/VaiNaWeb/primeiros-passos-na-web/master/aulas/aula06/assets/Sour_Tennessee_Red_Sting.mp3" controls="controls"></audio>
```

Vários outros atributos podem acompanhar o atributo src no elemento <audio>. Os mais populares incluem reprodução automática, controles, loop e pré-carregamento.

Os atributos de reprodução automática, controles e loop são atributos booleanos. Booleanos retornam true ou false, em HTML, se um atributo booleano estiver presente ele já significa true e retorna a funcionalidade. Logo, não precisamos atribuir valores, basta adiciona-lo. 

Por padrão, o elemento <audio> não é exibido em uma página. Se o atributo de reprodução automática estiver presente no elemento <audio>, nada aparecerá na página, mas o arquivo de áudio será executado automaticamente após o carregamento. Exemplo:
    
```html
<audio src="https://raw.githubusercontent.com/VaiNaWeb/primeiros-passos-na-web/master/aulas/aula06/assets/Sour_Tennessee_Red_Sting.mp3" controls="controls" autoplay></audio>
```


## Adicionando vídeo

## Adicionando iframes

## Figuras e legendas
