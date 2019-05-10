---
description: Vamos descobrir como deixar as páginas cheias de estilo
---

# Começando com CSS

### Introdução

Agora que já conhecemos bastante sobre HTML. Vamos aprender sobre as folhas de estilo em cascata, ou CSS, a linguagem responsável por estilizar as nossas páginas em HTML. 

### Adicionando estilos

Podemos adicionar estilos em uma página de três formas. Uma delas é adicionando o atributo style na própria marcação:

```markup
<p style="color: #f05a20;">Vai na Web</p>
```

Outra forma, é adicionar na header do documento a marcação style:

```markup
<head>
    <style>
        /* seu CSS aqui */
    </style>
</head>
<body>
    <p>Vai na Web</p>
</body>
```

A última forma e mais comum e recomendada é importar a folha de estilos. Basta criar o arquivo estilos.css, e importa-lo na `<head>` do html. Ah! chamamos nosso arquivo de estilos.css, mas você pode criar um arquivo com o nome que quiser e utilizá-lo. Lembre-se de colocar junto ao nome do arquivo a extensão dele, ou seja, .css, no final.

```markup
<head>
    <title>Vai na Web</title>
    <link rel="stylesheet" href="estilos.css" />
</head>
<body>
    <p>Vai na Web</p>
</body>
```

### Sintaxe

Precisamos compreender a sintaxe que a linguagem usa. Pensar na sintaxe de uma linguagem significa pensar nas relações formais que unem as partes constituintes da sentença, criando uma estrutura. Ou seja, trata-se de pensar na estrutura através da qual ela é escrita.

```css
seletor {
    propriedade: valor;
}
```

Assim podemos fazer com que nossa página fique muito legal. Podemos alterar as cores, tamanhos, formas e até adicionar animações! Nas próximas aulas, vamos conhecer melhor essas e outras propriedades e valores.

### Principais seletores

Acontece mais ou menos assim: selecionamos os elementos do HTML que queremos estilizar e, então, o CSS define como, onde e quando colocar esses estilos. Vamos começar a entender sobre os [seletores](https://code.tutsplus.com/pt/tutorials/the-30-css-selectors-you-must-memorize--net-16048).

Podemos dar estilo diretamente ao próprio elemento do HTML.

```markup
<p>Olá mundo</p>
```

```css
p {
    color: #f05a20;
}
```

Ou podemos adicionar um ID ao elemento. É legal de ser usado em elementos que não se repetem na página.

```markup
<p id="sobre">Olá mundo</p>
```

```css
#sobre {
    color: #f05a20;
}
```

Podemos, ainda, adicionar uma classe ao elemento. Muito útil para as que se repetem ao longo da página.

```markup
<p class="sobre">Olá mundo</p>
```

```css
.sobre {
    color: #f05a20;
}
```

### Entenda a cascata

Dependendo da posição em que o CSS esteja sendo chamado na página o código tem uma certa prioridade na hora de ser exibido pelo navegador. Como nas pedras da cachoeira, a água flui melhor em alguns lugares do que em outros. Esse é um conceito que vai ser muito importante futuramente.

O navegador lê nossa página de baixo para cima, no exemplo a seguir, ambos elementos estão sendo selecionados usando mesmo tipo de seletor, nesse caso as classes, mas a propriedade do bloco de baixo consegue sobrescrever a de cima.

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

Os seletores também têm prioridades diferentes. A classe que tiver important! tem maior prioridade, seguida dela, o ID tem maior prioridade, depois a classe, e por último o próprio elemento. Exemplo:

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

