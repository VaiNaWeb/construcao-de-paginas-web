# Tipografia

### Introdução

Há muitas propriedades oferecidas pelo CSS para trabalhar com as palavras, elas se encaixam em duas categorias: propriedades baseadas em fontes e propriedades baseadas em texto. 

A maioria dessas propriedades será precedida com fonte, entenda a fonte como o arquivo da letra, e texto que são as palavras de fato. Vamos conhecer algumas!

### Font Family

A propriedade font-family é usada para declarar qual tipo de letra devem ser usadas para exibir texto. O valor da propriedade font-family pode conter vários nomes de fontes, todos separados por vírgulas.

Funciona assim, primeira fonte declarada, a partir da esquerda, é a escolha principal da fonte. Caso a primeira fonte não esteja disponível, as fontes alternativas são declaradas depois dela em ordem de preferência da esquerda para a direita.

```css
p {
  font-family: Helvetica, Arial, sans-serif;
}
```

### Font Size

A propriedade font-size nos permite definir o tamanho do texto usando alguns valores. Assim como quando falamos em dinheiro precisamos citar a moeda, quando definimos o valor de um font-size usamos algumas unidades de medida. Alguns exemplos são:

#### Pixels

Pixels sao unidades de medida usadas em telas (por exmplo, telas de computadores). Um pixel é equivalente a um ponto na tela do computador (a menor divisão da resulução da sua tela). Um problema do pixel é que não aumenta para leitores com deficiência visual ou se adequa a dispositivos móveis. Exemplo:
```css
p {
  font-size: 16px;
}
```

#### EM
EM é uma unidade escalável para ser usada em documentos web. Um EM é equivalente ao tamanho da fonte atual, ou seja, se o tamanho da fonte do documento é 12pt, 1em é igual a 12pt. EMs são escaláveis por natureza, entao 2em seriam equivalentes a 24pt, 5em seriam iguais a 60pt, etc. EM está se tornando bem popular em documentos online devido à escalabilidade e à sua natureza amigável para dispositivos móveis.
```css
p {
  font-size: 1em;
}
```

#### Porcentagens
A unidade porcentagem é muito parecida com a unidade EM, exceto por algumas diferenças fundamentais. Primeiramente, o tamanho da fonte atual é igual a 100% (ou seja, 12pt é equivalente a 100%). Ao usar a unidade de porcentagem, seu texto permanece totalmente escalável para dispositivos móveis e para acessibilidade. Exemplo:
```css
p {
  font-size: 100%;
}
```

#### Pontos
Pontos são, tradicionalmente, usados em mídia impressa. Um ponto é aproximadamente 352mm. Os pontos são muito parecidos com pixels, pois são unidades de tamanho fixo e não podem ser redimensionados.
```css
p {
  font-size: 12pt;
}
```

### Font Style

A propriedade font-style aceita quatro valores de palavras-chave: normal, italic, oblique e inherit. Destes quatro, os mais utilizados são o itálico, que define o texto para o itálico, e o normal que como o próprio nome sugere, retorna o texto ao seu estilo normal. Exemplo:

```css
p {
  font-style: italic;
}
```

### Font Variant

A propriedade font-variant aceita três valores: normal, small-caps, e inherit. Os valores mais comuns são normal e small-caps. Exemplo:

```css
p {
  font-variant: small-caps;
}
```

### Font Weight

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

### Line Height

A propriedade line-height é responsável por modificar a distância entre duas linhas de texto declaramos usando a propriedade de altura da linha. Exemplo:

```css
p {
  height: 26px;
  line-height: 26px;
}
```

### Text Align

Essa propriedade modifica o alinhamento de uma frase em relação a uma página. Ela aceita os valores left, right, center, e justify. Exemplo:

```css
p {
  text-align: center;
}
```

### Text Transform

Enquanto a propriedade font-variant procura uma variante alternativa de um tipo de letra, a propriedade text-transform alterará o texto. A propriedade text-transform aceita cinco valores: none, capitalize, uppercase, lowercase, e inherit.

Um caso de uso muito comum: se um texto precisa escrito em letras maiúsculas não é recomendando sempre escreve-lo no HTML assim, melhor usar o CSS para isso. Exemplo:

```css
p {
  text-transform: uppercase;
}
```

### Usando fontes seguras

Existem algumas fontes que são comuns em todos os computadores, tablets, smartphones e outros dispositivos compatíveis com os navegadores na web. Como eles foram instalados em todos os dispositivos, podemos usar essas fontes livremente em nossos sites, sabendo que não importa qual dispositivo esteja navegando em nosso site, a fonte irá aparecer corretamente. Exemplos de fontes seguras:

* Arial
* Courier New, Courier
* Garamond
* Georgia
* Lucida Sans Lucida Grande, Lucida
* Palatino Linotype
* Tahoma
* Times New Roman
* Verdana

### Carregando novas fontes

Quando não queremos usar as fontes que vêm por padrão em todos os computadores, podemos também carregar novas fontes e usa-las em nossa página. Existem dois caminhos mais conhecidos para fazer isso, o mais simples, é usando recursos como o [Google Fonts](https://fonts.google.com/).

O Google Fonts é uma biblioteca de fontes licenciadas livres, que nos permite escolher e usar convenientemente as fontes por meio do CSS. Basta escolher a fonte, e o próprio Google Fonts já nos sugere um link com instruções para que possamos importar essa fonte e depois basta selecionar a fonte CSS.

Podemos importar através do HTML:

```markup
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

