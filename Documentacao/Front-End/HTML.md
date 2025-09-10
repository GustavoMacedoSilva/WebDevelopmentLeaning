<h2>COMANDOS</h2>

```
<hr>
<br>
<pre>
	La
	La
	La
</pre>
```

<hr>

<h2>HYPERLINK</h2>

Criação de um link:
```
<a href="link-que-vc-quer.com"
target="_blank"
title="Vai para o link que voce quer"
>
</a>
```
O codigo ali faz o seguinte:

<a href="link-que-vc-quer.com"
target="_blank"
title="Vai para o link que voce quer">
Texto Clickavel
</a>

- O ```<a href=""></a>``` é oque da a propriedade de hyperlink para o texto, dentro do "" do href voce coloca o link que quer.
- O ``target="_blank"`` da a propriedade de quando voce clicka no link, ele abre uma outra pagina para o link, inves de sobrescrever a que voce esta.
- O ``title=""`` faz com que quando voce coloque o mouse por cima do hyperlink ele mostra o que esta escrito dentro do ""

<hr>

<h2>IMAGENS</h2>

Para colocarmos uma imagem no HTML usaremos:

```
<img src="./caminho-da-imagem.png"
alt="Meio que uma descrição para a imagem"
height="200">
```

Passo a passo do que essas linhas significam:
- A linha ``src=""`` é onde voce coloca o caminho relativo ao arquivo HTML para a imagem.
- A linha ``alt=""`` pode ser escrito uma descrição para a imagem, isso ajuda muito as ferramentas de acessibilidade, principalmente para pessoas cegas.
- Você também pode alterar a dimensão da imagem usando ``height=""`` ou ``width=""``.
Também é possível transformar a imagem em um hyperlink, apenas encaixotar o ``<img>`` em um ``<a></a>``.
O ``<img>`` também funciona com arquivos tipo GIF.

<hr>

<h2>Áudio</h2>

Para adicionar áudio faça:

```
<audio controls>
	<source src="caminho-para-o-audio.mp3">
</audio>
```

Explicação do que esta acontecendo:
- A linha ``<audio></audio>`` é onde você declara o áudio, você pode, ao lado do primeiro "audio", colocar funções, como ``controls``, que faz com que aparece os controles para o áudio. Você pode também adicionar as seguintes funções ``autoplay``,``loop``, ``muted``. Também é boa pratica deixar outros tipos de faixa de áudio para caso o navegador do usuário não reconheça certos tipos de audio-files:
```
<audio controls>
	<source src="caminho-para-o-audio.mp3" type="audio/mpeg">
	<source src="caminho2.wav" type="audio/wav">
</audio>
```

Também é interessante especificar o tipo de file que é usando o ``type=""``.

<hr>

<h2>VÍDEOS</h2>
Para colocarmos vídeos utilizaremos:

```
<video controls autoplay muted loop>
	<source src="caminho-para-o-video.mp4" type="video/mp4">
	<source src="caminho-para-o-video.webm" type="video/webm">
</video>
```

Segue o mesmo naipe do áudio.

<hr>

<h3>FAVICON</h3>
Favicon é o ícone da página. Os tipos de arquivos utilizados são:
- .ico
- .png
- .gif
- .jpg
- .svg
A melhor dimensão é pelo menos 90px por 90px.
Para adicionar faça:
```head-do-HTML
<link rel="icon" type="image/jpg" href="./caminho-icone.jpg">
```

O ``rel=""`` especifica o tipo de relacionamento do link.

<hr>

<h3>TEXT FORMATING</h3>

Abaixo estão alguns tipos de formatação de texto em HTML:

<p>This is normal text</p>
<p>This is <b>bold</b> text</p>
<p>This is <i>italic</i> text</p>
<p>This is <u>underlined</u> text</p>
<p>This is <del>deleted</del> text</p>
<p>This is <big>big</big> text</p>
<p>This is <small>small</small> text</p>
<p>This is <sub>subscript</sub> text</p>
<p>This is <sup>superscript</sup> text</p>
<p>This is <tt>monospace</tt> text</p>
<p>This is <mark>marked</mark> text</p>
<hr>

