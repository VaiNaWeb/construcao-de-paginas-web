# Desafios

## Desafio 01: Versionando uma música!

1. Crie uma pasta
2. Crie um arquivo de texto chamado musica.txt
3. Abra sua pasta no terminal e peça ao git que comece a versiona-la
4. Abra seu arquivo de texto e escreva uma frase da música que você mais gosta. Depois salve ele
5. Volte ao terminal e o use o comando para avisar ao git que você quer mesmo que sua alteração seja salva
6. Ainda no terminal, peça ao git que salve essa alteração, e deixe nela um comentário
7. Abra novamente seu arquivo de texto e adicione mais uma frase da música
8. Volte ao terminal e lembre ao git novamente de que você vai querer salvar essa alteração
9. Ainda no terminal, peça ao git que salve essa alteração, e deixe nela mais um comentário
10. Pergunte ao Git quais alterações foram gravadas

## Desafio 02: Minha página na web

1. Crie uma conta no Github
2. Crie uma pasta no seu computador chamada seunome.github.io
3. Abra sua pasta ano terminal e peça ao git que comece a versiona-la
4. Abra a pasta e crie dentro dela um arquivo chamado index.html
5. Abra o arquivo, escreva seu nome, e um textinho contando quem é você e coisas que você gosta de fazer. Salve ele
6. Volte ao terminal e o use o camando para avisar ao git que você quer mesmo que sua alteração seja salva
7. Ainda no terminal, peça ao git que salve essa alteração, e deixe nela um comentário
8. Vá ao Github e crie uma pasta também chamada seunome.github.io
9. Volte ao terminal e digite o comando que sincroniza a pasta do github com a pasta do seu computador
10. Ainda no terminal, digite o camando para subir as alterações do seu computador para o Github
11. Acesse o endereço seunome.github.io pelo seu navegador

## Desafio 03: Minha página web ramificada.

1. Crie um novo branch na pasta do projeto em seu computador

   ```text
   git checkout -b meu-novo-ramo
   ```

2. Abra o arquivo index.html
3. Acrescente algum conteúdo que gostaria de ver em seu site, uma foto, uma lista de músicas.

   ```text
   <ul>
   <li>Zezé de Camargo e Luciano - Evidências</li>
   <li>The Lumineers - Ophelia</li>
   <li>Imagine Dragons - Thunder</li>
   <li>Tom Rosenthal - Go Solo</li>
   </ul>
   ```

4. Abra o terminal e peça para o git preparar as mudanças no seu arquivo

   ```text
   git add index.html
   ```

5. Ainda no terminal peça para o git salvar suas alterações

   ```text
   git commit -m "Adicionei uma lista de músicas"
   ```

6. Volte para o ramo \(_branch_\) **master** digitando o seguinte comando

   ```text
   git checkout master
   ```

7. Peça para o git mesclar os dois ramos _master_ e _meu-novo-ramo_ utilizando o seguinte comando

   ```text
   git merge meu-novo-ramo
   ```

8. Peça para o git subir suas alterações para o GitHub

   ```text
   git pull -u origin master
   ```

9. Acesse o endereço seunome.github.io para verificar as alterações.

Podemos utilizar as ramificações quando queremos trabalhar com algum colega e não queremos alterar código juntos. Existem alguns problemas em trabalhar em ramificações, quando utilizar o comando _git merge_ podemos ter alguns conflitos,

## Desafio 04: Trabalhando com colega, resolvendo conflitos

Não temos nenhum complexo de identidade, mas aqui iremos nos passar por duas pessoas, a primeira é você e a segunda é seu colega lhe ajudando com o código da sua página.

Vamos começar sendo você mesmo.

1. Crie um novo branch chamado letra-musica

   ```text
   git checkout -b letra-musica
   ```

2. Abra o arquivo index.html
3. Insira no arquivo a letra de uma música, como por exemplo **Ophelia**

   ```text
   <h2>Trecho da Música Ophelia</h2>
   <p>
   Oh, oh, when I was younger, oh, oh, should have known better
   And I can't feel no remorse, and you don't feel nothing back
   </p>
   ```

4. Peça para que o git se prepare as modificações no arquivo index.html

   ```text
   git add index.html
   ```

5. Faça com que o git persista as alterações no código

   ```text
   git commit -m "Trecho da música Ophelia da banda Luminners"
   ```

6. Volte para o ramo \(branch\) **master**

   ```text
   git checkout master
   ```

Agora iremos se passar pelo seu colega.

1. Na pasta do projeto do seu computador, crie um novo branch

   ```text
   git checkout -b letra-musica-do-colega
   ```

2. Abra o arquivo index.html
3. Insira no arquivo a letra de uma música, como por exemplo **Ophelia**

   ```text
   <h2>Trecho da Música Ophelia</h2>
   <p>
   Oh, oh, got a new girlfriend, he feels like he's on top
   And I don't feel no remorse, and you can't see past my blinders
   </p>
   ```

4. Peça para que o git se prepare as modificações no arquivo index.html

   ```text
   git add index.html
   ```

5. Faça com que o git persista as alterações no código

   ```text
   git commit -m "Trecho da música Ophelia da banda Luminners"
   ```

6. Volte para o ramo \(branch\) **master**

   ```text
   git checkout -b master
   ```

Agora podemos atualizar o branch master em relação as branchs criados anteriormente.

1. Sincronize o branch _master_ com o branch _letra-musica_

   ```text
   git merge letra-musica
   ```

2. Sincronize o branch _master_ com o branch _letra-musica-colega_

   ```text
   git merge letra-musica-colega
   ```

Para apresentar o conflito o git inseri no arquivo que contém o conflito os seguintes caracteres.

```text
<<<<
'trecho de música do branch _letra-musica_
====
'trecho de música do branch _letra-musica-colega_
>>>>
```

1. Abra o arquivo index.html
2. Navegue até o trecho de código conflitante.
3. Encontre os caracteres inseridos pelo git para identificar o conflito.
4. Resolva o conflito, escolha o trecho do seu colega e apague

   ```text
   <<<<
   O seu trecho
   ====
   >>>>
   ```

5. Após remover os caracteres de conflito, peça para o git preparar as mudanças.

   ```text
   git add index.html
   ```

6. Faça o git persistir as mudanças.

   ```text
   git commit -m "Conflito resolvido, trecho de música do colega escolhido"
   ```

7. Envie o código para o github

   ```text
   git push -u origin master
   ```

8. Entre na página seu-projeto.github.io para vizualizar as mudanças.

## Desafio 05: Começando uma nova linha de trabalho

A ideia deste desafio é utilizar o comando "cherry-pick", que permite você trabalhar a partir de um determinado commit específico de seu ambiente local. Para auxiliá-lo no entendimento, você pode realizar um breve estudo vendo este conteúdo aqui: [https://www.youtube.com/watch?v=CUpk6F2eNs0](https://www.youtube.com/watch?v=CUpk6F2eNs0)

1. Realize 4 novos commits em seu projeto
2. Crie uma nova branch com o nome "new\_work\_branch"
3. Na nova branch, especifique que você deseja trabalhar a partir do conteúdo do seu terceiro commit realizado \(criado no passo 1\)
4. Verifique no log do GIT como está seu ambiente de trabalho, para o completo entendimento do comando cherry-pick

