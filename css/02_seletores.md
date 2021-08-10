## Seletores

São utilizados para direcionar elementos HTML em nossas páginas da web que queremos estilizar. O seletor é a primeira parte de uma regra CSS. É um padrão de elementos e outros termos que informam ao navegador quais elementos HTML devem ser selecionados para que os valores de propriedade dentro da regra seja aplicados a eles.

```css
h1{
    color: blue
    background-color: yellow;
}

p {
    color: red;
}
```

#### Tipos de Seletores

Existem alguns agrupamentos diferentes de seletores:

- Seletores por nome de elemento

  ```css
  a{
      color: red
  }
  ```

- Seletores por classe

  ```css
  .titulo{
      /* declarações aqui */
  }
  ```

- Seletores por ID

  ```css
  #tituloUnico{
      /* declarações aqui */
  }
  ```

- Seletores por atributo

  Os elementos HTML podem ter atributos que fornecem mais detalhes sobre o elemento que está sendo marcado. Em CSS, você pode usar seletores de atributo para estilizar elementos com determinados atributos.

  - Seletores de presença e valor

    Esses seletores permitem a seleção de um elemento com base na presença de um atributo sozinho (por exemplo, href) ou mesmo através do atributo juntamente com o valor desse.

    ![Alt](/home/tiagotardelli/Projetos/estudos-programacao/repositorio/imagens/seletores_presenca_valor_css.jpg)

    ```css
    /* Usando li[class] pode-se combinar qualquer seletor com atibuto de classe. Isso corresponde a todos os itens da lista, exceto o primeiro */
    li[class] {
        front-size: 200%;
    }
    /* li[class="a"] corresponde a um seletor com uma classe de a, mas não a um seletor com uma classe de a com outra classe separada por espaço como parte do valor. Ele seleciona o segundo item da lista */
    lin[class="a"]{
        background-color: yellow;
    }
    
    /* li[class~="a"] corresponderá a uma classe a, mas também a um valor que contém a classe de a como parte de uma lista separada por espaços em branco. Ele seleciona o segundo e o terceiro item da lista. */
    li[class~="a"]{
        color: red;
    }
    ```

    ```html
    <h1>Attribute presence and value selectors</h1>
    <ul>
        <li>item l</li>
        <li class="a">Item 2</li>
        <li class="a b">Item 3</li>
        <li class="ab">Item 4</li>
    </ul>
    ```

    ![Alt](/home/tiagotardelli/Projetos/estudos-programacao/repositorio/imagens/exemplo_seletores_presenca_valor_css.jpg)

    - Seletores de substring

      Esses seletores permitem uma correspondência mais avançada de substring dentro do valor do seu atributo. Por exemplo, se você tivesse classes de box-warning e box-error e quisesse combinar tudo que começou com a string "box-", você podeira usar [class^="box-"]  para selecionar os dois (ou class|="box"] como descrito abaixo)

      ![Alt](/home/tiagotardelli/Projetos/estudos-programacao/repositorio/imagens/seletores_substring_css.jpg)

      ```css
      /* li[class^="a"] corresponde a qualquer valor de atributo que comece com a, portanto, corresponde aos dois primeiros itens da lista. */
      li[class^="a"]{
          font-size: 200%;
      }
      
      /* li[class$="a"] corresponde a qualquer valor de atributo que termina com a, portanto, corresponde ao primeiro e terceiro item da lista */
      li[class$="a"]{
          background-color: yellow;
      }
      
      /* li[class*="a"] corresponde a qualquer valor de atributo onde a aparença em qualquer lugar na string, portanto, corresponde a todos os itens da nossa lista */
      li[class*="a"] {
          color: red;
      }
      ```

      ```html
      <h1>Attribute sibstring matching selectors</h1>
      <ul>
          <li class="a">Item 1</li>
          <li class="ab">Item 2</li>
          <li class="bca">Item 3</li>
          <li class="bcabc">Item 4</li>
      </ul>
      ```

      ![Alt](/home/tiagotardelli/Projetos/estudos-programacao/repositorio/imagens/exemplo_seletores_substring_css.jpg)

      - Se você deseja combinar valores de atributo sem distinção entre maiúsculas e minúsculas, você pode usar o valor i antes do colchete de fechamento. Este sinalizador informa ao navegador para corresponder caracteres ASCII sem distinção entre maiúsculas e minúsculas. Sem o sinalizador, os valores serão correspondidos de acordo com a distinção entre maiúsculas e minúsculas do idioma do documento - no caso do HTML, será sensível a maiúsculas e minúsculas.

        ```css
        /* li[class^="a"] corresponde a um valor que começa com um "a" minúsculo */
        li[class^="a"]{
            background-color: yellow;
        }
        
        /* li[class^="a" i] corresponde a um valor que começa com um "a" independente de ser maiúsculo ou minúsculo */
        li[class^="a" i]{
            color: red;
        }
        ```

        ```html
        <h1>Case-insensitivity</h1>
        <ul>
            <li class="a">Item 1</li>
            <li class ="A">Item 2</li>
            <li class ="Ab">Item 3</li>
        </ul>
        ```

        ![Alt](/home/tiagotardelli/Projetos/estudos-programacao/repositorio/imagens/exemplo2_seletores_substring.jpg)

        

### Leitura Complementar

- [Seletores CSS](https://developer.mozilla.org/pt-BR/docs/Learn/CSS/Building_blocks/Selectors)

