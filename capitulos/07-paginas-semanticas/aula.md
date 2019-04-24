# Páginas semânticas

## Introdução

Há elementos no HTML que conhecemos como elementos de caixa, ou containers. Usamos eles normalmente para agrupar nossos elementos. Houve uma época em que construíamos essas caixas simplesmente com uma tag chamada `<div>`, e ainda usamos ela eventualmente para caixas que não carregam um sentido.

Com a chegada do HTML5, ganhamos algumas tags com significado semântico, e passamos a usar não somente `div`. Isso foi muito importante para os navegadores e usuários, consequentemente isso facilitou também a nossa vida enquanto desenvolvedor. Agora temos uma tag `<header>` para cabeçalho, uma tag `<footer>` para rodapé e mais algumas:

`<section>` Define uma seção  
`<nav>` Define um menu com links de navegação  
`<article>` Pode definir um artigo, um comentário enviado pelo usuário etc  
`<aside>` Define um conteúdo reservado dentro página.  
`<header>` Define o cabeçalho de uma página ou seção.  
`<footer>` Define o rodapé de uma página ou seção.  
`<main>` Define o conteúdo principal ou importante no documento. Deve existir apenas um.

Na dúvida sobre qual elemento de caixa usar, você deve pensar sobre qual o sentido ou significado dessa caixa em sua página. Exemplo: uma caixa que representa um menu, deve ser definida por um nav. Uma caixa que não representa nenhum sentido, mas precisa ser usada mesmo assim, deveria ser uma div.

## Evoluindo minha página com mais HTML

### Listando coisas

Existem três tipos de listas: as ordenadas, as não ordenadas e as de definições.

#### Ordenadas

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

#### Não ordenadas

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

#### De definição

Neste tipo de lista, os itens são definidos.

```markup
<dl>
    <dt>Caneta</dt>
        <dd>Azul, com tinta</dd>
    <dt>Lápis</dt>
        <dd>De madeira</dd>
</dl>
```

CanetaAzul, com tintaLápisDe madeira

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