<h3>SPAN and DIV</h3>
``Span`` é um inline container, ou seja, ele fica na linha em si.
Já o ``div`` é um block container, ele pega o bloco inteiro.

<span style="background-color: tomato">Esse é um texto com SPAN</span>
<div style="background-color: cyan">Esse é um texto em DIV</div>

<h5>SPAN</h5>
Lorem ipsum dolor sit amet. Ut tempora recusandae nam soluta cumque et galisum dolore eos doloremque provident? Eos suscipit repellat qui quia neque et natus beatae eum aspernatur rerum eum autem quia in libero blanditiis.
<span style="background-color: tomato">Et vero ullam 33 dolorem impedit ab itaque nemo 33 delectus dolores. Sit tenetur quos non necessitatibus dolorem hic Quis quia id adipisci quia.</span> Aut error fuga et dolorum odit ut rerum voluptatem et enim accusamus et commodi minus.

<h5>DIV</h5>
Lorem ipsum dolor sit amet. Ut tempora recusandae nam soluta cumque et galisum dolore eos doloremque provident? Eos suscipit repellat qui quia neque et natus beatae eum aspernatur rerum eum autem quia in libero blanditiis.
<div style="background-color: yellow">Et vero ullam 33 dolorem impedit ab itaque nemo 33 delectus dolores. Sit tenetur quos non necessitatibus dolorem hic Quis quia id adipisci quia.</div> Aut error fuga et dolorum odit ut rerum voluptatem et enim accusamus et commodi minus.

<hr>

<h3>LISTS</h3>
Temos 3 tipos de listas em HTML:
- Lista desorganizada
- Lista organizada
- Lista de descrição

<div>
<h5>Lista Desorganizada</h5>
<p>(Unordered List)</p>
</div>
faremos o seguinte:
```
<ul>
	<li>eggs</li>
	<li>milk</li>
	<li>coffee suplies</li>
	<ul>
		<li>coffee</li>
		<li>sugar</li>
		<li>creamer</li>
	</ul>
</ul>
```
Isso ficaria assim no site:

<hr>
<ul>
	<li>eggs</li>
	<li>milk</li>
	<li>coffee suplies</li>
	<ul>
		<li>coffee</li>
		<li>sugar</li>
		<li>creamer</li>
	</ul>
</ul>
<hr>
 Provando que você pode "Nestar" listas

<h5>Lista Ordenada</h5>
<p>Ordered List</p>
Fazemos do mesmo jeito do Unordered List, só que usando ``<ol></ol>``.

<h5>Lista Descrição</h5>
<p>Description List</p>

Fazemos da seguinte forma:

```
<dl>
	<dt>dragon</dt>
		<dd>A dragon is a magical legendary creature that appears in the folklore of multiple cultures worldwide.</dd>
		
	<dt>vampire</dt>
		<dd>A preternatural being, commonly believed to be a reanimated corpse, that is said to suck the blood of sleeping persons at night.</dd>
</dl>
```

Isso ficaria do seguinte jeito:

<dl style="border: 2px solid">
	<dt>dragon</dt>
		<dd>A dragon is a magical legendary creature that appears in the folklore of multiple cultures worldwide.</dd>
		
	<dt>vampire</dt>
		<dd>A preternatural being, commonly believed to be a reanimated corpse, that is said to suck the blood of sleeping persons at night.</dd>
</dl>

<hr>

<h3>TABLES</h3>

Para criar tabelas usaremos o ``<table>``, ``<tr>``, ``<th>`` e o ``<td>``.

```
<table>
	<tr>
		<th>Coluna1</th>
		<th>Coluna2</th>
		<th>Coluna3</th>
		<th>Coluna4</th>
		<th>Coluna5</th>
	</tr>
	<tr>
		<td>linha1</td>
		<td>linha2</td>
		<td>linha3</td>
		<td>linha4</td>
		<td>linha5</td>
	</tr>
</table>
```
Isso ficaria:

