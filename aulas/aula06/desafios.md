<!-- Aula 06 - Git e Github -->
# Desafio01: Versionando uma música!

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

# Desafio02: Minha página na web

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

# Desafio03: Minha página web ramificada.

1. Crie um novo branch na pasta do projeto em seu computador
```
git checkout -b meu-novo-ramo
```
2. Abra o arquivo index.html
2. Acrescente algum conteúdo que gostaria de ver em seu site, uma foto, uma lista de músicas.
```
<ul>
  <li>Zezé de Camargo e Luciano - Evidências</li>
  <li>The Lumineers - Ophelia</li>
  <li>Imagine Dragons - Thunder</li>
  <li>Tom Rosenthal - Go Solo</li>
</ul>
```
3. Abra o terminal e peça para o git preparar as mudanças no seu arquivo
```
git add index.html
```
4. Ainda no terminal peça para o git salvar suas alterações
```
git commit -m "Adicionei uma lista de músicas"
```
5. Volte para o ramo (_branch_) **master** digitando o seguinte comando
```
git checkout master
```
6. Peça para o git mesclar os dois ramos _master_ e _meu-novo-ramo_ utilizando o seguinte comando
```
git merge meu-novo-ramo
```
7. Acesse o endereço seunome.github.io para verificar as alterações.

---
Podemos utilizar as ramificações quando queremos trabalhar com algum colega e não queremos alterar código juntos.
Existem alguns problemas em trabalhar em ramificações, quando utilizar o comando _git merge_ podemos ter alguns conflitos,

---


Não lembra dos principais comandos do git? Sinta-se à vontade para ler novamente a aula, e/ou o resumo dela.
