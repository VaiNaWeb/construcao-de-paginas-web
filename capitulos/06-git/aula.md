# Começando com Git

### Introdução

Vamos colocar nossa primeira página online, e para isso vamos usar Git, o Github e seu serviço Github Pages como nossa ferramenta. Mas antes, precisamos compreender o que são cada uma dessas ferramentas e como elas funcionam.

### Primeiros comandos com Git

O Git é um sistema de controle de versão e gerenciamento de código fonte desenvolvido por Linus Torvalds, criado inicialmente para o desenvolvimento do Kernel Linux.

Podemos pensar no Git como um fotógrafo de nossas alterações. Ele fica registrando as mudanças feitas em um ou mais arquivos ao longo do tempo. Mas como ele faz isso? Bom... Vamos aprender na prática como isso acontece!

Cada diretório de trabalho do Git tem seu histórico completo e habilidade total de acompanhamento das revisões.

Antes de tudo, precisamos inicializar o Git em nosso projeto. Isso precisa ser feito apenas uma vez no projeto. Precisamos fazer esse passo uma vez por projeto. Navegue até a pasta que você quer começar a rastrear, tenha certeza de que você está dentro da pasta certa e digite o comando:

```text
git init
```

Se você está versionando uma pasta que já tem arquivos dentro dela, ele vai entender que todos esses arquivos fazem parte da sua primeira alteração.

Se você está versionando uma pasta vazia, sugerimos que você crie dentro dela um novo arquivo em branco, esse arquivo vai ser a sua primeira alteração. Ou simplesmente dê inicio ao seu projeto real.

Agora, ainda pensando no git como um fotógrafo de nossas alterações, precisamos dizer a ele quais fotografias queremos que ele nos lembre. Para isso, vamos pedir que ele marque isso como se colocasse um post-it no conjunto de mudanças que fizemos. Fazendo isso estamos solicitando ao git para guardar esse estado de nosso repositório. É como salvar o momento de um jogo no videogame e poder voltar nele ou só lembrar dele depois, sabe?

Mas antes de guardar, é sempre bom ter certeza de qual estado é esse que estamos falando. Quais arquivos foram alterados? Para checar isso, vamos usar uma instrução para que o git nos informe quais são. Usamos o seguinte comando:

```text
git status
```

Agora já sabemos quais arquivos foram alterados! Supondo que esse é mesmo o momento da história do nosso repositório que queremos guardar, usamos agora o seguinte comando para guardar as alterações de um arquivo:

```text
git add nomedoarquivo
```

Se você tiver alterado mais de um arquivo, e não quiser digitar esse comando para cada um deles, você pode usar \* ou . ao invés de especificar os nomes deles. Exemplo:

```text
git add *
```

Dai então podemos fazer mais alterações e adicionar a esse momento usando de novo o git add, ou podemos querer guardar esse momento exato, sem novas alterações. Para isso, vamos criar um commit, o commit é o nome que damos a esses momentos guardados na história do repositório. Cada momento deve ter uma descrição sobre ele também. Para isso usamos o comando:

```text
git commit -m "oi! eu sou o seu primeiro commit!"
```

Você pode alterar o comentário do commit escrevendo outra frase dentro das aspas. Que tal fazer novas alterações e criar mais um commit? Crie um novo arquivo em branco ou altere o conteúdo de arquivos existentes. Depois você pode usar o git add novamente, não esqueça disso, e daí então criar mais um commit com um novo comentário para guardar esse novo momento. Exemplo:

```text
git commit -m "parabénss, mais um commit!"
```

Uma das vantagens em poder guardar esses momentos, digo, commits é que se a gente precisar é possível desfazer as mudanças que fizemos e então o repositório fica igual ao ultimo commit que criamos. Para isso, ao invés de usar o git add, usamos o git checkout:

```text
git checkout nomedoarquivo
```

Se você já tiver usado o git add, isso significa que ele já está na área de seleção já esperando pelo próximo commit, se você fez isso, precisa tirar ele de lá. Para isso você pode usar o comando:

```text
git reset HEAD nomedoarquivo
```

Agora é só usar o git checkout novamente, e prontinho, alterações desfeitas!

Existem vários outros comandos que podemos aprender, você pode ver uma lista com a descrição de mais alguns usando o comando help:

```text
git help
```

### Referências

[https://git-scm.com/](https://git-scm.com/)  
[https://pt.wikipedia.org/wiki/Git](https://pt.wikipedia.org/wiki/Git)  
[https://guides.github.com/introduction/git-handbook/](https://guides.github.com/introduction/git-handbook/)  
[https://github.github.com/training-kit/downloads/pt\_BR/github-git-cheat-sheet/](https://github.github.com/training-kit/downloads/pt_BR/github-git-cheat-sheet/)

