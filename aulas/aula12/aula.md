# Criando páginas acessíveis

Quando geralmente criamos um site não pensamos em detalhes pequenos que são megas importantes. Ter uma página web acessível siginifica fornecer oportunidades iguais para pessoas com necessidades especiais, além de incluir-las a sociedade.

Atualmente a acessibilidade web é obrigatória por lei ou regulamentos. A W3C criou o WAI (Web Accessibility Initiative) em 1997, e tem como grande objetivo padronizar os componentes para que seja lidos pelos softwares e promover a acessibilidade na Web.

Para tornar o sua página web acessível basta seguir as seguintes regras:

- Respeite os Elementos do HTML:

    Um site com uma boa estruturação, ou seja, com uma boa semântica é lido perfeitamente pelos os softwares de acessibilidade. Você pode adicionar atributos aos elementos para ajudar o usuário a saber o que está acontecendo ali.

    ##### Exemplos:

    - Para navegar pela página com o botão Tab:

        ```html
        <div tabindex="0">Div 1</div>
        <div tabindex="1">Div 2</div>
        <div tabindex="2">Div 3</div>
        <div tabindex="-1">Div Não-Acessível</div>
        ```

        A função do tabindex é definir como um elemento deve se comportar durante a navegação através do teclado. Ele pode receber os seguintes valores.    Caso ele receba um valor **negativo**  (ex: -1) ele não poderá ser acessado pela a tecla Tab. Caso ele receba um número **inteiro** e **ordenado** (ex: 1,2) essa será a ordem o qual ele seguirá, e por final a última forma de utilização é atribuindo o valor **zero**, neste caso o ordem a ser selecionada será definida pelo o DOM.

        Lembrando que para um elemento ser considerado focalizável deve satisfazer todas as seguintes condições:
        1. Possuir a propriedade tabindex definida.
        2. Estar renderizado na página.
        3. Não ser um elemento inerte.
        4. Não estar desabilitado (propriedade disabled).

    - Tabelas acessíveis:

        ```html

        ```

        A função do

    - Imagens acessíveis:

        ```html
        <img src="coelho.png" alt="Imagem de Coelho, sentado comendo uma Cenoura">
        ```

        A função do alt é transcrever a imagem para o usuário.

    - Indicando os campos em um Formulário:

        ```html
        <div>
            <label for="nome">Nome:</label>
            <input type="text" id="nome" nome="nome">
        </div>
        ```

        A função do alt é transcrever a imagem para o usuário.