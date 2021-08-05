## HTML (Linguagem de Marcação de Hipertexto) 

#### O que é ?

O HTML fornece uma forma estruturada de criar páginas web. Com as tags disponibilizadas pelo HTML podemos controlar o que o browser (navegador) interpreta para exibir para o usuário.

<a href="https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element" >Referência de Elementos/Tags HTML</a>

### Tags

As tags são utilizadas dentro dos sinais de menor que (<) e maior que (>), porém a tag de fechamento leva o caractere "/" (o browser reconhece como fechamento). Em sua grande maioria as tags de abertura e fechamento são correspondentes. 

```html
<h1>Meu nome é ...</h1>
```

As tags podem também estar aninhadas umas dentro das outras.

```html
<div>
	<p>Parágrafo</p>
</div>

<div>
    <p>Carro</p>
    <p>Moto</p>
    <p>Avião</p>
</div>
```

As tags usam atributos para adicionar funcionalidades ou descrever comportamentos.

Algumas tags têm fechamento próprio. Essas tags normalmente não envolvem algum conteúdo. A tag <img> é uma tag de fechamento próprio. Como você pode ver, ainda há uma "/" no final da tag. Observe também o uso dos atributos.

```html
<img src="caminho/para/arquivo/de/imagem.jpg" alt="descrição da imagem" />
```

 
