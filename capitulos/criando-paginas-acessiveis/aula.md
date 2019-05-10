# Criando páginas acessíveis

Geralmente quando criamos um site não pensamos em detalhes pequenos que são mega importante. Ter uma página web acessível significa fornecer oportunidades iguais para pessoas com necessidades especiais, além de incluí-las na sociedade.

A acessibilidade pode ser definida como como uma forma de dar autonomia para todos aqueles que possuem algum tipo de mobilidade reduzida ou deficiência. Garantindo que essas pessoas possam realizar atividades sem precisar pedir ajuda.

Na construção de uma aplicação ou um site, é importante pensar que todas as pessoas que farão uso, possam ter acesso aos mesmos conteúdos, a mesma facilidade de uso e por fim, a mesma satisfação. A acessibilidade não deve ser encarada como um bônus ou deixada para ser pensada depois que o site já estiver pronto, ela precisa estar em primeiro plano para fornecer oportunidades iguais para pessoas com capacidades diferentes e inseridas em diversos contextos, isso inclui também idosos, pessoas que possuem menor capacidade de velocidade na internet ou até mesmo tornar uma experiência boa para aqueles que nunca tiveram contato com a internet.

Mas existem tantas pessoas assim que precisam ser levadas em conta? Bom, segundo o [Censo de 2010 do IBGE](http://www.pessoacomdeficiencia.gov.br/app/sites/default/files/publicacoes/cartilha-censo-2010-pessoas-com-deficienciareduzido.pdf): 23,9% da população total, têm pelo menos algum tipo de deficiência – visual, auditiva, motora e intelectual.

Atualmente a acessibilidade web é obrigatória por lei ou regulamentos. A W3C criou o WAI \(Web Accessibility Initiative\) em 1997, e tem como grande objetivo padronizar os componentes para que seja lidos pelos softwares e promover a acessibilidade na Web.

Na [cartilha de acessibilidade na Web](http://www.w3c.br/pub/Materiais/PublicacoesW3C/cartilha-w3cbr-acessibilidade-web-fasciculo-I.html) da W3C, se diz: _"Para a maioria das pessoas, a tecnologia torna a vida mais fácil. Para uma pessoa com necessidades especiais, a tecnologia torna as coisas possíveis."_ A ideia a ser passada é que essas pessoas já são limitadas no ambiente físico por não possuírem acesso a recursos que em sua maioria estão indisponíveis, então há aqui uma chance de mudar essa realidade para muitos, apenas com a atenção de buscar que tipos de usuários existem e fazer algumas mudanças para que possam não só desfrutar da internet em condições melhores, mas como também contribuir com ela, com suas experiências e seus conhecimentos.

Para tornar a sua página web acessível basta seguir as seguintes regras:

### Respeite os Elementos do HTML

Um site com uma boa estruturação, ou seja, com uma boa semântica é lido perfeitamente pelos os softwares de acessibilidade. Você pode adicionar atributos aos elementos para ajudar o usuário a saber o que está acontecendo ali.

**Exemplos:**

* Para navegar pela página com o botão Tab:

  ```markup
    <div tabindex="0">Div 1</div>
    <div tabindex="1">Div 2</div>
    <div tabindex="2">Div 3</div>
    <div tabindex="-1">Div Não-Acessível</div>
  ```

  A função do tabindex é definir como um elemento deve se comportar durante a navegação através do teclado. Ele pode receber os seguintes valores.

  Caso ele receba um valor **negativo** \(ex: -1\) ele não poderá ser acessado pela a tecla Tab.

  Caso ele receba um número **inteiro** e **ordenado** \(ex: 1,2\) essa será a ordem o qual ele seguirá, e por final a última forma de utilização é atribuindo o valor **zero**, neste caso a ordem a ser selecionada será definida pelo o DOM.

  Lembrando que para um elemento ser considerado focalizável deve satisfazer todas as seguintes condições: 1. Possuir a propriedade tabindex definida. 2. Estar renderizado na página. 3. Não ser um elemento inerte. 4. Não estar desabilitado \(propriedade disabled\).

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

HTML

```markup
  <span class="icone-social"></span>
  <a href="#">Meu Facebook!</a>
```

CSS

```css
  .icone-social {
      background-image: url(../img/icone_facebook.png);
  }
```

### Imagens com textos.

Quando há uma imagem com textos que informam e passam alguma mensagem importante, não é bom limitar apenas para aqueles que não utilizam leitores de tela.

Também, não use uma imagem com texto como botão, faça um botão manual com o HTML e CSS, para que seja lido pelo leitor de tela e o usuário entenda o que o botão faz e se deseja clicar nele, caso não seja possível, não esqueça de descrever com atributo **alt** o que o link significa. Seja claro com a frase de um botão, tomando cuidado para não deixar vago demais.

### Não force a atualização da página.

Não é uma boa ideia colocar um temporizador na página para que ela atualize após um tempo, pois pode causar confusão para uma pessoa com deficiência visual, já que utilizam leitores de tela.

* Adicione uma Ferramente de Libras ao seu Site.

  A seguinte [**ferramenta**](http://www.prodeaf.net) é capaz de traduzir os textos e áudio \(apenas em portugês\) do seu site para Libras.

* Valide a sua Página Web.

  Você pode validar a sua página web com uma [**Extensão**](https://goo.gl/Y2bEwC) ou com programas automatizados como o [_CynthiaSays_](http://www.cynthiasays.com/) ou o [_Wave_](http://wave.webaim.org/).

O W3C também criou o documento WCAG 2.0 com recomendações para a web, ele está estruturado em _quatro princípios_:

1. **Perceptível** - a informação e os componentes da interface do usuário têm de ser apresentados aos usuários em formas que eles possam perceber.
2. **Operável** - os componentes de interface de usuário e a navegação têm de ser operáveis. 
3. **Compreensível** - a informação e a operação da interface de usuário têm de ser compreensíveis. 
4. **Robusto** - o conteúdo tem de ser robusto o suficiente para poder ser interpretado de forma concisa por diversos agentes do usuário, incluindo recursos de tecnologia assistiva.

Para saber mais sobre essas convenções da W3C basta acessar a [_Documentação da WCAG_](https://www.w3.org/Translations/WCAG20-pt-br/).

