## CSS (Cascading Style Sheets)

CSS (Folha de Estilo em Cascata) é o que utilizamos para dar estilo para nossas páginas. Ela não é uma linguagem de programação e sim uma linguagem de estilização, ele permite aplicar estilos seletivamente a elementos em documentos HTML

```css
/* Selecionar todos os elemento parágrafo <p> e tornar o texto em vermelho */
p {
    color: red;
}
```

### Estrutura do CSS

![Alt](/home/tiagotardelli/Projetos/estudos-programacao/repositorio/imagens/estrutura_css.jpg)

#### Selector(Seletor)

Aqui é onde colocamos o nome do elemento HTML. Ele seleciona o(s) elementos(s) a serem estilizados.

#### Property(Propriedades)

Serve para alterar as propriedades do elemento HTML colocando um novo estilo.

#### Property Value(Valor da Propriedade)

O valor da propriedade é onde selecionamos uma dentre muitas aparências possíveis para uma determinada propriedade.

#### Declaretion(Declaração)

Uma regra simples como color: red; epecificando quais das propriedades do elemento você quer utilizar.

#### Outras partes importantes da sintaxe:

- cada linha de comando deve ser envolvida em chaves({}).
- dentro de cada declaração para separar a propriedade de seus valores deve-se usar dois pontos (:).
-  dentro de cada conjunto de regras para separar cada declaração da próxima deve-se usar ponto e vírgula (;).

```css
p {
    color: red;
    width: 500px;
    border: 1px solid black;
}

/* Podemos selecionar várias categorias de elementos e aplicar um único conjunto de regras */
p, li, h1 {
    color: red;
}
```

### Leituras Complementares

- [O que realmente é CSS?](https://developer.mozilla.org/pt-BR/docs/Learn/Getting_started_with_the_web/CSS_basics)
- [Como CSS é estruturado](https://developer.mozilla.org/pt-BR/docs/Learn/CSS/First_steps/How_CSS_is_structured)



