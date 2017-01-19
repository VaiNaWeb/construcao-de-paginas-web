#Posicionamento de elementos com CSS

Já aprendemos sobre tamanho, preenchimento, espaçamento e mais algumas propriedades que influem em nossas caixas, agora vamos aprender como posiciona-las.

Em CSS temos a propriedade position, que pode receber alguns valores diferentes, cada um com seu comportamento. O valor padrão dessa propriedade, e que podemos mudar, é o static. Podemos usar os valores static, absolute, relative e fixed.

##Static

O valor static não se posiciona de forma especial, ou seja, dizer que o elemento tem valor estático significa dizer que ele não tem ainda uma posição definida. 

```css
.elemento {
  position: static;
}
```
##Relative

Você pode imaginar que no navegador, há um sistema de coordenadas, e temos que adicionar propriedades extras junto ao position para posicionar o elemento nesse sistema. As propriedades extras que usamos são: top, right, bottom, e left. O position com valor relative posiciona o elemento em relação a si mesmo, e faz esse cálculo a partir do seu canto superior esquerdo.

```css
.elemento {
  position: relative;
}
```
```css
.elemento {
  position: relative;
  top: 20px;
  left: 20px;
}
```

##Absolute

Assim como o valor relative, o absolute precisa dessas propriedades extras de coordenadas. Porém diferente do position relative, o elemento com valor absolute não se posiciona em relação a si mesmo, mas a outros elementos, como seu elemento pai, ou, se o elemento pai não tiver seu position definido, ele usa como referencia o próprio body da página.
```css
.elemento {
  position: absolute;
  top: 20px;
  left: 20px;
}
```
##Fixed

O valor fixed, como o próprio nome sugere se posiciona de forma fixa na página, isso significa que ele sempre ficará no mesmo lugar ainda que rolemos a página. Assim como o relative, e absolute, as propriedades top, right, bottom e left também podem ser utilizadas.
```css
.elemento {
  position: fixed;
  top: 20px;
  left: 20px;
}
```
