# As unidades de medidas CSS 

Há várias unidades de medidas que podemos usar em nossas página. Não existe uma unidade mais correta que a outra, existem unidades diferentes que podem ser usadas em determinado contexto ou situação de forma mais adequada. Não se preocupe, você vai conhecendo eles e descobrindo quais usar. Por enquanto, vamos conhecer as mais usadas!
 
Há medidas absolutas, que são medidas fixas, e que usamos em comparação geralmente ao próprio hardware, essas são indicadas quando você sabe em que aparelhos a sua página vai ser exibida, o que não é muito comum. Há também medidas de distância relativas, que são medidas calculadas em relação a uma outra unidade de medida. Usar unidades de medidas relativas é mais apropriado para se obter ajustes em diferentes tipos de mídia.

## Medidas de distância absolutas
- pt - point: 1/72in;
- px - pixel: 1/96in;

``` css
p { font-size: 14px; }
```

``` css
hr { width: 14pt; } 
```

## Medidas de distância relativas
- em: em relação ao tamanho da fonte do elemento no qual a unidade é declarada;
- rem: em relação ao tamanho da fonte do elemento raiz do documento.
- %: em relação ao tamanho disponível no viewport
- vw: 1% da largura da viewport;
- vh: 1% da altura da viewport;
- vmin: a menor medida entre vw e vh;
- vmax: a maior medida entre vw e vh.

``` css
div { margin: 1.5em; } 
```

``` css
.classe { padding: 90%; }
```

``` css
div { width: 50vw; }
```

## Unidades para ângulos
- deg - grau: um círculo tem 360deg;
- turn - volta: um círculo tem 1turn;

``` css
background-image: linear-gradient( 45deg, white, black );
```

## Unidades de duração
- s - segundo: 1s;
- ms - milissegundo: 1/1000s;
