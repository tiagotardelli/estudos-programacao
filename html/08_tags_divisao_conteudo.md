## Tags de divisão de conteúdo

### Tag article

Reṕresentado pela tag <article> representa uma composição completa ou independente em uma página. Pode ser uma postagem num fórum, um artigo de revista ou jornal, um post de um blog ou mesmo um comentário de um usuário.

Quando as tags <article> são aninhados, os elementos internos represtam artigos que estão relacionados ao conteúdo do artigo externo. Por exemplo, os comentários do  post de um blog, podem ser implementados com a tag article.

```html
<article>
	<header>
        <h1>A Primeira Regra da Vida</h1>
        <p><time>3 dias atrás</time></p>
    </header>
    
    <p>Se houver um microfone perto de você, assuma-o</p>

	<footer>
    	<a href="#">Mostrar comentários...</a>
    </footer>
</article>
```

### Leitura Complementar

- [Tag article do HTML 5](https://www.youtube.com/watch?v=rUmkpuRNTgM)

### Tag section

Representa uma seção genérica de uma página. Uma seção, neste contexto, é um agrupamento temático do conteúdo, por exemplo, uma seção de serviços.

```html
<!-- Capítulos de um livro, seções de uma tese, uma página web com uma parte para a introduçao,uma para post e outra para informações de contato -->

<article>
	<p>A maça é o fruto da macieira.</p>
    <section>
    	<h1>Maça vermelha</h1>
        <p>Essas maças vermelhas brilhantes são as mais comumente 
            encontradas na maioria dos supermercados.</p>
    </section>
    <section>
    	<h1>Maça-verde</h1>
        <p>Essas maças verdese suculentas fazem um ótimo recheio para 
            tortas de maça.</p>
    </section>
</article>

<!-- Podemos montar seções para listas -->
<!DOCTYPE hmtl>
<html lang="pt-BR">
    <head>
        <title>Cerimônia de Graduação Verão 2022</title>
    </head>
    <body>
        <h1>Graduação</h1>
        <section>
        	<h1>Cerimônia</h1>
            <p>Procissão de Abertura</p>
            <p>Discurso do Orador da Turma</p>
            <p>Discurso do Presidente da Turma</p>
            <p>Apresentação dos Diplomas</p>
            <p>Discurso de Fechamento do Diretor</p>
        </section>
        <section>
            <h1>Graduados</h1>
            <ul>
                <li>Molly Carpneter</li>
                <li>Anastasia Luccio</li>
                <li>Ebenezar McCov</li>
            </ul>
        </section>
    </body>
</html>

<!-- Exemplo de uso simples -->
<!-- ANTES -->
<div>
    <h2>Cabeçalho</h2>
    <p>Amontoado de conteúdos</p>
</div>
<!-- DEPOIS -->
<section>
    <h2>Cabeçalho</h2>
    <p>Amontoado de conteúdos</p>
</section>
```

O elemento <section> é utilizado para um corte genérico, indica-se usar somente se não houver um elemento específico, como é o caso da tag <nav> que utilizamos para menu de navegação. O elemento <article> deve ser utilizado sempre que o conteúdo for considerado como uma unidade atômica autônoma.

### Leitura Complementar

- [Tag section do HTML 5](https://www.youtube.com/watch?v=Y_lv0Zl09Eo)
