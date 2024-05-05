# Box-Sizing e Box-Model

No HTML, todos os elementos se comportam como uma caixa. O tamanho total do elemento é a soma de sua largura ou altura, mais sua borda e margem interna.

## O Problema com o Padding

Quando adicionamos um padding a um elemento, o tamanho total do elemento é afetado. Vamos considerar um elemento <div> com uma largura de 150px e uma altura de 100px. Se adicionarmos um padding de 25px, o elemento passará a ter uma largura de 200px e uma altura de 150px. Isso ocorre porque, por padrão, o HTML adiciona o padding ao tamanho do elemento.

## O Que é o Box-Sizing?

O ``box-sizing`` é uma propriedade CSS que permite controlar como o tamanho total de um elemento é calculado. Ao alterar o valor do ``box-sizing`` para ``border-box``, o comportamento padrão é removido.

Com o valor ``border-box``, o tamanho total do elemento é definido pela largura e altura que você especificou, incluindo o padding e a border. Isso significa que o ``padding`` e a ``border`` são incluídos dentro do tamanho total do elemento, em vez de serem adicionados a ele.

## Por que Usar o Box-Sizing: Border-Box?

O uso do ``box-sizing: border-box`` é comum em desenvolvimento web, pois oferece algumas vantagens importantes:

    Simplifica o cálculo do layout: Ao usar border-box, você pode especificar tamanhos fixos para elementos, levando em conta o espaço ocupado pela padding e border. Isso simplifica o cálculo do layout e facilita o alinhamento de elementos.

    Evita quebras de layout: Com o border-box, o padding e a border não são adicionados ao tamanho total do elemento. Isso evita que elementos adjacentes sejam empurrados para baixo ou para os lados quando padding e border são aplicados.

    Melhora a responsividade: Ao usar border-box, você pode definir a largura dos elementos de forma precisa, considerando o espaço ocupado pelo padding e border. Isso é especialmente útil para criar layouts responsivos, onde os elementos devem se adaptar a diferentes tamanhos de tela.

## Aplicando o Box-Sizing

Para aplicar o ``box-sizing: border-box`` a todos os elementos em seu documento HTML, você pode usar o seguinte código CSS:

```css

* {
  box-sizing: border-box;
}
```

Esse código define o ``box-sizing: border-box`` como o valor padrão para todos os elementos. É comum colocar esse código no início do arquivo CSS principal do seu site ou aplicação.

Ao usar o ``box-sizing: border-box``, você terá mais controle sobre o tamanho e o layout dos elementos em seu documento HTML, tornando o desenvolvimento mais eficiente e evitando problemas comuns de quebras de layout.