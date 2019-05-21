# Estruturando páginas

### Introdução

Agora que já sabemos como criar marcações e entendemos como elas funcionam, vamos aprender novas marcações para criar a estrutura completa de uma página.

### Estrutura básica

Há algumas tags principais que compõem uma página padrão. Toda página na web tem uma tag html, head e body. A tag `html` indica elementos em html, dentro dela temos `<head>`, que significa cabeça, e `<body>`, que significa corpo.

Fazendo uma analogia ao corpo humano, na cabeça temos as coisas que não vemos, coisas que pensamos e que são importantes para nosso funcionamento. Mas as coisas do nosso corpo são as partes de nós que podem ser vistas. Assim é no HTML, as coisas que ficam na `head` são importantes, mas não são exibidas no navegador quando a página é carregada.  A parte que queremos exibir e o nosso conteúdo que deve ficar na `body`.

Um exemplo de elemento importante mas não precisa ser visto diretamente na página é o `title`. Veremos outros no decorrer deste módulo.

```markup
<html>
    <head>
        <title>Título</title>
    </head>
    <body>
        <p>Olá mundo!</p>
    </body>
</html>
```

Há vários elementos diferentes, continue conhecendo mais alguns!

### Elementos aninhados

Nossa estrutura HTML contém vários elementos diferentes e alguns elementos até estão dentro de outros elementos, como se guardássemos uma caixa dentro de outra caixa e dentro dela colocássemos outra caixa, e outra caixa... Confuso, não é?

Imaginar a cena das caixas já pode ter sido confuso para muita gente, assim como para o navegador diante de elementos dispostos dessa forma. Para que isso não aconteça, nós aninhamos nossos elementos, ou seja, usamos esses espaçamentos nas linhas para indicar que um elemento está dentro de outro. Exemplo:

```markup
<section>
    <p>Olá, eu sou um parágrafo.</p> 
</section>
```

### Listando coisas

#### Listas Ordenadas

Assim como o nome parece sugerir, são listas em que a ordem dos itens importa, e eles podem ser enumerados.

```markup
<ol>
    <li>Caneta</li>
    <li>Lápis</li>
    <li>Borracha</li>
    <li>Tesoura</li>
    <li>Papel</li>
</ol>
```

1. Caneta
2. Lápis
3. Borracha
4. Tesoura
5. Papel

#### Listas não ordenadas

Nesta, os itens não são enumerados e podem estar acompanhados apenas de um símbolo.

```markup
<ul>
    <li>Caneta</li>
    <li>Lápis</li>
    <li>Borracha</li>
    <li>Tesoura</li>
    <li>Papel</li>
</ul>
```

* Caneta
* Lápis
* Borracha
* Tesoura
* Papel

### Criando tabelas

Criamos uma tabela com a tag `<table>` uma linha de Table Row, ou `<tr>`. Cada célula de dados será uma Table Data, ou `<td>` podemos, se nececessário, adicionar o atributo rowspan, que vai criar uma expansão de linha nas células. Podemos também usar o atributo colspan e teremos uma expansão de coluna nas células.

```markup
<table>
  <tr>
    <th>Nome</th>
    <th>Sobre</th>
    <th>Cidade</th>
  </tr>
  <tr>
    <td>Maria</td>
    <td>Gosta de cachorros</td>
    <td>Rio de Janeiro</td>
  </tr>
  <tr>
    <td>Rosa</td>
    <td>Solta pipa com os irmãos</td>
    <td>Brasília</td>
  </tr>
  <tr>
    <td>João</td>
    <td>Adora gatos</td>
    <td>Recife</td>
  </tr>
  <tr>
    <td>Ana</td>
    <td>Gosta de árvores</td>
    <td>São Paulo</td>
  </tr>    
</table>
```

| Nome | Sobre | Cidade |
| :--- | :--- | :--- |
| Maria | Gosta de cachorros | Rio de Janeiro |
| Rosa | Solta pipa com os irmãos | Brasília |
| João | Adora gatos | Recife |
| Ana | Gosta de árvores | São Paulo |

### Referências

* [HTML Atributes - Mozilla](https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes)
* [O que está na head? - Mozilla](https://developer.mozilla.org/pt-BR/docs/Aprender/HTML/Introducao_ao_HTML/The_head_metadata_in_HTML)
* [Fundamentos do texto em HTML - Mozilla](https://developer.mozilla.org/pt-BR/docs/Aprender/HTML/Introducao_ao_HTML/Fundamentos_textuais_HTML)
* [MarketSheet.io](https://marksheet.io/)

