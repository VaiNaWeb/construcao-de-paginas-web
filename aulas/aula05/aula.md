# Construindo formulários

Os formulários são uma parte essencial da Internet, usamos formulários para capturar informações dos usuários e processar solicitações. Através de controles ou campos, os formulários podem solicitar uma pequena quantidade de informações, como um campo de buscas do Google faz, por exemplo.

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

Outro elemento que é usado para capturar texto é o elemento textarea. Diferente de input, esse elemento pode aceitar textos maiores, ideal para quando queremos receber um texto com mais de uma linha. Ele aceita apenas um tipo de valor, o atributo name.
```html
<textarea name="comment">Add your comment here</textarea>
```
