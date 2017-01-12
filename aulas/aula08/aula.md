#Modelo de caixa com CSS

Continuando as analogias sobre nossos elementos serem caixas, agora imaginem que eles são realmente caixinhas retangulares. Como se em cada um deles houvesse um retângulo invisível.

Em nossas páginas nós podermos determinar o tamanho, altura, preenchimento, espaçamento, e até cores dessas caixas. Assim criamos interessantes e belíssimos layouts para sites.

Cada caixa tem uma largura e altura, que determinamos usando as propriedades width e height.

```css
.elemento {
  width: 100px;
  height: 100px;
}
```
Além do width e height temos também o padding e margin, que servem para dar espaçamento. Padding pode aumentar o preenchimento de uma caixa, enquanto margin, pode aumentar seu espaçamento.

```css
.elemento {
  width: 100px;
  height: 100px;
  padding: 50px;
  margin: 50px;
}
```
Temos também a propriedade border que pode servir para aplicar estilo às bordas de uma caixa.
```css
.elemento {
  width: 100px;
  height: 100px;
  padding: 50px;
  margin: 50px;
  border: 5px solid black;
}
```
