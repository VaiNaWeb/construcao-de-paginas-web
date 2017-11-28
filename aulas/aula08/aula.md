# Modelo de caixa com CSS

Continuando as analogias sobre nossos elementos serem caixas, agora imaginem que eles são realmente caixinhas retangulares. Como se em cada um deles houvesse um retângulo invisível.

Em nossas páginas, nós podemos determinar o tamanho, a altura, o preenchimento, o espaçamento, e até as cores dessas caixas. Assim criamos interessantes e belíssimas composições visuais para sites.

Cada caixa tem uma largura e uma altura, que determinamos usando as propriedades <code>width</code> e <code>height</code>.

```css
.elemento {
    width: 100px;
    height: 100px;
}
```
Além de <code>width</code> e <code>height</code> temos também o <code>padding</code> e o <code>margin</code>. <code>Padding</code> pode aumentar o preenchimento de uma caixa, enquanto <code>margin</code> pode aumentar seu espaçamento.

```css
.elemento {
    width: 100px;
    height: 100px;
    padding: 50px;
    margin: 50px;
}
```
Temos também a propriedade <code>border</code>, que pode servir para aplicar estilo às bordas de uma caixa.
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
##Comportamento de bloco

Há caixas que se comportam em forma de bloco e há caixas que se comportam em forma de linha. Cada elemento já tem esse comportamento definido por padrão, mas podemos alterá-lo também. Basta alterar os valores da propriedade display com <code>inline</code>, ou <code>block</code>.

Elementos que se comportam como bloco, como <code>h1</code>, <code>h2</code>, <code>h3</code>, <code>p</code>, <code>ul</code>, <code>li</code>, ocupam toda a largura de uma página. Assim sendo, se duas caixas que se comportam como bloco forem adicionadas, a primeira vai querer ocupar toda a largura, então a outra aparecerá abaixo dela, ocupando também toda a largura da página.
```css
p {
    display: block;
}
```
Alguns exemplos de elementos que se comportam em forma de linha são a, <code>img</code>, <code>input</code>, <code>label</code>. Eles não tentam ocupar uma largura que não precisam, dessa forma conseguem ser alinhados visualmente em uma única linha.
```css
a {
    display: inline;
}
```
Testem, testem e testem! Explorem sem medo todas as propriedades e valores que foram vistos hoje. Aproveitem todas as possibilidades que eles podem criar. Na dúvida, sintam-se à vontade para usar o inspetor do navegador e ter uma melhor visualização do comportamento dos seus estilos.
