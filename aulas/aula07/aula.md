# Introdução CSS

Vamos descobrir como deixar as páginas cheias de estilo. CSS significa folhas de estilo em cascasta. Imaginem uma cachoeira enorme, cheia de pedras, e muita água linda e refrescante caindo em cascata. Assim acontece em nosso navegador, nossos códigos estão em cascata.

É importante saber que o CSS não trabalha sozinho, precisamos usa-lo com o HTML. Funciona exatamente assim: selecionamos os elementos do HTML que queremos estilizar e, então, algum seletor CSS define como, onde e quando colocar esses estilos.

## Adicionando ao documento

Podemos adicionar a CSS em nossa página HTML de três formas:

### Em linha, usando o atributo style
```html
<p style="color: #f05a20;">Vai na Web</p>
```

### Direto na Head
```html
<head>
	<style>
		p { color: #f05a20; }
	</style>
</head>
<body>
	<p>Vai na Web</p>
</body>
```

### Externamente

Dessa forma, criamos um arquivo chamado estilos.css, e o aplicamos no `<head>` do html. Ah! chamamos nosso arquivo de estilos.css, mas você pode criar um arquivo com o nome que quiser e utilizá-lo. Lembre-se de colocar junto ao nome do arquivo a extensão dele, ou seja, .css, no final.
```html
<head>
	<title>Vai na Web</title>
	<link rel="stylesheet" href="estilos.css" />
</head>
<body>
    <p>Vai na Web</p>
</body>
```

## Sintaxe

Precisamos compreender a sintaxe que a linguagem usa. Pensar na sintaxe de uma linguagem significa pensar nas relações formais que unem as partes constituintes da sentença, criando uma estrutura. Ou seja, trata-se de pensar na estrutura através da qual ela é escrita.
```css
seletor {
	propriedade: valor;
}
```

Assim podemos fazer com que nossa página fique muito legal. Podemos alterar as cores, tamanhos, formas e até adicionar animações! Nas próximas aulas, vamos conhecer melhor essas e outras propriedades e valores.

## Principais seletores

Precisamos dizer ao CSS qual elemento queremos selecionar e adicionar a ele os estilos que desejamos. Mas, para isso, devemos entender sobre os [seletores](https://code.tutsplus.com/pt/tutorials/the-30-css-selectors-you-must-memorize--net-16048).

### Elemento

Podemos dar estilo diretamente ao próprio elemento do HTML.
```css
p {
	color: #f05a20;
}
```

### Id 

Ou podemos adicionar um ID ao elemento. É legal de ser usado em elementos que não se repetem na página.
```css
#sobre {
	color: #f05a20;
}
```

### Classe

Podemos, ainda, adicionar uma classe ao elemento. Muito útil para as que se repetem ao longo da página.
```css
.sobre {
	color: #f05a20;
}
```

## Fluindo na Cascata

Dependendo da posição em que o CSS esteja sendo chamado na página o código tem uma certa prioridade na hora de ser exibido pelo navegador. Como nas pedras da cachoeira, a água flui  melhor em alguns lugares do que em outros. Esse é um conceito que vai ser muito importante futuramente.

Quem tem maior prioridade sobrescreve que tem menor. A prioridade na cascata de acordo com a forma que chamamos o código na página é a seguinte:

Usando important! > Em linha > Direto na Head > Externamente

Explicando melhor, em algum momento vamos estudar o que esse important faz, por agora, entendam somente que se um estilo estiver usando ele, ele tem maior prioridade, depois dele o estilo que está em linha tem uma prioridade maior, e assim por diante.

Dependendo da posição dentro de um arquivo essa prioridade muda também.
