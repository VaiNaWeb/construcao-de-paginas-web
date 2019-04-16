# Construindo formulários

Usamos formulários para receber dados e processar solicitações. Através de controles ou campos, os formulários podem solicitar uma pequena quantidade de informações, como um campo de buscas do Google faz, por exemplo.

Precisamos saber como criar formulários para adquirir a entrada do usuário. Por enquanto, vamos discutir como usar o HTML para marcar um formulário, quais elementos usar para capturar diferentes tipos de dados.

Não nos aprofundaremos em como as informações de um formulário são processadas e tratadas ainda. O processamento de formulários é um tópico mais profundo, vamos aprender sobre isso nos próximos módulos.

## Criando um Formulário

Para adicionar um formulário a uma página, usaremos o elemento form:

```markup
<form>
  ...
</form>
```

## Input

Um dos elementos principais usados para obter uma entrada do usuário é o elemento input. Esse elemento usa o atributo type para definir qual tipo de informação deve ser capturada pelo input. O valor de atributo de tipo mais popular é o texto.

Além do atributo type, é a melhor prática dar um elemento de `<input>` também um atributo name, que serve para dar o nome desse controle, isso é útil, pois assim enviamos junto com o dado o lugar de onde veio esse dado para o servidor.

```markup
<input type="text" name="cidade">
```

Além do text podemos usar os seguintes types:

* color
* date
* datetime
* email
* month
* number
* range
* search
* tel
* time
* url
* week

## Textarea

Outro elemento que é usado para capturar texto é o elemento textarea. Diferente do input, esse elemento pode aceitar textos maiores, ideal para quando queremos receber um texto com mais de uma linha. Ele aceita apenas um tipo de valor, o atributo name.

```markup
<textarea name="comentario">Deixe aqui seu comentário</textarea>
```

## Radio Buttons

Permitem que os usurios façam uma escolha rápida de uma pequena lista de opções. Os botões de rádio permitem aos usuários selecionar apenas uma opção.

Parar cria-lo, usamos o input, e adicionamos o type radio. É necessário que todos os botões do conjunto tenham o mesmo name, assim sabemos que todos fazem parte do mesmo.

Com botões de rádio, um usuário faz uma seleção de múltipla escolha. Assim, temos que definir o valor de entrada. Usando o atributo de value, podemos definir um valor específico para cada elemento input.

É possível também pré-selecionar um botão de opção para o usuário, podemos usar o atributo checked.

```markup
<input type="radio" name="dia" value="Segunda" checked> Segunda
<input type="radio" name="dia" value="Sábado"> Sábado
<input type="radio" name="dia" value="Domingo"> Domingo
```

## Check Boxes

Usam os mesmos atributos e padrões do radio buttons, mas para usa-lo mudamos o valor do type para checkbox. Com o checkbox, os usuários podem selecionar vários valores.

```markup
<input type="checkbox" name="dia" value="Segunda" checked> Segunda
<input type="checkbox" name="dia" value="Sábado"> Sábado
<input type="checkbox" name="dia" value="Domingo"> Domingo
```

## Drop-Down Lists

Uma maneira ótima para pertmir aos usuários selecionar uma opção em uma lista. Para cria-la usaramos os elementos select e option. O elemento select envolve todas as opções, e cada opção é marcada usando o elemento option.

Usamos o atributo name dentro de selected, e o atributo value em cada option que estão dentro de select. O atributo value em cada elemento option corresponde ao atributo name no elemento select.

Cada elemento da lista fica em um option. Ao invés de checked, para pré-selecionar uma opção usamos o selected como atributo na opção que queremos fazer isso.

```markup
<select name="dia">
  <option value="Segunda" selected>Segunda</option>
  <option value="Sábado">Sábado</option>
  <option value="Domingo">Domingo</option>
</select>
```

## Form Buttons

Os usuários clicam no botão enviar para processar dados depois de preencher um formulário. O botão enviar é criado usando o elemento input com um valor de atributo de tipo de envio. O atributo de valor é usado para especificar o texto que aparece no botão.

```markup
<input type="submit" name="enviar" value="Enviar">
```

O elemento button executa da mesma maneira que o elemento input com o valor de atributo de tipo de submit; mas ele também inclui tags de abertura e fechamento, que podem conter outros elementos. Por padrão, o elemento button atua como se tivesse um valor de atributo de tipo de envio.

Em vez de usar o atributo value para controlar o texto dentro do botão submit, o texto que aparece entre as tags de abertura e de fechamento do elemento button aparecerá.

```markup
<button name="enviar">
  <strong>Enviar mensagem</strong>
</button>
```

## File Input

Para permitir que os usuários adicionem um arquivo a um formulário, como anexar um documento a um e-mail, por exemplo, usamos o valor do arquivo para o atributo type.

```markup
<input type="file" name="file">
```

## Label

Os labels fornecem legendas ou títulos, vinculando-os e criando uma forma acessível para todos os usuários e tecnologias assistivas, muito úteis para garantir acessibilidade. Criado usando o elemento label, os labels devem incluir um texto que descreva as entradas ou controles aos quais eles pertencem.

Podemos incluir um atributo for, o valor dele deve ser o mesmo que o valor do atributo id no controle de formulário ao qual esse label corresponde. A correspondência dos valores de atributo for e id atribui os dois elementos, permitindo aos usuários clicar no elemento para trazer foco para o controle de formulário apropriado.

```markup
<label for="usuario">Usuário</label>
<input type="text" name="usuario" id="usuario">
```

O elemento também pode envolver controles de formulário, como botões de opção ou caixas de seleção. Nesse caso não precisamos usar os atributos for e id.

```markup
<label>
  <input type="radio" name="dia" value="Segunda" checked> Segunda
</label>
<label>
  <input type="radio" name="dia" value="Sábado"> Sábado
</label>
<label>
  <input type="radio" name="dia" value="Domingo"> Domingo
</label>
```

## Fieldset

Usamos Fieldsets para agrupar os controles de formulário e os rótulos em seções organizadas. Assim como uma section, fieldset é um elemento de nível de bloco que envolve elementos relacionados dentro de um form, para melhor organização.

```markup
<fieldset>
  <label>
    Usuário
    <input type="text" name="usuario">
  </label>
  <label>
    Senha
    <input type="text" name="senha">
  </label>
</fieldset>
```

## Legend

Legend funciona como um título para o fieldset, ele pode envolver uma descrição dos controles do fieldset.

```markup
<fieldset>
  <legend>Login</legend>
  <label>
    Username
    <input type="text" name="username">
  </label>
  <label>
    Password
    <input type="text" name="password">
  </label>
</fieldset>
```

## Mais alguns atributos

Há ainda muitos atributos úteis que não vimos ainda, por agora, veremos mais alguns dos mais usados.

Para desabilitar um campo por exemplo, usamos o atributo disabled:

```markup
<label>
  Username
  <input type="text" name="usuario" disabled>
</label>
```

Para mostrar uma descrição do controle dentro do próprio campo input usamos o placeholder:

```markup
<label>
  Email
  <input type="email" name="email" placeholder="nome@exemplo.com">
</label>
```

Para tornar o preenchimento do campo como obrigatório usamos o required:

```markup
<label>
  Email
  <input type="email" name="email" required>
</label>
```

Outros atributos interessantes que você deveria pesquisar e ler mais sobre:

* accept
* autocomplete
* autofocus
* formaction
* formenctype
* formmethod
* formnovalidate
* formtarget
* max
* maxlength
* min
* pattern
* readonly
* selectionDirection
* step

