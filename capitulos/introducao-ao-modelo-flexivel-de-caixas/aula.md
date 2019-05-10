# Introdução ao modelo flexível de caixas

### Introdução

Existe um conjunto de propriedades em CSS criado com o objetivo de tornar mais flexível o alinhamento e espaçamento de caixas, chamamos esse conjunto de Flexbox.

O Flexbox nos dá o poder de determinar melhor a altura das nossas seções, centralizar nosso conteúdo, dividir nossas colunas, ou seja, nos permite montar layouts de forma mais flexível, e claro, mais prática.

### Ahh as caixas...

Desde o início das nossas aulas, estamos nos referindo aos elementos como caixas dentro de caixas. Para entender Flexbox, precisamos compreender que alguns elementos podem ser vistos como caixas, ou containers, e outros como itens desses containers.

Para começar a usar essas propriedades, adicionamos ao elemento container a propriedade `display` e atribuimos a ela o valor `flex`.

```css
.container {
    display: flex;
}
```

### Linhas e colunas

Com o flexbox é fácil criar linhas ou colunas, usamos a propriedade `flex-direction`. Como valor podemos usar `row`, `row-reverse`, `column`, e `column-reverse`. Row alinha os elementos de forma horizontal, ou seja, em linha.

`row`: Os itens são posicionados na mesma direção padrão da página.  
`row-reverse`: Os itens são posicionados na direção inversa ao padrão da página.  
`column`: Os itens são posicionados de cima para baixo.  
`column-reverse`: Os itens são posicionados de baixo para cima.

```css
.container {
    display: flex;
    flex-direction: row;
}
```

### Distribuição de espaço

Podemos definir também a distribuição de espaços entre um elemento e outro. Para isso usamos a propriedade `justify-content`. Essa propriedade aceita os valores `flex-start`, `flex-end`, `center`, `space-between`, `space-around`.

`flex-start:` Os itens são alinhados à esquerda do container.  
`flex-end:` Os itens são alinhados à direita do container.  
`center:` Os itens são alinhados no centro do container.  
`space-between`: Os itens são alinhados com distância igual entre eles.  
`space-around`: Os itens são alinhados com distância igual em torno deles.

```css
.container {
    display: flex;
    justify-content: flex-start;
}
```

### Espalhando elementos em linhas

Eventualmente nossos elementos podem ocupar uma única linha em um container. Outras vezes podemos achar melhor que os elementos possam ser espalhados em linhas adicionais. Definimos esse comportamento usando a propriedade `flex-wrap`. Podemos usar os valores `nowrap`, `wrap`, ou `wrap-reverse`.

`nowrap`: Todos os itens são apertados em uma única linha.  
`wrap:` Os itens são separados em linhas adicionais.  
`wrap-reverse:` Os itens são separados em linhas adicionais em reverso.

```css
.container {
    display: flex;
    flex-wrap: wrap;
}
```

### Alinhando itens

Podemos definir o alinhamento dos elementos em relação à altura da página ou container. Usamos a propriedade `align-items`, que pode receber os valores `flex-start`, `flex-end`, `center`, `baseline`, e `stretch`.

`flex-start:` Os itens são alinhados na parte de cima do container.  
`flex-end:` Os itens são alinhados na parte de baixo do container.  
`center:` Os itens são alinhados no centro vertical do container.  
`baseline:` Os itens são alinhados na linha da base do container.  
`stretch:` Os itens são alinhados para preencher o container.

```css
.container {
    display: flex;
    align-items: center;
}
```

### Alinhando múltiplas linhas

Em containers com múltiplas linhas podemos usar o `align-content`. Enquanto align-items determina como as linhas são alinhadas dentro do container como um todo, align-content determina como múltiplas linhas devem ser espaçadas uma das outras. Essa propriedade pode receber os seguintes valores:

`flex-start`: As linhas são agrupadas no topo do container.  
`flex-end`: As linhas são agrupadas no fundo do container.  
`center`: As linhas são agrupadas no centro vertical do container.  
`space-between`: As linhas são posicionadas com espaço igual entre elas.  
`space-around`: As linhas são posicionadas com espaço igual em torno delas.  
`stretch`: As linhas são esticadas para preencher o container.

```css
.container {
    display: flex;
    align-content: center;
}
```

### Mudando a ordem dos itens

Se quisermos mudar a ordem do item podemos adicionar a propriedade `order` no item.

```css
.item {
    display: flex;
    order: 1;
}
```

### Alinhando um item

Quando necessário, se precisarmos alterar o alinhamento de um item, podemos usar a propriedade `align-self` então ele pode mudar o comportamento de alinhamento dele mesmo. Assim como align-items, essa propriedade pode receber os valores `flex-start`, `flex-end`, `center`, `baseline`, e `stretch`.

`flex-start:` O item é alinhado na parte de cima do container.  
`flex-end:` O item é alinhado na parte de baixo do container.  
`center:` O item é alinhado no centro vertical do container.  
`baseline:` O item é alinhado na linha da base do container.  
`stretch:` O item é alinhado para preencher o container.

```css
.item {
    display: flex;
    align-self: center;
}
```

