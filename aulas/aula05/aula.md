# Construindo formulários

Usamos formulários para capturar informações dos usuários e processar solicitações. Através de controles ou campos, os formulários podem solicitar uma pequena quantidade de informações, como um campo de buscas do Google faz, por exemplo.

Precisamos saber como criar formulários para adquirir a entrada do usuário. Por enquanto, vamos discutir como usar o HTML para marcar um formulário, quais elementos usar para capturar diferentes tipos de dados. 

Não nos aprofundaremos em como as informações de um formulário são processadas e tratadas ainda. O processamento de formulários é um tópico mais profundo, vamos aprender sobre isso nos próximos módulos.

## Criando um Formulário

Para adicionar um formulário a uma página, usaremos o elemento form:
```html
<form>
  ...
</form>
```

## Input

Um dos elementos principais usados para obter uma entrada do usuário é o elemento input. Esse elemento usa o atributo type para definir qual tipo de informação deve ser capturada pelo input. O valor de atributo de tipo mais popular é o texto.

Além do atributo type, é a melhor prática dar um elemento de <input> também um atributo name, que serve para dar o nome desse controle, isso é útil, pois assim enviamos junto com o dado o lugar de onde veio esse dado para o servidor.
```html
<input type="text" name="cidade">
```
Além do text podemos usar os seguintes types:
- color
- date
- datetime
- email
- month
- number
- range
- search
- tel
- time
- url
- week

## Textarea

Outro elemento que é usado para capturar texto é o elemento textarea. Diferente do input, esse elemento pode aceitar textos maiores, ideal para quando queremos receber um texto com mais de uma linha. Ele aceita apenas um tipo de valor, o atributo name.
```html
<textarea name="comentario">Deixe aqui seu comentário</textarea>
```

## Radio Buttons

Permitem que os usurios façam uma escolha rápida de uma pequena lista de opções. Os botões de rádio permitem aos usuários selecionar apenas uma opção.

Parar cria-lo, usamos o input, e adicionamos o type radio. É necessário que todos os botões do conjunto tenham o mesmo name, assim sabemos que todos fazem parte do mesmo.

Com botões de rádio, um usuário faz uma seleção de múltipla escolha. Assim, temos que definir o valor de entrada. Usando o atributo de value, podemos definir um valor específico para cada elemento input.

É possível também pré-selecionar um botão de opção para o usuário, podemos usar o atributo checked.
```html
<input type="radio" name="dia" value="Segunda" checked> Segunda
<input type="radio" name="dia" value="Sábado"> Sábado
<input type="radio" name="dia" value="Domingo"> Domingo
```

## Check Boxes

Usam os mesmos atributos e padrões do radio buttons, mas para usa-lo mudamos o valor do type para checkbox. Com o checkbox, os usuários podem selecionar vários valores.
```html
<input type="checkbox" name="dia" value="Segunda" checked> Segunda
<input type="checkbox" name="dia" value="Sábado"> Sábado
<input type="checkbox" name="dia" value="Domingo"> Domingo
```

## Drop-Down Lists

Uma maneira ótima para pertmir aos usuários selecionar uma opção em uma lista. Para cria-la usaramos os elementos select e option. O elemento select envolve todas as opções, e cada opção é marcada usando o elemento option.

Usamos o atributo name dentro de selected, e o atributo value em cada option que estão dentro de select. O atributo value em cada elemento option corresponde ao atributo name no elemento select.

Cada elemento da lista fica em um option. Ao invés de checked, para pré-selecionar uma opção usamos o selected como atributo na opção que queremos fazer isso.

```html
<select name="dia">
  <option value="Segunda" selected>Segunda</option>
  <option value="Sábado">Sábado</option>
  <option value="Domingo">Domingo</option>
</select>
```
## Form Buttons
## File Input
## Label
## Fieldset
## Legend
## Form & Input Attributes




