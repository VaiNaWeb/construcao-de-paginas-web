# Acessibilidade

Pela definição da W3C, acessibilidade significa que sites, ferramentas e tecnologias são projetadas e desenvolvidas para que todas as pessoas possam usá-las. Se espera todos possam: perceber, entender, navegar e interagir com a Web e contribuir para a Web.

### Porque se preocupar com acessibilidade

Antes de tudo, você deveria se preocupar com isso como um exercício de humanidade. As pessoas com deficiência lidam com muitos desafios diariamente. Se elas estão entre seus clientes ou usuários, permitir que eles interajam com seu aplicativo da web é o mínimo que você precisa fazer.

Há dados de que **1 bilhão de pessoas em todo o mundo** e **20% de todos os usuários de internet** tenham alguma forma de deficiência.

No Brasil, segundo o [Censo de 2010 do IBGE](https://educa.ibge.gov.br/jovens/conheca-o-brasil/populacao/20551-pessoas-com-deficiencia.html), quase 46 milhões de brasileiros, cerca de **24% da população**, declarou ter pelo menos um tipo de deficiência – visual, auditiva, motora e intelectual.

Além disso a legislação atual em todo o mundo está se movendo em uma direção onde a acessibilidade está se tornando uma característica obrigatória da web.

### Respeite a semântica do HTML

Um site com uma boa estruturação, ou seja, com uma boa semântica é lido perfeitamente pelos os softwares de acessibilidade. Você pode adicionar atributos aos elementos para ajudar o usuário a saber o que está acontecendo ali. Exemplos**:**

Para navegar pela página com o botão Tab:

```markup
  <div tabindex="0">Div 1</div>
  <div tabindex="1">Div 2</div>
  <div tabindex="2">Div 3</div>
  <div tabindex="-1">Div Não-Acessível</div>
```

* A função do tabindex é definir como um elemento deve se comportar durante a navegação através do teclado. Ele pode receber os seguintes valores.
* Caso ele receba um valor **negativo** \(ex: -1\) ele não poderá ser acessado pela a tecla Tab.
* Caso ele receba um número **inteiro** e **ordenado** \(ex: 1,2\) essa será a ordem o qual ele seguirá, e por final a última forma de utilização é atribuindo o valor **zero**, neste caso a ordem a ser selecionada será definida pelo o DOM.
* Lembrando que para um elemento ser considerado focalizável deve satisfazer todas as seguintes condições: 1. Possuir a propriedade tabindex definida. 2. Estar renderizado na página. 3. Não ser um elemento inerte. 4. Não estar desabilitado \(propriedade disabled\).

### Tabelas acessíveis:

```markup
  <table>
      <caption>Quantidade de Dias em no Mês</caption>
      <thead>
          <tr>
              <th scope="col">Mês</th>
              <th scope="col">Quantidade de Dias</th>
          </tr>
      </thead>
      <tbody>
          <tr>
              <th scope="row">Janeiro</th>
              <td>31</td>
          </tr>
          <tr>
              <th scope="row">Fevereiro</th>
              <td>28</td>
          </tr>
      </tbody>
  </table>
```

O **Caption** tem como objetivo dizer sobre o que a tabela se trata. Quando você atribui ao scope um **row** ou **col**, você indica o que é Coluna e o que é Linha.

### Imagens acessíveis:

```markup
  <img src="coelho.png" alt="Imagem de Coelho, sentado comendo uma Cenoura">
```

A função do alt é transcrever a imagem para o usuário.

### Indicando os campos em um Formulário:

```markup
  <div>
      <label for="nome">Nome:</label>
      <input type="text" id="nome" name="nome" placeholder="Nome">
  </div>
```

O label é associado ao input, então fica fácil de indicar o que é solicitado no campo.

### Deixe os Links descritivos para o destino remetido:

```markup
<a href="paginainicial.html" title="Ir para Página inicial">Página Inicial</a>
```

O atributo title é ótimo para dar uma descrição ao seu link. Essa descrição é lida pelos os softwares, e aparece um popover quando se passa o cursor em cima.

Perceba que tudo que foi apresentado acima, são apenas boas práticas e um HTML bem estruturado. Para saber se seu HTML está acessível basta usar um [Validador de HTML](https://achecker.ca/checker/index.php).

### Manipulando o CSS de forma correta.

É possível mudar o tamanho das fontes e das cores de um site utilizando o CSS. Um dos cuidados especiais que temos que ter com o css é o **Espaçamento entre as letras** e os constrates de cores.

Devemos tomar alguns cuidados ao criar o design de um site, temos que pensar muito bem nas animações, e o contraste entre os planos.

Você pode testar se as cores do seu site estão com os contrates condizentes com as regras do W3C. A [**ferramenta**](http://www.checkmycolours.com/) para realizar essa verificação é apenas para sites que já estejam publicados.

### Imagens decorativas.

A ideia é que as imagens decorativas sejam ignoradas pelo leitor de tela, então essas imagens devem ser inseridas pelo CSS e **não deverão ter o alt** para que possam ser ignoradas pelo leitor.

É possível inserir dessa forma:

```markup
  <span class="icone-social"></span>
  <a href="#">Meu Facebook!</a>
```

```css
  .icone-social {
      background-image: url(../img/icone_facebook.png);
  }
```

### Imagens com textos.

Quando há uma imagem com textos que informam e passam alguma mensagem importante, não é bom limitar apenas para aqueles que não utilizam leitores de tela.

Também, não use uma imagem com texto como botão, faça um botão manual com o HTML e CSS, para que seja lido pelo leitor de tela e o usuário entenda o que o botão faz e se deseja clicar nele, caso não seja possível, não esqueça de descrever com atributo **alt** o que o link significa. Seja claro com a frase de um botão, tomando cuidado para não deixar vago demais.

### Outras recomendações

* Não é uma boa ideia colocar um temporizador na página para que ela atualize após um tempo, pois pode causar confusão para uma pessoa com deficiência visual, já que utilizam leitores de tela.
* Adicione uma Ferramente de Libras ao seu Site. A seguinte [**ferramenta**](http://www.prodeaf.net) é capaz de traduzir os textos e áudio \(apenas em português\) do seu site para Libras.
* Valide a sua Página Web. Você pode validar a sua página web com uma [**Extensão**](https://goo.gl/Y2bEwC) ou com programas automatizados como o [_CynthiaSays_](http://www.cynthiasays.com/) ou o [_Wave_](http://wave.webaim.org/).

### Referências

\*\*\*\*[Documentação da WCAG](https://www.w3.org/Translations/WCAG20-pt-br/)  
[Cartilha de acessibilidade na Web](http://www.w3c.br/pub/Materiais/PublicacoesW3C/cartilha-w3cbr-acessibilidade-web-fasciculo-I.html)   
[A11y project](https://a11yproject.com/)  
[Curso de acessibilidade da Google](https://eu.udacity.com/course/web-accessibility--ud891)

