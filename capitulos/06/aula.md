# Git

Vamos colocar nossa primeira página online, e para isso vamos usar Git, o Github e seu serviço Github Pages como nossa ferramenta. Mas antes, precisamos compreender o que são cada uma dessas ferramentas e como elas funcionam.

O Git é um sistema de controle de versão e gerenciamento de código fonte. Foi desenvolvido por Linus Torvalds, criado inicialmente para o desenvolvimento do Kernel Linux, e é ainda hoje muito usado em diferentes projetos digitais no mundo inteiro.

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

O Github é uma plataforma social através da qual milhares de pessoas constroem códigos, entre outras coisas, de forma colaborativa, aberta e gratuita.

>"O Github, é na verdade uma rede social ou uma fábrica social de software, que desenvolve e promove milhares de códigos fontes pré armazenados, para as mais diversas finalidades." Wikipedia

Queremos que nossos arquivos sejam armazenados não somente em nosso computador, mas também no Github. Vamos usar alguns comandos do Git para nos ajudar nessa missão.

## Subindo um repositório para o Github

Nossa pasta já existe no computador, mas dentro do Github ainda não, certo? Então, vamos abrir o site do github, criar uma conta, e lá criar um repositório vazio para nosso projeto.

O projeto da sua máquina precisa conversar com o projeto que está lá no Github, para isso, um precisa saber quem é o outro. Vamos voltar ao terminal e dentro da nossa pasta usar um comando que diz o endereço para onde ela deve ir. Lembre de copiar esse endereço lá no Github. Exemplo:

```
git remote add origin https://github.com/seunome/suapasta.git
```

Agora que a nossa pasta já sabe para onde ela deve ir, vamos pedir que ela vá! Vamos subir os nossos commits que estão em nossa pasta para a pasta que criamos no Github usando o comando push:

```
git push origin master
```

No primeiro push precisamos especificar o apelido do remote, e a branch que enviaremos. O Remote é o endereço do repositório, por padrão chamamos ele de origin, mas você pode adicionar novos remotes com outros apelidos depois. A primeira branch por padrão chamamos de master, vamos aprender o que são elas em outras aulas.

Nos próximos commits que você desejar enviar, não precisa necessariamente dizer essas informações, a não ser que elas tenham mudado. Basta usar o push assim:

```
git push
``` 

## Clonando um repositório do Github

Se um diretório já existe no Github, mas ainda não em nossa máquina, podemos clonar ele em nosso computador, para isso usamos o seguinte comando:

```
git clone https://github.com/seuusername/suapasta.git
```

## Atualizando um repositório

Se a pasta já existe no computador, e também no Github, mas a pasta do computador está desatualizada, podemos baixar os novos commits que estão lá, atualizando a nossa pasta com o seguinte comando:

```
git pull
```

### Criando páginas no Github

Agora nossa pasta já existe no Github e queremos criar uma página dela usando o serviço do Github Pages. Como essa será nossa primeira página, podemos criá-la apenas dando a nossa pasta o nome de seunome.github.io

### Ramificando páginas

O Git tem um recurso maravilhoso chamado Branch, ramo em português. Vamos voltar a pensar no Git como um fotógrafo de alterações! Imagine, agora, que nossas fotografias são frutos de uma árvore e que podem crescer por vários ramos diferentes. Podemos escolher quais ramos queremos que cresçam e podemos dar nomes a eles.

Vamos criar um ramo chamado gh-pages onde crescerão nossos frutinhos, ops! nossas páginas. Usamos o comando ``git checkout -b gh-pages`` para criar um ramo e mudar para ele ao mesmo tempo, então criamos ou mudamos nossos arquivos como queremos, damos commit, depois damos push para subir ele ao Github.

Agora podemos acessar no navegador seunome.github.io/suapasta e tchanrann! nossa página já está online!

Então já podemos usar o [Github Pages](https://tableless.com.br/criando-paginas-web-para-seus-repositorios-com-o-github-pages/) para colocar nossa página online. Ele é um serviço oferecido pelo Github, que permite a criação de páginas na web a partir de projetos que foram armazenados nele.