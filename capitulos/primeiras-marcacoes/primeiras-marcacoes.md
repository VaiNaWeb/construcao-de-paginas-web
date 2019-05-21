# Primeiras marcações

### Introdução

Para estruturar páginas a linguagem HTML usa um conjunto predefinido de regras para identificar os diversos tipos de conteúdos. Usamos as Tags para criar marcações que dizem aos navegadores quais elementos estão presentes na página e como devem ser interpretados.

### Primeiras marcações

Uma tag precisa começar com o sinal de menor &lt; e terminar com o sinal de maior &gt;. Exemplo:

```markup
<p>
```

Embora algumas tags especiais sejam fechadas por padrão, a maior parte delas não é. Logo, ao criar uma tag para abrir uma marcação precisamos também adicionar uma para fecha-la. Para criar uma tag de fechamento, usamos um sinal de barra / depois do sinal de maior. 

Exemplo:

```markup
<p>Olá, eu sou um parágrafo.</p>
```

As tags devem dizer exatamente o que é o conteúdo entre sua tag de abertura e fechamento. Devemos marcar com as tags quais partes do conteúdo são parágrafos, títulos, listas, etc, chamamos isso de Semântica.

### Criando títulos

Existem seis níveis diferentes de títulos para usar em uma imagem. O título `H1` é o mais importante,`h6` é o menos importante. 

Exemplo:

```markup
<h1>Eu sou o título mais importante!</h1>
<h2>Eu sou um pouco menos importante</h2>
<h3>Eu sou um pouco menos importante</h3>
<h4>Eu sou um pouco menos importante</h4>
<h5>Eu sou um pouco menos importante</h5>
<h6>Eu sou o menos importante</h6>
```

### Conectando páginas

Sabemos que nossos sites são conjuntos de páginas conectadas, ou lincadas, umas às outras. Agora vamos compreender melhor como isso acontece. A criação do hiperlink foi uma das responsáveis por tornar a web tão maravilhosa como ela é. Foi assim que conseguimos começar a facilmente conectar páginas. 

Qualquer elemento que aparece entre a abertura e o fechamento de tags é a parte que será um link clicável na página. Exemplo:

```markup
<p>Esse é um exemplo de palavra <a href="http://www.vainaweb.com.br"> clicável </a>.</p>
```

Qualquer coisa mesmo, não somente textos. Nós podemos deixar imagens clicáveis também!

```markup
<a href="http://www.vainaweb.com.br">
    <img src="http://www.vainaweb.com.br/img/vainaweb.svg" alt="logo">
</a>
```

