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