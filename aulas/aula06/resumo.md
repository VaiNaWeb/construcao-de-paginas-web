#Modelo de caixa com CSS

- Imaginem que elementos são realmente caixinhas retangulares. Como se em cada um deles houvesse um retângulo invisível.

- Em nossas páginas nós podermos determinar o tamanho, altura, preenchimento, espaçamento, e até cores dessas caixas. Assim criamos interessantes composições para sites.

- Cada caixa tem uma largura e altura, que determinamos usando as propriedades width e height.

- Temos também o padding e margin, padding pode aumentar o preenchimento de uma caixa, enquanto margin, pode aumentar seu espaçamento.

- A propriedade border pode servir para aplicar estilo às bordas de uma caixa.
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

- Há caixas que se comportam em forma de bloco, e há caixas que se comportam como em forma de linha. 

- Cada elemento já tem esse comportamento definido por padrão, mas podemos altera-lo, basta alterar os valores da propriedade display com inline, ou block.

- Elementos que se comportam como bloco, como h1, h2, h3, p, ul, li, ocupam toda a largura de uma página, assim sendo, se duas caixas que se comportam como bloco forem adicionadas, a primeira vai querer ocupar toda a largura, então a outra apacerá abaixo dela, ocupando também toda a largura da página.
```css
p {
  display: block;
}
```
- Elementos que se comportam em forma de linha como a, img, input, label, não tentam ocupar uma largura que não precisam, dessa forma conseguem ser alinhados visualmente em uma única linha.
```css
a {
  display: inline;
}
```
Testem, testem, e testem! Explorem sem medo todas as propriedades e valores que foram vistos hoje. Na dúvida, sintam-se à vontade para usar o inspetor do navegador e ter uma melhor visualização do comportamento dos seus estilos.
