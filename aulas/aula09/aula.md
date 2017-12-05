# As cores na web

Aprenderemos como colocar cores na web. Há alguns [sistemas de cores](https://tableless.com.br/sobre-cor-e-webdesign/) que precisamos conhecer para entender como adiciona-las em nossas folhas de estilo.

## RGB

Monitores são pretos e iluminados por vários pontinhos de luz. Vamos somando pontinhos vermelhos, verdes, e azuis até chegar na cor. A cor RGB É formada por três pares de números, vermelho, verde e azul, formados por três dígitos. Quanto mais alto o número mais clara é a cor.
```css
p {
    color: rgb(0, 0, 255);
}
```
Eventualmente podemos precisar alterar a opacidade da cor, deixando ela mais transparente ou mais opaca. Para isso, podemos usar um quarto número, que representa o canal alpha da cor.
```css
p {
    color: rgb(0, 0, 255, 0.5);
}
```
## Hexadecimais

Compostos por uma combinação de três conjuntos de pares formados a partir de número e letras de A a F. Quanto mais alto o número mais clara é a cor.

Cada par é responsável por uma cor, assim como o RGB, Vermelho, verde e azul. Ou seja #ff0000 é o vermelho, e o #00ff00 é o verde e #0000ff é o azul.

```css
p {
    color: #ff0000;
}
```
## Ferramentas legais

http://lokeshdhakar.com/projects/color-thief/<br>
http://moviesincolor.com/<br>
https://color.adobe.com/pt/create/color-wheel/<br>
https://www.w3schools.com/colors/colors_picker.asp?colorhex=F0F8FF<br>

# Tipografia

Temos muitas propriedades oferecidas pelo CSS para trabalhar com as palavras, elas se encaixam em duas categorias: propriedades baseadas em fontes e propriedades baseadas em texto. A maioria dessas propriedades será precedida com fonte, entenda a fonte como o arquivo da letra, e texto que são as palavras de fato. 

## Família de fontes

A propriedade font-family é usada para declarar qual tipo de letra devem ser usadas para exibir texto. O valor da propriedade font-family pode conter vários nomes de fontes, todos separados por vírgulas.

Funciona assim, primeira fonte declarada, a partir da esquerda, é a escolha principal da fonte. Caso a primeira fonte não esteja disponível, as fontes alternativas são declaradas depois dela em ordem de preferência da esquerda para a direita.
```css
body {
  font-family: Helvetica, Arial, sans-serif;
}
```
## Font Size

A propriedade font-size nos permite definir o tamanho do texto usando alguns valores. Assim como quando falamos em dinheiro precisamos citar a moeda, quando definimos o valor de um font-size usamos algumas unidades de medida, por exemplo: pixels, em, porcentagens, pontos, etc. Exemplo com pixel:
```css
body {
  font-size: 16px;
}
```

## Font Style

A propriedade font-style aceita quatro valores de palavras-chave: normal, italic, oblique e inherit. Destes quatro, os mais utilizados são o itálico, que define o texto para o itálico, e o normal que como o próprio nome sugere, retorna o texto ao seu estilo normal. Exemplo:
```css
body {
  font-style: italic;
}
```

## Font Variant

## Font Weight 

## Line Height 

## Shorthand Font Properties

## Text Align

## Text Decoration 

## Text Indent

## Text Shadow

## Letter Spacing
  
## Word Spacing

## Using Web-Safe Fonts

## Embedding Web Fonts
