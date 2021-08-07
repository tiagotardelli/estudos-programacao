## Listas no HTML

Dentro do HTML podemos trabalhar com listas ordenadas e listas não ordenadas, onde essas são contituídas de itens de lista, porém temos um terceiro tipo que são as listas de definições que não são constituidas de itens de lista.

Listas ordenadas e não ordenadas são constituidas de itens de lista, e a marcação é virtualmente idêntica. As listas ordenadas são utilizados no caso que necessitamos de uma ordem e as não ordenadas para onde esta ordem não importa.

```html
<h1>Filmes de 1978</h1>

<h2>Filmes de maior bilheteria (EUA)</h2>
<ol> <!-- Lista ordenada (com numeração)  -->
    <li>Grease - Nos Tempos da Brilhantina</li>
    <li>Superman</li>
    <li>Clube dos Cafajestes</li>
    <li>Doido para Brigar... Louco para Amar</li>
    <li>O Diabo Disse Não</li>
</ol>

<h2>Indicadores para melhor filme</h2>
<ul> <!-- Lista não ordenada (em tópicos) -->
    <li>Expresso da Meia-noite</li>
    <li>O paraíso Pode Esperar</li>
    <li>O Franco Atirador</li>
    <li>Amargo Regresso</li>
    <li>Uma Mulher Descasada</li>
</ul>
```

A lista ordenada contém alguns atributos que a lista não ordenada não têm.

```html
<h2>Filmes de maior bilheteria (EUA)</h2>
<ol start="6"> <!-- Atributo para iniciar a lista a partir do número apontado -->
    <li>Hooper, o Homem das Mil Façanhas</li>
    <li>Tubarão 2</li>
    <li>A Vingança da Pantera Cor-de-Rosa</li>
	<li>O Franco Atirador</li>
    <li>Halloween - O Inpicio</li>
</ol>

<h2>Top 5</h2>
<ol reversed> <!-- Atributo booleno para inverter a lista. Os valores são opcionais se colocar o valor ele deve ter o mesmo nome do atributo <ol reversed=¨reversed¨> -->
    <li>O Paraíso</li>
    <li>Doido para Brigar... Louco para Amar</li>
    <li>Clube dos Cafajestes</li>
    <li>Superman</li>
    <li>Grease - Nos Tempos da Brilhantina</li>
</ol>

<h2>Top 5</h2>
<ol type=¨I¨> <!-- Pode-se fazer a alteração para algarismos romanos ou letras ao invés de números. Para algorismos romanos coloque "I" para maiúsculos e "i" para minúsculos. Para letras "A" para maiúsculos e "a" para minúsculas -->
    <li>Introdução</li>
    <li>Elenco</li>1
    <li>Resumo do enredo</li>
    <li>Pontos Fortes</li>
    <li>Pontos Fracos</li>
    <li>Conclusão</li>
</ol>
```

Os itens da listas também possuem atributos

```html
<h1>Filmes com a maioria dos prêmios da Academia</h1>
<ol>
    <li>Ben-Hur (empate)</li> <!-- Podemos usar a abordagem no value para repitir um valor e após ele a lista prossegue com a contagem -->
    <li value="1">Titanic (empate)</li>
    <li value="1">O Retorno do Rei (empate)</li>
    <li value="4">Amor, Sublime Amor</li>
</ol>
```

Podemos ordenar uma lista dentro de outra

```html
<h1>Review de Roger Ebert's sobre Grease - Nos Tempos da Brilhantina</h1>
<ol type="I">
    <li>Introdução</li>
    <li>Elenco
        <ul>
            <li>Olivia Newton-John</li>
            <li>John Travolta</li>
        </ul>
    </li>
    <li>Resumo de enredo</li>
    <li>Pontos Fortes</li>
    <li>Pontos Fracos</li>
    <li>Conclusão</li>
</ol>
```

Leitura complementar

- [Listas em HTML no w3schools](https://www.w3schools.com/html/html_lists.asp)
- [Listas não ordenadas no MDN](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/ul)
- [Listas ordenadas no MDN](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/o)
- [Listas de itens no MDN](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/li)
- [Listas de pares de termos e descrições no MDN](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/dl)
