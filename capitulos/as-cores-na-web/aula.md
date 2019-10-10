# As cores na web

### Introdução

Aprenderemos como colocar cores na web. Há alguns [sistemas de cores](https://tableless.com.br/sobre-cor-e-webdesign/) que precisamos conhecer para entender como adiciona-las em nossas folhas de estilo.

### RGB

Monitores são pretos e iluminados por vários pontinhos de luz: pixels. Vamos somando pontinhos vermelhos, verdes e azuis até chegar na cor desejada. A cor RGB é formada por um conjunto de três números de três dígitos; cada número refere-se a uma das cores base do sistema (vermelho, verde e azul). Quanto mais alto o número mais clara é a cor.

```css
p {
    color: rgb(0, 0, 255);
}
```

Eventualmente, podemos precisar alterar a opacidade da cor, deixando ela mais transparente (próximo de 0) ou mais opaca (próoximo de 1). Para isso, usa-se um quarto número, que representa o canal alpha da cor.

```css
p {
    color: rgb(0, 0, 255, 0.5);
}
```

### Hexadecimais

Compostos por uma combinação de três conjuntos de pares formados a partir de número e letras de A a F. Quanto mais alto o número mais clara é a cor.

Cada par é responsável por uma cor, assim como o RGB, Vermelho, verde e azul. Ou seja \#ff0000 é o vermelho, e o \#00ff00 é o verde e \#0000ff é o azul.

```css
p {
    color: #ff0000;
}
```

### Referências

[http://lokeshdhakar.com/projects/color-thief/](http://lokeshdhakar.com/projects/color-thief/)  
[http://moviesincolor.com/](http://moviesincolor.com/)  
[https://color.adobe.com/pt/create/color-wheel/](https://color.adobe.com/pt/create/color-wheel/)  
[https://www.w3schools.com/colors/colors\_picker.asp?colorhex=F0F8FF](https://www.w3schools.com/colors/colors_picker.asp?colorhex=F0F8FF)  
[https://css-tricks.com/snippets/css/named-colors-and-hex-equivalents/](https://css-tricks.com/snippets/css/named-colors-and-hex-equivalents/)

