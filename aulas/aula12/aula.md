# Criando páginas acessíveis

Quando geralmente criamos um site não pensamos em detalhes pequenos que são mega importante. Ter uma página web acessível siginifica fornecer oportunidades iguais para pessoas com necessidades especiais, além de incluir-las na sociedade.

Atualmente a acessibilidade web é obrigatória por lei ou regulamentos. A W3C criou o WAI (Web Accessibility Initiative) em 1997, e tem como grande objetivo padronizar os componentes para que seja lidos pelos softwares e promover a acessibilidade na Web.

Para tornar o sua página web acessível basta seguir as seguintes regras:

- Respeite os Elementos do HTML.

    Um site com uma boa estruturação, ou seja, com uma boa semântica é lido perfeitamente pelos os softwares de acessibilidade. Você pode adicionar atributos aos elementos para ajudar o usuário a saber o que está acontecendo ali.

    ##### Exemplos:

    - Para navegar pela página com o botão Tab:

        ```html
        <div tabindex="0">Div 1</div>
        <div tabindex="1">Div 2</div>
        <div tabindex="2">Div 3</div>
        <div tabindex="-1">Div Não-Acessível</div>
        ```

        A função do tabindex é definir como um elemento deve se comportar durante a navegação através do teclado. Ele pode receber os seguintes valores.

        Caso ele receba um valor **negativo**  (ex: -1) ele não poderá ser acessado pela a tecla Tab.

        Caso ele receba um número **inteiro** e **ordenado** (ex: 1,2) essa será a ordem o qual ele seguirá, e por final a última forma de utilização é atribuindo o valor **zero**, neste caso o ordem a ser selecionada será definida pelo o DOM.

        Lembrando que para um elemento ser considerado focalizável deve satisfazer todas as seguintes condições:
        1. Possuir a propriedade tabindex definida.
        2. Estar renderizado na página.
        3. Não ser um elemento inerte.
        4. Não estar desabilitado (propriedade disabled).

    - Tabelas acessíveis:

        ```html
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

    - Imagens acessíveis:

        ```html
        <img src="coelho.png" alt="Imagem de Coelho, sentado comendo uma Cenoura">
        ```
        A função do alt é transcrever a imagem para o usuário.

    - Indicando os campos em um Formulário:

        ```html
        <div>
            <label for="nome">Nome:</label>
            <input type="text" id="nome" name="nome" placeholder="Nome">
        </div>
        ```

        O label é associado ao input, então fica fácil de indicar o que é solicitado no campo.

    - Deixe os Links descritivos para o destino remetido:

    ```html
    <a href="paginainicial.html" title="Ir para Página inicial">Página Inicial</a>
    ```

    O atributo title é ótimo para dar uma descrição ao seu link. Essa descrição é lida pelos os softwares, e aparece um popover quando se passa o cursor em cima.

    Perceba que tudo que foi apresentado acima, são apenas boas práticas e um HTML bem estruturado. Para saber se seu HTML está acessível basta usar um [Validador de HTML](https://achecker.ca/checker/index.php).

- Manipulando o CSS de forma correta.

    É possível mudar o tamanho das fontes e das cores de um site utilizando o CSS. Um dos cuidados especiais que temos que ter com o css é o  **Espaçamento entre as letras** e os constrates de cores.

    Devemos tomar alguns cuidados ao criar o design de um site, temos que pensar muito bem nas animações, e o contraste entre os planos.

    Você pode testar se as cores do seu site estão com os contrates condizentes com as regras do W3C. A [**ferramenta**](http://www.checkmycolours.com/) para realizar essa verificação é apenas para sites que já estejam publicados.

- Não utilizar captchas.

    Nem todos os CAPTCHAS possuem acessibilidade, então crie formas de verificar se o usuário não é um bot, quem sabe uma conta matemática?

- Adicione uma Ferramente de Libras ao seu Site.

    A seguinte [**ferramenta**](http://www.prodeaf.net) é capaz de traduzir os textos e áudio (apenas em portugês) do seu site para Libras.

- Valide a sua Página Web.

    Você pode validar a sua página web com uma [**Extensão**](https://goo.gl/Y2bEwC) ou com programas automatizados como o [*CynthiaSays*](http://www.cynthiasays.com/) ou o [*Wave*](http://wave.webaim.org/).

Para saber mais sobre essas convenções da W3C basta acessar a [*Documentação da WCAG*](https://www.w3.org/Translations/WCAG20-pt-br/).
