# Git

Vamos colocar nossa primeira página online, e para isso vamos usar Git, o Github e seu serviço Github Pages como nossa ferramenta. Mas antes, precisamos compreender o que são cada uma dessas ferramentas e como elas funcionam.

Antes de tudo, precisamos [versionar](http://rogerdudler.github.io/git-guide/index.pt_BR.html) nossos arquivos com o Git. Um sistema de controle de versão e gerenciamento de código fonte. Foi desenvolvido por Linus Torvalds, criado inicialmente para o desenvolvimento do Kernel Linux, e é ainda hoje muito usado em diferentes projetos digitais no mundo inteiro.

Cada projeto que o Git acompanha é um repositório com um histórico completo e habilidade total de acompanhamento das revisões. Vamos aprender algumas instruções para acompanhar essas revisões.

## Primeiros comandos

Podemos pensar no Git como um fotografo de nossas alterações. Ele fica fotografando as alterações que acontecem dentro da nossa pasta, para nos dar o poder de criar versões de nossos arquivos. Mas como ele faz isso? Bom... Vamos aprender na prática como isso acontece! Weeee!

Antes de tudo, precisamos inicializar o repositório git em nossa pasta. Só precisamos fazer esse passo uma vez por projeto. Para fazer isso, tenha certeza de que você está dentro da pasta que você quer inicializar e digite o comando:

```
git init
```

Prontinho, o Git está pronto para nos ajudar a controlar as alterações para todos os arquivos e pastas neste diretório em que solicitamos.

Se você está versionando uma pasta que já tem arquivos dentro dela, ele vai entender que todos esses arquivos fazem parte da sua primeira alteração. Se você está versionando uma pasta vazia, sugerimos que você crie dentro dela um novo arquivo em branco, esse arquivo vai ser a sua primeira alteração.

Agora, ainda pensando no git como um fotógrafo de nossas alterações, precisamos dizer a ele quais fotografias queremos que ele nos lembre. Para isso, vamos pedir que ele marque isso como se colocasse um post-it no conjunto de mudanças que fizemos. Fazendo isso estamos solicitando ao git para guardar esse estado de nosso repositório. É como salvar o momento de um jogo no videogame e poder voltar nele ou só lembrar dele depois, sabe?

Mas antes de guardar, é sempre bom ter certeza de qual estado é esse que estamos falando. Quais arquivos foram alterados? Para checar isso, vamos usar uma instrução para que o git nos informe quais são. Usamos o seguinte comando:

```
git status
```

Agora já sabemos quais arquivos foram alterados! Supondo que esse é mesmo o momento da história do nosso repositório que queremos guardar, usamos agora o seguinte comando para guardar as alterações de um arquivo:

```
git add nomedoarquivo
```

Se você tiver alterado mais de um arquivo, e não quiser digitar esse comando para cada um deles, você pode usar * ou . ao invés de especificar os nomes deles. Exemplo:

```
git add *
```

Dai então podemos fazer mais alterações e adicionar a esse momento usando de novo o git add, ou podemos querer guardar esse momento exato, sem novas alterações. Para isso, vamos criar um commit, o commit é o nome que damos a esses momentos guardados na história do repositório. Cada momento deve ter uma descrição sobre ele também. Para isso usamos o comando:

```
git commit -m "oi! eu sou o seu primeiro commit!"
```

Você pode alterar o comentário do commit escrevendo outra frase dentro das aspas. Que tal fazer novas alterações e criar mais um commit? Crie um novo arquivo em branco ou altere o conteúdo de arquivos existentes. Depois você pode usar o git add novamente, não esqueça disso, e daí então criar mais um commit com um novo comentário para guardar esse novo momento. Exemplo:

```
git commit -m "parabénss, mais um commit!"
```

Uma das vantagens em poder guardar esses momentos, digo, commits é que se a gente precisar é possível desfazer as mudanças que fizemos e então o repositório fica igual ao ultimo commit que criamos. Para isso, ao invés de usar o git add, usamos o git checkout:

```
git checkout nomedoarquivo
```

Se você já tiver usado o git add, isso significa que ele já está na área de seleção já esperando pelo próximo commit, se você fez isso, precisa tirar ele de lá. Para isso você pode usar o comando:

```
git reset HEAD nomedoarquivo
```

Agora é só usar o git checkout novamente, e prontinho, alterações desfeitas!

Existem vários outros comandos que podemos aprender, você pode ver uma lista com a descrição de mais alguns usando o comando help:

```
git help
```

# Github

Vimos anteriormente que nossos arquivos podem ser versionados com o Git, depois guardados no Github, e então hospedados no Github Pages para ter nossas páginas online.


Depois precisamos armazenar nosso projeto no Github. Uma plataforma social através da qual milhares de pessoas constroem códigos, entre outras coisas, de forma colaborativa, aberta e gratuita. O Github oferece um espaço para armazenar pastas e arquivos com seu conteúdo versionado através do Git.

>"O Github, é na verdade uma rede social ou uma fábrica social de software, que desenvolve e promove milhares de códigos fontes pré armazenados, para as mais diversas finalidades." Wikipedia

Então já podemos usar o [Github Pages](https://tableless.com.br/criando-paginas-web-para-seus-repositorios-com-o-github-pages/) para colocar nossa página online. Ele é um serviço oferecido pelo Github, que permite a criação de páginas na web a partir de projetos que foram armazenados nele.

### Subindo nossos arquivos para o Github

Agora que já conhecemos os comandos mais básicos no Git, queremos que nossos arquivos sejam armazenados não somente no nosso computador, mas também no Github!

Nossa pasta já existe no computador, mas dentro do Github ainda não. Então, vamos abrir o site e criar um repositório vazio dentro dele. Ainda usando o git, precisamos dizer ao Github que nossa pasta e seus commits existem na nossa máquina e queremos que ela vá também para ele. Usamos o comando <code>git remote add origin https://github.com/seunome/suapasta.git</code> para dizer que é essa pasta que vai receber a pasta do nosso computador, ou seja a pasta do github vai estar sincronizada à pasta do seu computador. Depois usamos o comando <code>git push</code> para enviar nossos arquivos.

## Clonando um repositório do Github

Se um diretório já existe no Github, e queremos clonar ele em nosso computador, podemos usar o comando <code>git clone https://github.com/seuusername/suapasta.git</code>. Só isso, e se essa pasta pertence a nós mesmos ou o dono dela nos deu permissão, podemos simplesmente começar a modificar esses arquivos, commitar, e subir novamente nossos arquivos usando o `git push`.

E se a pasta já existe no computador, e também no Github, mas a pasta do computador está desatualizada, podemos usar o comando <code>git pull</code>.

### Criando páginas no Github

Agora nossa pasta já existe no Github e queremos criar uma página dela usando o serviço do Github Pages. Como essa será nossa primeira página, podemos criá-la apenas dando a nossa pasta o nome de seunome.github.io

### Ramificando páginas

O Git tem um recurso maravilhoso chamado Branch, ramo em português. Vamos voltar a pensar no Git como um fotógrafo de alterações! Imagine, agora, que nossas fotografias são frutos de uma árvore e que podem crescer por vários ramos diferentes. Podemos escolher quais ramos queremos que cresçam e podemos dar nomes a eles.

Vamos criar um ramo chamado gh-pages onde crescerão nossos frutinhos, ops! nossas páginas. Usamos o comando ``git checkout -b gh-pages`` para criar um ramo e mudar para ele ao mesmo tempo, então criamos ou mudamos nossos arquivos como queremos, damos commit, depois damos push para subir ele ao Github.

Agora podemos acessar no navegador seunome.github.io/suapasta e tchanrann! nossa página já está online!