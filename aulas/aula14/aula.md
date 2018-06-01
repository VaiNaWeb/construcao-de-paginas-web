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

Temos muitas propriedades oferecidas pelo CSS para trabalhar com as palavras, elas se encaixam em duas categorias: propriedades baseadas em fontes e propriedades baseadas em texto. A maioria dessas propriedades será precedida com fonte, entenda a fonte como o arquivo da letra, e texto que são as palavras de fato. Vamos conhecer algumas!

## Font Family 

A propriedade font-family é usada para declarar qual tipo de letra devem ser usadas para exibir texto. O valor da propriedade font-family pode conter vários nomes de fontes, todos separados por vírgulas.

Funciona assim, primeira fonte declarada, a partir da esquerda, é a escolha principal da fonte. Caso a primeira fonte não esteja disponível, as fontes alternativas são declaradas depois dela em ordem de preferência da esquerda para a direita.
```css
p {
  font-family: Helvetica, Arial, sans-serif;
}
```
## Font Size

A propriedade font-size nos permite definir o tamanho do texto usando alguns valores. Assim como quando falamos em dinheiro precisamos citar a moeda, quando definimos o valor de um font-size usamos algumas unidades de medida, por exemplo: pixels, em, porcentagens, pontos, etc. Exemplo com pixel:
```css
p {
  font-size: 16px;
}
```

## Font Style

A propriedade font-style aceita quatro valores de palavras-chave: normal, italic, oblique e inherit. Destes quatro, os mais utilizados são o itálico, que define o texto para o itálico, e o normal que como o próprio nome sugere, retorna o texto ao seu estilo normal. Exemplo:
```css
p {
  font-style: italic;
}
```
## Font Variant

A propriedade font-variant aceita três valores:  normal, small-caps, e inherit. Os valores mais comuns são normal e small-caps. Exemplo:
```css
p {
  font-variant: small-caps;
}
```
## Font Weight 

Podemos definir um texto em negrito ou alterar o peso específico de um tipo de letra. Para esses casos, usaremos a propriedade font-weight. A propriedade font-weight aceita valores de palavra-chave ou numéricos.

Os valores mais usados são o normal e o bold para mudar o texto do normal para o negrito. Podemos usar também um valor numérico para mais variações. Exemplo:
```css
p {
  font-weight: bold;
}
```
Exemplo usando valor numérico:
```css
p {
  font-weight: 800;
}
```
## Line Height

A propriedade line-height é responsável por modificar a distância entre duas linhas de texto declaramos usando a propriedade de altura da linha. Exemplo:
```css
p {
  height: 26px;
  line-height: 26px;
}
```
## Text Align

Essa propriedade modifica o alinhamento de uma frase em relação a uma página. Ela aceita os valores left, right, center, e justify. Exemplo:
```css
p {
  text-align: center;
}
```

## Text Transform

Enquanto a propriedade font-variant procura uma variante alternativa de um tipo de letra, a propriedade text-transform alterará o texto. A propriedade text-transform aceita cinco valores: none, capitalize, uppercase, lowercase, e inherit. 

Um caso de uso muito comum: se um texto precisa escrito em letras maiúsculas não é recomendando sempre escreve-lo no HTML assim,  melhor usar o CSS para isso. Exemplo:
```css
p {
  text-transform: uppercase;
}
```

## Usando fontes seguras

Existem algumas fontes que são comuns em todos os computadores, tablets, smartphones e outros dispositivos compatíveis com os navegadores na web. Como eles foram instalados em todos os dispositivos, podemos usar essas fontes livremente em nossos sites, sabendo que não importa qual dispositivo esteja navegando em nosso site, a fonte irá aparecer corretamente. Exemplos de fontes seguras:

- Arial
- Courier New, Courier
- Garamond
- Georgia
- Lucida Sans Lucida Grande, Lucida
- Palatino Linotype
- Tahoma
- Times New Roman
- Verdana

## Carregando novas fontes

Quando não queremos usar as fontes que vêm por padrão em todos os computadores, podemos também carregar novas fontes e usa-las em nossa página. Existem dois caminhos mais conhecidos para fazer isso, o mais simples, é usando recursos como o [Google Fonts](https://fonts.google.com/).

O Google Fonts é uma biblioteca de fontes licenciadas livres, que nos permite escolher e usar convenientemente as fontes por meio do CSS. Basta escolher a fonte, e o próprio Google Fonts já nos sugere um link com instruções para que possamos importar essa fonte e depois basta selecionar a fonte CSS. 

Podemos importar através do HTML:

```html
<head>
    <link href="https://fonts.googleapis.com/css?family=Abril+Fatface" rel="stylesheet">
</head>
```
Ou podemos importar através do CSS

```css
@import url('https://fonts.googleapis.com/css?family=Abril+Fatface');
```
Depois basta selecionarmos a fonte onde queremos usa-la:

```css
@import url('https://fonts.googleapis.com/css?family=Abril+Fatface');

body {
  font-family: 'Abril Fatface', cursive;
}
```
Uma outra forma um pouco mais complexa mas eventualmente necessária é carregando uma fonte adicionado o próprio arquivo em nosso projeto. 

Usamos o @font-face para identificar o nome da nossa fonte, através da propriedade font-family, bem como a fonte de nossa fonte através do arquivo, usando a propriedade src. A partir daí, podemos usar essa fonte incluindo seu nome dentro como valor em uma font-family, como já aprendemos anteriormente.

```css
@font-face {
  font-family: 'Exemplo';
  src: url('Exemplo') format("woff");
}

body {
  font-family: 'Exemplo';
}
```
É recomendável nesse caso, adicionarmos vários formatos diferentes de fontes, pois há navegadores que suportam uns e outros não, isso pode trazer uma dor de cabeça. Existem algumas ferramentas que nos ajudam nessa conversão, como a [transfonter](https://transfonter.org/) por exemplo.

```css
@font-face {
	font-family: 'Exemplo';
	src: url('Exemplo.eot');
	src: url('Exemplo.eot?#iefix') format('embedded-opentype'),
		 url('Exemplo.woff2') format('woff2'),
		 url('Exemplo.woff') format('woff'),
		 url('Exemplo.ttf') format('truetype');
}

body {
  font-family: 'Exemplo';
}
```
