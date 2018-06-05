# Conhecendo a linha de comando

Vamos conhecer finalmente a famosa telinha preta que vemos os hackers usando nos filmes e séries. Algo que o cinema não mostra, é que elas são bem simples, e podem ser usadas para diversas coisas, desde criar um novo arquivo na área de trabalho, e até mesmo colocar um site ou aplicação online.

Essa famosa telinha preta, que é chamada de linha de comando, cmd, prompt, console, terminal... ufa! ou interface de linha de comando, é um aplicativo baseado em texto para visualização, manipulação e manuseio de arquivos em seu computador.

Graças às maravilhosas e amigáveis interfaces que foram criadas para usarmos nos computadores, perdemos a necessidade de usar o terminal no nosso dia-a-dia. Mas dominar alguns comandos dessa telinha pode ajudar muito em nossa jornada na programação, e é por isso que vamos começar a aprende-los! Para aproveitar melhor esssa e outras aulas, é recomendado que você escreva os comandos ao invés de copia-los, dessa forma você vai lembrar deles depois.

Vamos aprender alguns comandos, eles mudam um pouco de sistema operacional para sistema operacional. Durante essa aula vamos focar nos comandos do Linux. Isso porque nos computadores dos polos onde o VnW acontece escolhemos usar esse sistema. 

Mas se você usa Windows em casa pode pesquisar os comandos equivalentes, ou se preferir, você pode usar o [Git Bash](https://git-scm.com/) mas nem todos os comandos podem funcionar. 

## Primeiros comandos

Para começar, abra o terminal digite o seguinte comando:
```
whoami
```
O computador acabou de apresentar seu nome de usuário! Legal, não é?


Seria legal saber em que pasta estamos agora. É recomendável que você sempre saiba essa informaço! Se você não souber, é só usar o comando. Digite o seguinte comando e aperte o enter:

```
pwd
```
Se preferir, você pode também se localizar vendo quais arquivos estão dentro da pasta. Você pode descobrir isso usando o comando:
```
ls
```
## Navegando entre pastas

Uma coisa bem legal que você pode fazer agora é aprender a navegar entre pastas! Eu não tenho certeza de quais pastas você tem aí em seu computador, então vamos criar uma nova chamada teste. Digite o seguinte comando:
```
mkdir teste
```
Para ter certeza de que a pasta foi criada você pode usar o ls de novamente.
```
ls
```
Se a pasta foi criada, agora você pode entrar dentro dela usando o seguinte comando:
```
cd teste
```
Legal! Você conseguiu entrar dentro dela. Que tal agora voltar? Você pode fazer isso usando o comando:
```
cd ..
```

## Alguns comandos

Há muitos comandos úteis, que podem fazer muitas coisas, como desligar o computador, criar arquivos, remover arquivos, e mais um monte de outras coisas. Há alguns bem básicos que podem nos ajudar muito em nossas tarefas enquanto desenvolvedor. Vamos conhecer alguns:

<code>whoami</code>: Mostra o nome do usuário<br>
<code>man</code>: Usado para mostrar o manual de um outro comando<br>
<code>sudo</code>: Deve ser usado com cuidado. Ele dá permissões de administrador<br>
<code>ls</code>: Lista os arquivos do diretório<br>
<code>pwd</code>: Mostra o diretório atual<br>
<code>cd</code>: Usado para mudar de diretório<br>
<code>cp</code>: Copia um arquivo ou diretório<br>
<code>mv</code>: Usado para mover um arquivo ou renomea-lo<br>
<code>mkdir</code>: Cria uma nova pasta<br>
<code>touch</code>: Cria um novo arquivo<br>
<code>more</code>: Lê um arquivo de texto<br>
<code>grep</code>: Lê e faz uma busca por palavras dentro de um arquivo<br>
<code>clear</code>: Limpa a tela<br>
<code>exit</code>: Fecha o terminal<br>
