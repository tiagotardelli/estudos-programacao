## Elementos de Bloco e Em Linha

Você deve sempre alinhas os seus elementos dentro um dos outros fechando as tags adequadamente. Quando fazemos esse tipo de abordagem o elemento externo recebe o nome de pai e o interno de filho.

```html
<p>
    Aqui <em>tem</em> teste!
</p>
```

Podemos também ter o alinhamento onde o <body> é o pai, o parágrafo <p> é seu filho e a citação <cite> é a filha do parágrafo, ou seja, a citação é neta do body.

```html
<body>
    <p>
        Quero escutar <cite>Capital Inicial!</cite>
    </p>
</body>
```

Para os demais níveis da estrutura não utilizamos como bisavô para marcação, o que é mais usual é apenas chamar de ancestrais e descendentes. O elemento <html> é ancestral de todos os elementos da página e todos os elementos são descendentes do elemento <html>.

Com a vinda do HTML 5 temos uma reclassificação dos elementos de HTML o qual dificultou um pouco as coisas, com isso devemos conhecer primeiramente os elementos usados nas versões anteriores, pois estes obdecem a regras não nos permitindo utilizar elementos de forma desordenada. 

Primeiramente devemos compreender que podemos usar elementos a nível de bloco (começam em uma nova linha e preeenchem toda a largura de seu container) e elementos em linha (podem iniciar e terminar no meio de uma linha). Exemplos:

```html
-- Exemplo de bloco
<h1>
    Digite aqui o seu título
</h1>

-- Exemplo de linha
<strong>Texto Aqui</strong>
```

Uma das principais regras são:

- Elementos de linha podem estar dentro de elementos de bloco;
- Elementos de linha podem estar dentro de elementos de linha;
- Elementos de bloco podem, em alguns casos, estar dentro de elementos de bloco;
- Elementos de bloco não podem estar dentro de elementos de linha;
- Elementos de bloco são aceitos dentro de um parágrafo <p> ou dentro de títulos de <h1> a <h6>.

A divisão de conteúdo, conhecida com <div> é um elemento sem significado semântico, por este motivo ele serve como container para outros elementos. Ele é um elemento a nível de bloco e pode conter qualquer outro elemento dentro de seu corpo. Este elemento tem sua maior serventia quando trabalhamos com CSS. Também existem ocasiões que ele pode ser utilizado em linha, em caso de necessitar do uso de CSS em uma linha.

### Leitura complementar

- <a href="https://developer.mozilla.org/pt-BR/docs/Web/HTML/Inline_elements">Elementos Inline no MDN</a>
- <a href="https://developer.mozilla.org/pt-BR/docs/Web/HTML/Block-level_elements">Elementos em Nível de Bloco no MDN</a>

