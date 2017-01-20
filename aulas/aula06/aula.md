#Modelo de caixa com CSS

Continuando as analogias sobre nossos elementos serem caixas, agora imaginem que eles são realmente caixinhas retangulares. Como se em cada um deles houvesse um retângulo invisível.

Em nossas páginas, nós podemos determinar o tamanho, a altura, o preenchimento, o espaçamento, e até as cores dessas caixas. Assim criamos interessantes e belíssimas composições visuais para sites.

Cada caixa tem uma largura e uma altura, que determinamos usando as propriedades width e height.

```css
.elemento {
  width: 100px;
  height: 100px;
}
```
Além de width e height temos também o padding e o margin. Padding pode aumentar o preenchimento de uma caixa, enquanto margin pode aumentar seu espaçamento.

```css
.elemento {
  width: 100px;
  height: 100px;
  padding: 50px;
  margin: 50px;
}
```
Temos também a propriedade border, que pode servir para aplicar estilo às bordas de uma caixa.
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

Há caixas que se comportam em forma de bloco e há caixas que se comportam em forma de linha. Cada elemento já tem esse comportamento definido por padrão, mas podemos alterá-lo também. Basta alterar os valores da propriedade display com inline, ou block.

Elementos que se comportam como bloco, como h1, h2, h3, p, ul, li, ocupam toda a largura de uma página. Assim sendo, se duas caixas que se comportam como bloco forem adicionadas, a primeira vai querer ocupar toda a largura, então a outra apacerá abaixo dela, ocupando também toda a largura da página.
```css
p {
  display: block;
}
```
Alguns exemplos de elementos que se comportam em forma de linha são a, img, input, label. Eles não tentam ocupar uma largura que não precisam, dessa forma conseguem ser alinhados visualmente em uma única linha.
```css
a {
  display: inline;
}
```
Testem, testem e testem! Explorem sem medo todas as propriedades e valores que foram vistos hoje. Aproveitem todas as possibilidades que eles podem criar. Na dúvida, sintam-se à vontade para usar o inspetor do navegador e ter uma melhor visualização do comportamento dos seus estilos.
