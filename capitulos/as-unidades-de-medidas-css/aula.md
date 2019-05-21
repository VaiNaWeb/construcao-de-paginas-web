# As unidades de medidas CSS

## Introdução

Existem várias unidades de medidas que podemos usar em nossas páginas. Não existe uma unidade mais correta que a outra, existem unidades diferentes que podem ser usadas em determinado contexto ou situação de forma mais adequada. Não se preocupe,  aos poucos você vai descobrindo quais usar. Por enquanto, vamos conhecer as mais usadas!

Há medidas absolutas, que são medidas fixas, e que usamos em comparação geralmente ao próprio hardware, essas são indicadas quando você sabe em que aparelhos a sua página vai ser exibida, o que não é muito comum. Há também medidas de distância relativas, que são medidas calculadas em relação a uma outra unidade de medida. Usar unidades de medidas relativas é mais apropriado para se obter ajustes em diferentes tipos de mídia.

### Medidas de distância absolutas

* cm - centimeters\(centímetros\);
* mm - millimeters\(milímetros\);
* in - inches\(polegadas\) \(1in = 96px = 2.54cm\);
* px - pixels \(1px = 1/96th of 1in\);
* pt - points\(pontos \(1pt = 1/72 of 1in\);
* pc - picas\(paica\) \(1pc = 12 pt\);

```css
p { font-size: 14px; }
```

```css
hr { width: 14pt; }
```

### Medidas de distância relativas

* em: em relação ao tamanho da fonte do elemento no qual a unidade é declarada
* rem: em relação ao tamanho da fonte do elemento raiz do documento
* %: em relação ao tamanho disponível na tela
* vw: largura da tela
* vh: altura da tela
* vmin: a menor medida entre vw e vh
* vmax: a maior medida entre vw e vh

Exemplo de texto usando em:

```css
div { margin: 1.5em; }
```

Exemplo de altura ocupando a tela inteira:

```css
div { height: 100vh; }
```

Exemplo de largura ocupando metade da tela:

```css
div { width: 50vw; }
```

### Unidades para ângulos

* deg - grau: um círculo tem 360deg;
* rad - radiano: um círculo tem 2𝛑rad;
* turn - volta: um círculo tem 1turn;

```css
background-image: linear-gradient( 45deg, white, black );
```

### Unidades de duração

* s - segundo: 1s;
* ms - milissegundo: 1/1000s;

```css
div {
     transition: background-color 1s;
}
```

### Referências

[https://css-tricks.com/the-lengths-of-css/](https://css-tricks.com/the-lengths-of-css/)  
[https://css-tricks.com/fun-viewport-units/](https://css-tricks.com/fun-viewport-units/)



