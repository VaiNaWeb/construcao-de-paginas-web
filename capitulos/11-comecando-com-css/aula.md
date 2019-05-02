---
description: Vamos descobrir como deixar as páginas cheias de estilo
---

# Começando com CSS

## Introdução

Imagine uma cachoeira enorme, cheia de pedras, e muita água linda e refrescante caindo em cascata. Assim acontece em nosso navegador, nossos estilos estão em cascata.

As folhas de estilo em cascata, ou CSS, são os códigos responsáveis por estilizar as nossas páginas em HTML. O CSS funciona junto com o HTML. Acontece mais ou menos assim: selecionamos os elementos do HTML que queremos estilizar e, então, o CSS define como, onde e quando colocar esses estilos.

### Adicionando ao documento

Para adicionar CSS em uma página precisamos importa-lo. Podemos fazer isso de três formas:

### Em linha, usando o atributo style

```markup
<p style="color: #f05a20;">Vai na Web</p>
```

### Direto na Head

```markup
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

```markup
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

Dependendo da posição em que o CSS esteja sendo chamado na página o código tem uma certa prioridade na hora de ser exibido pelo navegador. Como nas pedras da cachoeira, a água flui melhor em alguns lugares do que em outros. Esse é um conceito que vai ser muito importante futuramente.

Quem tem maior prioridade sobrescreve que tem menor. A prioridade na cascata de acordo com a forma que chamamos o código na página é a seguinte:

Usando important! &gt; Em linha &gt; Direto na Head &gt; Externamente

Explicando melhor, em algum momento vamos estudar o que esse important faz, por agora, entendam somente que se um estilo estiver usando ele, ele tem maior prioridade, depois dele o estilo que está em linha tem uma prioridade maior, e assim por diante.

Dependendo da posição dentro de um arquivo essa prioridade muda também. O navegador lê nossa página de baixo para cima, no exemplo a seguir, ambos elementos estão sendo selecionados usando mesmo recurso, nesse caso as classes, mas o que está em baixo tem maior prioridade que o de cima.

Logo, quando houver a mesma propriedade, o valor da que tem maior prioridade é exibido, sobrescrevendo a de cima.

```css
.paragrafo {
  background-color: red;
}

.paragrafo {
  background-color: gray;
}
```

Quando as propriedades forem diferentes, elas simplesmente ficam combinadas. Ambas são mostradas. Exemplo:

```css
.paragrafo {
  background-color: red;
}

.paragrafo {
  padding: 20px;
  margin: 20px;
}
```

O navegador entende assim:

```css
.paragrafo {
  background-color: red;
  padding: 20px;
  margin: 20px;
}
```

Os seletores também têm prioridades diferentes. A clase que tiver important! tem maior prioridade, seguida dela, o ID tem maior prioridade, depois a classe, e por último o próprio elemento. Exemplo:

```css
#vermelho {
  background-color: red;
}

.cinza {
  background-color: gray; 
}

p {
  background-color: blue !important;
  color: white;
  padding: 5px;
}
```

Faça alguns testes! O que acontece se você apagar o !important do elemento parágrafo?

### Referências

[CSS Reference, by Codrops](https://tympanus.net/codrops/css_reference/)

