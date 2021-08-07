## Estrutura Básica de páginas HTML

Para se trabalhar com o HTML temos algumas tags básicas para uma boa formatação da página. Utilizaremos o HTML 5 como base.

```html
<!DOCTYPE html>
<html>
    <head>
        <title></title>
    </head>
    <body>
    </body>
</html>
```

### Doctype

```html
<!DOCTYPE HTML PUBLIC
	"-//W3C//DTD HTML 4.01//EN"
	"http://www.w3.org/TR/html4/strict.dtd"
>
```

É uma palavra especial, é um artefato histórico. Antigamente verificava se continha essa tag e se sim a página era exibida em standards mode

```html
<!DOCTYPE html>
```

Em html 5 não  é mais necessário usar toda a especificação. Ela informa ao navegador qual versão do HTML serã usada no documento. Doctype não é considerado uma tag de verdade, mas sim uma declaração. Ela teve estar presente sempre na primeira linha do documento.

### html

```html
<!DOCTYPE html>
<html lang="en">
</html>
```

É a tag que representa o elemento raiz (elemento de nível superior) de um documento HTML, por este motivo é chamado de elemento raiz. Todos os outros elementos devem ser descendentes deste elemento.

Utilizamos o "en" que vem da <a href="https://pt.wikipedia.org/wiki/ISO_639">ISO639-1 </a> . Essa espeficação de idioma ajuda nos mecanismos debusca e para programas de leitura de tela usado por pessoas com deficiências visuais.

### head

```html
<head>
	<meta charset="utf-8">
	<title>My fancy web page</title>
</head>
```
É a tag que contém metadados da página, como título <title></title> das páginas que é exibido na aba do browser ou na barra de título, ele pode conter somente texto. É no <head> onde inserimos também coisas como <meta> e planilhas de estilo. O charset="utf-8" fala qual as letras e caracteres que podem aparecer na página.

### body

```html
<body>
</body>
```

Representa o conteúdo de um documento HMTL. Pode existir somente um elemento <body> em um documento HTML. É nele que são exibidas as coisas para que as pessoas que visitam a página.

##### Exemplo de HTML

```html
<!DOCTYPE html> <!-- Indicando a versão do meu HTML -->
<html lang="en"> <!-- Dentro da tag HTML é que teremos o nosso site 
					  O atributo lang é importante para falar o idioma da página -->
    <head> <!-- Todas as configurações da página, informações para o browser -->
		<meta charset="UTF-8"> <!-- Informa qual é a configuração do conteúdo do site 
									UTF-8 suporta uma grande quantidade de caracteres -->
		<title>My fancy web page</title> <!-- Aparece no título do nosso site -->
	</head>
	<body> <!-- É onde colocamos o conteúdo do site -->
        <h1>Hello there.</h1>
	</body>
</html>
```

- tag <html> é a raiz / root

### Leitura complementar

- <a href="https://developer.mozilla.org/pt-BR/docs/Learn/HTML/Introduction_to_HTML/Getting_started">Introdução ao HTML no MDN</a>
- <a href="https://developer.mozilla.org/pt-BR/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML">O que á no head ?</a>
- <a href="https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/meta">O elemento meta no MDN</a>

