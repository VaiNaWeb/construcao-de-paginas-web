#Conhecendo CSS e seus poderes

Com o CSS ganhamos o poder de deixar as páginas em HTML cheias de estilo. Funciona exatamente assim: selecionamos o que queremos estilizar, e então algum seletor CSS define como, onde, e até quando colocar esses estilos. 

##Adicionando ao documento

Podemos adicionar a CSS em nossa página HTML de três formas:

###Em linha usando o atributo style

```html
<p style="color: #f05a20;">Vai na Web</p>
```

###Direto no `<head>`

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

###Externamente

Dessa forma, criamos um arquivo chamado estilos.css, e o chamamos no `<head>` do html. Ah! chamamos nosso arquivo de estilos.css, mas você pode criar um arquivo com o nome que quiser e chamo-lo ai, lembre-se de colocar junto ao nome do arquivo a extensão dele, ou seja .css no final.

```html
<head>
	<title>Vai na Web</title>
	<link rel="stylesheet" href="estilos.css" />
</head>
<body>
    <p>Vai na Web</p>
</body>
```

```css
p {
	color: #f05a20;
}
```

##Sintaxe

Precisamos compreender a sintaxe que a linguagem usa. Pensar na sintaxe de uma linguagem, significa pensar nas relações formais que unem as partes que constituem a sentença, criando uma estrutura. Ou seja, pensar na estrutura como ela é escrita.

```css
seletor {
	propriedade: valor;
}

```

Assim podemos fazer com que nossa página fique muito legal. Podemos alterar as cores, tamanhos, formas, e até adicionar animações! Nas próximas aulas vamos conhecer melhor mais propriedades e valores.

##Principais seletores

Precisamos dizer ao CSS qual elemento queremos selecionar, e adicionar a ele os estilos que queremos. Mas para para isso, precisamos entender sobre os seletores.

###Elemento

Podemos dar estilo diretamente ao próprio elemento do HTML.

```css
p {
	color: #f05a20;
}
```

###Id 

Ou podemos adicionar um ID ao elemento. É legal de ser usado em elementos que não se repetem na página.

```css
#sobre {
	color: #f05a20;
}

```

###Classe

Podemos ainda adicionar uma classe ao elemento. Muito útil em classes que se repetem ao longo dá página.

```css
.sobre {
	color: #f05a20;
}
```

## As cores na web

## RGB

## Hexadecimais

Essa foi apenas uma introdução sobre como adicionamos os estilos. Vamos conhecer novas propriedades nas próximas aulas e entender como elas funcionam, até lá, não deixem de praticar.

##Leia mais!
https://code.tutsplus.com/pt/tutorials/the-30-css-selectors-you-must-memorize--net-16048