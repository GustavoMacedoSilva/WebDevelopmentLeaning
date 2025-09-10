
### Introdução

3 jeitos de aplicar CSS: Inline, Internal e External

Inline:

```
<body style="background-color: black">
	<h1 style="color: white">This is my website</h1>
	
	<p style="color: white">xexo1</p>
	<p style="color: white">xexo2</p>
	<p style="color: white">xexo3</p>
	<p style="color: white">xexo4</p>
</body>
```

Internal:

```
<!DOCTYPE html>

<html lang="en">

<head>

    <meta charset="UTF-8">

    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Document</title>
    <style>
	    body{
		    background-color: red;
	    }
	    h1{
		    color: blue;
	    }
	    p{
		    color: black;
	    }
    </style>

</head>

<body>
	<h1>This is my website</h1>
		
		<p>xexo1</p>
		<p>xexo2</p>
		<p>xexo3</p>
		<p>xexo4</p>
</body>

</html>
```

External:

Criamos um arquivo novo .css, colocamos la oque queremos mudar e no html usamos:

```
<!DOCTYPE html>

<html lang="en">

<head>

    <meta charset="UTF-8">

    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Document</title>
    <link rel="stylesheet" href="caminho-ate-o-arquivo.css">

</head>

<body>

</body>

</html>
```

No arquivo css faremos:

```CSS
body{
	background-color: black;
}
h1{
	color: white;
}
#p1{
	color: red;
}
#p2{
	color: orange;
}
.odd{
	color: red;
}
```
Utilizamos o ``#`` para apontar para elementos com aquele ``id``. Para aplicar em classes utilizamos o ``.`` (ponto).