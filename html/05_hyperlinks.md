## HTML Hyperlinks

O hyperlink, ou apenas link, serve para que possamos ser direcionados para outra página do mesmo site ou para outro site ou até mesmo para fazer o download de um arquivo. Para isso usamos o elemento <a>

```html
<!-- Utilizamos o atributo href para indicar o caminho que pode ser uma URL ou um fragmento de URL -->

 <!-- exemplo com URL -->
<a href="about.hml">Sobre nós</a>

<!-- exemplo com fragmento ele aponta para um elemento específico na página se utilizando do elemento id. O browser irá rolar a página até o elemento correspondente -->
<a href="#products">Produtos</a> 
<h2 id="products">Nossos Produtos</h2>

<!-- Pode-se colocar o # no final de uma URL para linkar para um elemento de outra pãgina -->
<a href="about.html#founders">Fundadores</a>

<!-- Você pode linkar para o topo da página que está usando # ou #top sem a necessidade de ter um elemento com id "top" -->
```

Pode-se se usar o link com praticamente tudo, menos com outro link. Links se comportam como elementos de linha, mas mesmo assim é possível colocar um elemento em nível de bloco dentro de um link.

```html
<!-- Exemplo com apenas o texto clicável -->
<h1>
    <a href="https://www.google.com">Google</a>
</h1>

<!-- Exemplo com todo o h1 clicável -->
<a href="https://www.google.com">
	<h1>Google</h1>
</a>
```

3Os links têm vários atributos além do href

```html
<!-- Temos o atributo target onde a maioria dos seus valores tem a ver com frames. O valor principal que trabalhamos é com o _blank para que abra o link em uma nova aba ou janela que é util para manter o usuário em nossa página (CUIDADO!!! Ele sempre força esse comportamento) -->
<a href="https://www.google.com" target="_blank">Google</a>

<!-- Podemos usar o rel="noopener" para resolver um problema de segurança de origem cruzada -->
<a href="https://www.google.com" target="_blank" rel="noopener">Google</a>
```

### Leitura Complementar

- [HTML tag <a>](https://www.w3schools.com/tags/tag_a.asp)
- [O elemento âncora](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/a)
- [Sobre rel=noopener](https://mathiasbynens.github.io/rel-noopener/)