<table>
	<tr>
		<th>Coluna1</th>
		<th>Coluna2</th>
		<th>Coluna3</th>
		<th>Coluna4</th>
		<th>Coluna5</th>
	</tr>
	<tr>
		<td>linha1</td>
		<td>linha2</td>
		<td>linha3</td>
		<td>linha4</td>
		<td>linha5</td>
	</tr>
</table>

É possível formatar o texto também, colocando atributos no ``<tr>``. Como por exemplo o ``align="center"``:

<table border="1">
	<tr>
		<th>Coluna1</th>
		<th>Coluna2</th>
		<th>Coluna3</th>
		<th>Coluna4</th>
		<th>Coluna5</th>
	</tr>
	<tr align="center">
		<td>linha1</td>
		<td>linha2</td>
		<td>linha3</td>
		<td>linha4</td>
		<td>linha5</td>
	</tr>
</table>

Fica difícil de ver mas funciona xD.

``border=""`` ajusta o tamanho das linhas da borda da table.
É possível também alterar o tamanho das células usando o ``widht`` ou ``height``.

<hr>

<h3>BUTTON</h3>
Utilizaremos a tag ``<button></button>``. É bem simples:
```
<button>Click Me</button>
```
<button>Click Me</button>
É possivel fazer alterações nele usando atributos tambem, como ``font-size``, ``backgournd-color``, etc....

Para fazer com que ele jogue para outra página utilizamos o ``<a>``, também podemos usar ``JavaScript``, porém isso é mais pra frente.

<hr>

<h3>FORMS</h3>

<form action="index.php" method="POST" enctype="multipart/form/data">
		<label for="username">Username: </label>
		<input type="text" placeholder="Username" id="username" minlenght="3" maxlenght="50" required><br>

		<label for="password">Password: </label>
		<input type="password" id="password" required><br>

		<label for="email">Email: </label>
		<input type="email" id="email" placeholder="email@email.com"><br>

		<label for="phone">Phone: </label>
		<input type="phone" placeholder="35 999999999" pattern="[0-9]{2} [0-9]{9}"><br>

		<label for="birthday">Birthday: </label>
		<input type="date" id="birthday"><br>

		<label for="quantity">Quantity: </label>
		<input type="number" id="quantity" min="0" max='999'><br>

		<label for="title">Title:</label>

		<label for="Mr">Mr.</label>
		<input type="radio" id="Mr" value="Mr" name="title">
		<label for="Ms">Ms.</label>
		<input type="radio" id="Ms" value="Ms" name="title">
		<label for="PhD">PhD.</label>
		<input type="radio" id="PhD" value="PhD" name="title"><br>

		<label for="payment">Payment:</label>
		<select id="payment">
			<option value="visa">visa</option>
			<option value="mastercard">mastercard</option>
			<option value="elo">elo</option>
		</select><br>

		<label for="subscribe">subscribe</label>
		<input type="checkbox" id="subscribe"><br>

		<label for="comment">comment</label>
		<textarea id="comment" rows="3" cols="25"></textarea><br>

		<label for="file">file</label>
		<input type="file" id="file" accept="image/png, image/jpeg"><br>

		<input type="submit">
</form>


### Headers & Footers

<hr>

```
<header style="background-color: mediumpurple">
	<h1>Welcome to the Website</h1>
	<a href="">Home</a>
	<a href="">About us</a>
	<a href="">Contact us</a>
	<hr>
</header>

<main>
	<h4>Check out!!!</h4>
</main>

<footer style="background-color: mediumpurple">
	<hr>
	autor: XD<br>
	&copy; copyright reserved<br>
	<small><a href="mailto: Xexo@gmail.com">Xexp@gmail.com</a></small>
</footer>
```

Ficará assim:
<hr>
<header style="background-color: mediumpurple">
	<h1>Welcome to the Website</h1>
	<a href="">Home</a>
	<a href="">About us</a>
	<a href="">Contact us</a>
	<hr>
</header>

<main>
	<h4>Check out!!!</h4>
</main>

<footer style="background-color: mediumpurple">
	<hr>
	autor: XD<br>
	&copy; copyright reserved<br>
	<small><a href="mailto: Xexo@gmail.com">Xexp@gmail.com</a></small>
</footer>