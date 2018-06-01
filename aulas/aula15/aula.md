# Introdução ao modelo flexível de caixas

Existe um conjunto de propriedades em CSS criado com o objetivo de tornar mais flexível o alinhamento e espaçamento de caixas, chamamos esse conjunto de Flexbox.

O Flexbox nos dá o poder de determinar melhor a altura das nossas seções, centralizar nosso conteúdo, dividir nossas colunas, ou seja, nos permite montar layouts de forma mais flexível, e claro, mais prática.

## Ahh as caixas...

Desde o início das nossas aulas, estamos nos referindo aos elementos como caixas dentro de caixas. Para entender Flexbox, precisamos compreender que alguns elementos podem ser vistos como caixas, ou containers, e outros como itens desses containers.

Para começar a usar essas propriedades, adicionamos ao elemento container a propriedade <code>display</code> e atribuimos a ela o valor <code>flex</code>.

```css
.container {
	display: flex;
}
```
## Linhas e colunas

Com o flexbox é fácil criar linhas ou colunas, usamos a propriedade <code>flex-direction</code>. Como valor podemos usar <code>row</code>, <code>row-reverse</code>, <code>column</code>, e <code>column-reverse</code>. Row alinha os elementos de forma horizontal, ou seja, em linha. 

<code>row</code>: Os itens são posicionados na mesma direção padrão da página.<br>
<code>row-reverse</code>: Os itens são posicionados na direção inversa ao padrão da página.<br>
<code>column</code>: Os itens são posicionados de cima para baixo.<br>
<code>column-reverse</code>: Os itens são posicionados de baixo para cima.<br>

```css
.container {
	display: flex;
	flex-direction: row;
}
```
## Distribuição de espaço

Podemos definir também a distribuição de espaços entre um elemento e outro. Para isso usamos a propriedade <code>justify-content</code>. Essa propriedade aceita os valores <code>flex-start</code>, <code>flex-end</code>, <code>center</code>, <code>space-between</code>, <code>space-around</code>. 

<code>flex-start:</code> Os itens são alinhados à esquerda do container.<br>
<code>flex-end:</code> Os itens são alinhados à direita do container.<br>
<code>center:</code> Os itens são alinhados no centro do container.<br>
<code>space-between</code>: Os itens são alinhados com distância igual entre eles.<br>
<code>space-around</code>: Os itens são alinhados com distância igual em torno deles.<br>

```css
.container {
	display: flex;
	justify-content: flex-start;
}
```

## Espalhando elementos em linhas

Eventualmente nossos elementos podem ocupar uma única linha em um container. Outras vezes podemos achar melhor que os elementos possam ser espalhados em linhas adicionais. Definimos esse comportamento usando a propriedade <code>flex-wrap</code>. Podemos usar os valores <code>nowrap</code>, <code>wrap</code>, ou <code>wrap-reverse</code>.

<code>nowrap</code>: Todos os itens são apertados em uma única linha.<br>
<code>wrap:</code> Os itens são separados em linhas adicionais.<br>
<code>wrap-reverse:</code> Os itens são separados em linhas adicionais em reverso.<br>

```css
.container {
	display: flex;
	flex-wrap: wrap;
}
```

## Alinhando itens

Podemos definir o alinhamento dos elementos em relação à altura da página ou container. Usamos a propriedade <code>align-items</code>, que pode receber os valores <code>flex-start</code>, <code>flex-end</code>, <code>center</code>, <code>baseline</code>, e <code>stretch</code>.

<code>flex-start:</code> Os itens são alinhados na parte de cima do container.<br>
<code>flex-end:</code> Os itens são alinhados na parte de baixo do container.<br>
<code>center:</code> Os itens são alinhados no centro vertical do container.<br>
<code>baseline:</code> Os itens são alinhados na linha da base do container.<br>
<code>stretch:</code> Os itens são alinhados para preencher o container.<br>

```css
.container {
	display: flex;
	align-items: center;
}
```

## Alinhando multiplas linhas

Em containers com múltiplas linhas podemos usar o <code>align-content</code>. Enquanto align-items determina como as linhas são alinhadas dentro do container como um todo, align-content determina como múltiplas linhas devem ser espaçadas uma das outras. Essa propriedade pode receber os seguintes valores:

<code>flex-start</code>: As linhas são agrupadas no topo do container.<br>
<code>flex-end</code>: As linhas são agrupadas no fundo do container.<br>
<code>center</code>: As linhas são agrupadas no centro vertical do container.<br>
<code>space-between</code>: As linhas são posicionadas com espaço igual entre elas.<br>
<code>space-around</code>: As linhas são posicionadas com espaço igual em torno delas.<br>
<code>stretch</code>: As linhas são esticadas para preencher o container.<br>

```css
.container {
	display: flex;
	align-content: center;
}
```

## Mudando a ordem dos itens

Se quisermos mudar a ordem do item podemos adicionar a propriedade <code>order</code> no item. 

```css
.item {
	display: flex;
	order: 1;
}
```

## Alinhando um item

Quando necessário, se precisarmos alterar o alinhamento de um item, podemos usar a propriedade <code>align-self</code> então ele pode mudar o comportamento de alinhamento dele mesmo. Assim como align-items, essa propriedade pode receber os valores <code>flex-start</code>, <code>flex-end</code>, <code>center</code>, <code>baseline</code>, e <code>stretch</code>.

<code>flex-start:</code> O item é alinhado na parte de cima do container.<br>
<code>flex-end:</code> O item é alinhado na parte de baixo do container.<br>
<code>center:</code> O item é alinhado no centro vertical do container.<br>
<code>baseline:</code> O item é alinhado na linha da base do container.<br>
<code>stretch:</code> O item é alinhado para preencher o container.<br>

```css
.item {
	display: flex;
	align-self: center;
}
```