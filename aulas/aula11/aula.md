#Criando páginas para múltiplos dispositivos

Muita coisa aconteceu desde o surgimento da internet, e nossa experiência com a tecnologia também se modificou muito com o passar dos anos. A realidade que conhecemos hoje, é que estamos realmente conectados o tempo inteiro, e através de vários dispositivos diferentes.

Não somente no computador, hoje sabemos que é possível nos conectar usando uma infinidade de aparelhos diferentes, televisão, videogame, celular, etc. E estamos conectados também nos mais diferentes lugares, seja na padaria, na escola, ou em casa. A web está em todos os lugares!

##Design responsivo

É nosso dever e desafio enquanto desenvolvedores web, criar páginas que possibilitem que essas experiências aconteçam da melhor forma possível. Há muitas coisas que podemos fazer para garantir que isso aconteça, uma delas, é criar páginas que sejam exibidas de forma correta nos mais diferentes dispositivos, assim nasceu o conceito de [Design responsivo](https://brasil.uxdesign.cc/o-que-%C3%A9-responsive-web-design-ab292eb616b7#.oin348i9x).

Dizemos que uma página é responsiva, quando os elementos dela se adaptam automaticamente à tela do dispositivo no qual ela está sendo visualizada. Na prática, há algumas técnicas que usamos para que esse comportamento aconteça.

Antes de tudo, precisamos dizer ao navegador que a escala inicial da nossa página é equivalente ao tamanho do dispositivo. Adicionamos a seguinte linha ao <code>head</code>:

```html
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
```
Nós já aprendemos Flexbox, então todo o resto acaba por ficar mais simples a partir daqui. Isso porque o Flexbox é muito legal para tornar nosso layout flexível, e flexibilidade e fluidez faz parte do que queremos atingir com o design responsivo. Ao invés de ficar usando pixels, nós também podemos usar unidades de medida flexíveis, você pode ler mais sobre isso nesse [link](http://www.maujor.com/tutorial/unidades-de-medidas-css.php). 

Também muito importantes para tornar nossas páginas responsivas são as media queries. Usamos elas basicamente para criar modificações na página para que ela se adapte de acordo com uma medida. Nós podemos dizer por exemplo que se uma página tem até 640px de largura o background dela deve mudar sua cor.

```css
@media (max-width: 640px) {
	body {
		background: tomato;
	}
}
```

Mudar a cor de uma página de acordo com seu tamanho pode não ser muito interessante, mas podemos modificar outras coisas que são, como por exemplo modificar o tamanho de um container, o lugar de um botão, deixar uma letra maior ou menor... são muitas [possibilidades](https://tableless.com.br/design-responsivo-na-pratica-do-rascunho-ao-digita/) que podem e devem ser aproveitadas. 

De acordo com cada centário, podemos considerar muitas coisas, e pensando nessas coisas usar as melhores técnicas para criar a experiência de navegação que queremos.