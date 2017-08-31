# Introdução ao modelo flexível de caixas

- Conhecido com Flexbox

- Para entendermos o Flexbox, precisamos compreender alguns elementos como containers e outros como itens desses containers.

- Começamos a usar o Flexbox inserindo  a propriedade <code>display</code> com o valor <code>flex</code> no container.

```css
.container {
  display: flex;
}
```
- Existem propriedades específicas que usamos para container e  outras para os itens. Vejamos:

## Propriedades do container

### <code>flexp-direction</code>
- Valores atribuídos ao <code>flexp-direction</code>:<br> 
  <code>row <i>(padrão)</i></code>: Os itens são posicionados na mesma direção padrão da página.<br>
  <code>row-reverse</code>: Os itens são posicionados na direção inversa ao padrão da página.<br>
  <code>column</code>: Os itens são posicionados de cima para baixo.<br>
  <code>column-reverse</code>: Os itens são posicionados de baixo para cima.<br>

```css
.container {
  display: flex;
  flex-direction: row;
}
```

### <code>justify-content</code>
- Valores atribuídos ao <code>justify-content</code>:<br> 
<code>flex-start <i>(padrão)</i></code>: Os itens são alinhados à esquerda do container.<br>
<code>flex-end</code>: Os itens são alinhados à direita do container.<br>
<code>center</code>: Os itens são alinhados no centro do container.<br>
<code>space-between</code>: Os itens são alinhados com distância igual entre eles.<br>
<code>space-around</code>: Os itens são alinhados com distância igual em torno deles.<br>

```css
.container {
  display: flex;
  justify-content: flex-start;
}
```

### <code>flex-wrap</code>
- Valores atribuídos ao <code>flex-wrap</code>:<br> 
<code>nowrap <i>(padrão)</i></code>: Todos os itens são apertados em uma única linha.<br>
<code>wrap</code>: Os itens são separados em linhas adicionais.<br>
<code>wrap-reverse</code>: Os itens são separados em linhas adicionais em reverso.<br>

```css
.container {
  display: flex;
  flex-wrap: wrap;
}
```

### <code>align-items</code>
- Valores atribuídos ao <code>align-items</code>:<br>
<code>flex-start</code>: Os itens são alinhados na parte de cima do container.<br>
<code>flex-end</code>: Os itens são alinhados na parte de baixo do container.<br>
<code>center</code>: Os itens são alinhados no centro vertical do container.<br>
<code>baseline</code>: Os itens são alinhados na linha da base do container.<br>
<code>stretch <i>(padrão)</i></code>: Os itens são alinhados para preencher o container.<br>

```css
.container {
  display: flex;
  align-items: center;
}
```

### <code>align-content</code>
- Valores atribuídos ao <code>align-content</code>:<br>
<code>flex-start</code>: As linhas são agrupadas no topo do container.<br>
<code>flex-end</code>: As linhas são agrupadas no fundo do container.<br>
<code>center</code>: As linhas são agrupadas no centro vertical do container.<br>
<code>space-between</code>: As linhas são posicionadas com espaço igual entre elas.<br>
<code>space-around</code>: As linhas são posicionadas com espaço igual em torno delas.<br>
<code>stretch <i>(padrão)</i></code>: As linhas são esticadas para preencher o container.<br>

```css
.container {
  display: flex;
  align-content: center;
}
```

## Propriedades dos itens

### <code>order</code>
- Os valores atibuídos ao <code>order</code> são números positivos ou negativos.

```css
.container{
  display:flex;
}
.item {
  order: 1;
}
```

### <code>align-self</code>
- Valores atribuídos ao <code>align-self</code>:<br>
<code>flex-start</code>: O item é alinhado na parte de cima do container.<br>
<code>flex-end</code>: O item é alinhado na parte de baixo do container.<br>
<code>center</code>: O item é alinhado no centro vertical do container.<br>
<code>baseline</code>: O item é alinhado na linha da base do container.<br>
<code>stretch</code>: O item é alinhado para preencher o container.<br>

```css
.container{
  display:flex;
}
.item {
  align-self: center;
}
```
