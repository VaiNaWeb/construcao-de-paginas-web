# Modelo de caixa com CSS

### Introdução

Continuando as analogias sobre nossos elementos serem caixas, agora imaginem que eles são realmente caixinhas retangulares. Como se em cada um deles houvesse um retângulo invisível.

Em nossas páginas, nós podemos determinar o tamanho, a altura, o preenchimento, o espaçamento, e até as cores dessas caixas. Assim criamos interessantes e belíssimas composições visuais para sites.

Cada caixa tem uma largura e uma altura, que determinamos usando as propriedades `width` e `height`.

```css
.elemento {
    width: 100px;
    height: 100px;
}
```

Além de `width` e `height` temos também o `padding` e o `margin`. `Padding` pode aumentar o preenchimento de uma caixa, enquanto `margin` pode aumentar seu espaçamento.

```css
.elemento {
    width: 100px;
    height: 100px;
    padding: 50px;
    margin: 50px;
}
```

Temos também a propriedade `border`, que pode servir para aplicar estilo às bordas de uma caixa.

```css
.elemento {
    width: 100px;
    height: 100px;
    padding: 50px;
    margin: 50px;
    border-width: 5px;
    border-style: solid;
    border-color: black;
}
```

### Comportamento de bloco

Há caixas que se comportam em forma de bloco e há caixas que se comportam em forma de linha. Cada elemento já tem esse comportamento definido por padrão, mas podemos alterá-lo também. Basta alterar os valores da propriedade display com `inline`, ou `block`.

Elementos que se comportam como bloco, como `h1`, `h2`, `h3`, `p`, `ul`, `li`, ocupam toda a largura de uma página. Assim sendo, se duas caixas que se comportam como bloco forem adicionadas, a primeira vai querer ocupar toda a largura, então a outra aparecerá abaixo dela, ocupando também toda a largura da página.

```css
div {
    display: block;
}
```

Alguns exemplos de elementos que se comportam em forma de linha são a, `img`, `input`, `label`. Eles não tentam ocupar uma largura que não precisam, dessa forma conseguem ser alinhados visualmente em uma única linha.

```css
div {
    display: inline;
}
```

Com o valor none, o elemento simplesmente não é mostrado.

```css
div {
    display: none;
}
```

### Modelo de caixa

No modelo de caixa, o valor padrão é o content-box, isso quer dizer que se não alterarmos, ele é o valor que aparece em todos os elementos. O tamanho de um elemento começa com as propriedades de largura e altura e, em seguida, quaisquer valores de preenchimento, borda ou margem são somados a partir daí.

```css
div {
    box-sizing: content-box;
}
```

O `content-box` costuma deixar alguns desenvolvedores confusos, por isso comumente preferimos usar o border-box. Ao usar o valor border-box, se um elemento tiver uma largura de 400 pixels, um preenchimento de 20 pixels ao redor de cada lado e uma borda de 10 pixels ao redor de cada lado, a largura real permanecerá em 400 pixels.

```css
div {
    box-sizing: border-box;
}
```

Se adicionarmos uma margem, esses valores precisarão ser adicionados para calcular o tamanho total da caixa. Não importa qual valor de propriedade de dimensionamento de caixa seja usado, quaisquer valores de margem precisarão ser adicionados para calcular o tamanho completo do elemento.

Testem, testem e testem! Explorem sem medo todas as propriedades e valores que foram vistos hoje. Aproveitem todas as possibilidades que eles podem criar. Na dúvida, sintam-se à vontade para usar o inspetor do navegador e ter uma melhor visualização do comportamento dos seus estilos.

### Referências

[CSS: From Zero to Hero](https://dev.to/aspittel/css-from-zero-to-hero-3o16)  
[Box Model by Mozilla](https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS/Box_model)

