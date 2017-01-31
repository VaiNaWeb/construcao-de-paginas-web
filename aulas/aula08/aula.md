#Introdução ao modelo flexível de caixas

Existe um conjunto de propriedades em CSS criado com o objetivo de tornar mais flexível o alinhamento e espaçamento de caixas, chamamos esse conjunto de Flexbox.

O Flexbox nos dá o poder de determinar melhor a altura das nossas seções, centralizar nosso conteúdo, dividir nossas colunas, ou seja, nos permite montar layouts de forma mais flexível, e claro, mais prática.

##Ahh as caixas...

Desde o início das nossas aulas, estamos nos referindo aos elementos como caixas dentro de caixas. Para entender Flexbox, precisamos compreender que alguns elementos podem ser vistos como caixas, ou containers, e outros como itens desses containers.

Para começar a usar essas propriedades, adicionamos ao elemento container a propriedade <code>display</code> e atribuimos a ela o valor <code>flex</code>.

```css
.container {
	display: flex;
}

```
##Linhas e colunas

Com o flexbox é fácil criar linhas ou colunas, usamos a propriedade <code>flex-direction</code>. Como valor podemos usar <code>row</code>, <code>row-reverse</code>, <code>column</code>, e <code>column-reverse</code>. Row alinha os elementos de forma horizontal, ou seja, em linha. 

row: Os itens são posicionados na mesma direção padrão da página.
row-reverse: Os itens são posicionados na direção inversa ao padrão da página.
column: Os itens são posicionados de cima para baixo.
column-reverse: Os itens são posicionados de baixo para cima.

```css
.container {
	display: flex;
	flex-direction: row;
}

```
##Distribuição de espaço

Podemos definir também a distribuição de espaços entre um elemento e outro. Para isso usamos a propriedade <code>justify-content</code>. Essa propriedade aceita os valores <code>flex-start</code>, <code>flex-end</code>, <code>center</code>, <code>space-between</code>, <code>space-around</code>. 

flex-start: Itens se alinham à esquerda do container.
flex-end: Itens se alinham à direita do container.
center: Itens se alinham no centro do container.
space-between: Itens se alinham com distância igual entre eles.
space-around: Itens se alinham com distância igual em torno deles.





