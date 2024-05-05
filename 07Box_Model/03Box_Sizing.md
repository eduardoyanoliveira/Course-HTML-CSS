# Box-Sizing

Em HTML, todos os elementos se comportam como uma caixa, onde o tamanho total do elemento é a soma de sua largura ou altura, mais sua borda e margem interna.

```html

<head>
  <style>
    #container {
      width: 250px;
      height: 250px;
      background-color: cornflowerblue;
      padding: 30px;
    }
  </style>
</head>
<body>
  <div id="container"></div>
</body>
```

No exemplo acima, o elemento ``<div>`` com ``id="container"`` terá uma largura e altura de <i>310px</i>. Isso ocorre porque, além dos <i>250px</i> definidos na propriedade width, são adicionados <i>30px</i> de padding acima e abaixo.

Caso o elemento possua uma borda, a espessura da mesma também será somada ao tamanho final do elemento.

O tamanho final do elemento, incluindo sua borda, padding e margem interna, é chamado de box-model e representa o espaço ocupado pelo elemento na viewport.

## Box-Sizing: Border-Box

Na maioria dos casos, é desejável que o padding não seja somado ao tamanho total do elemento, pois isso pode quebrar o layout da aplicação.

Ao configurar a propriedade CSS box-sizing com o valor ``border-box``, é possível alterar o comportamento padrão no qual a borda e o padding são somados ao tamanho do elemento.

```css

div {
  box-sizing: border-box;
}
```

Ao utilizar ``box-sizing: border-box``, a largura e altura especificadas para o elemento incluirão o conteúdo, padding e borda, sem exceder esse tamanho. Isso facilita o controle do layout e evita problemas de dimensionamento.

## Resetando Valores Padrão

É comum que os desenvolvedores front-end removam as configurações padrões de margem, padding e box-sizing em todos os elementos HTML. Isso é conhecido como "reset" ou "normalização" de estilos.

```css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
```

O código acima redefine os valores padrão de margem e padding para zero, além de configurar ``box-sizing: border-box`` para todos os elementos. Essa prática ajuda a evitar inconsistências entre os navegadores e permite um controle mais preciso do layout.

Normalmente, esse código é adicionado no início do arquivo principal de CSS do site ou aplicação.

Dominar o conceito de ``box-sizing`` e utilizar adequadamente a propriedade box-sizing pode facilitar o desenvolvimento de layouts coesos e previsíveis, evitando surpresas indesejadas relacionadas ao dimensionamento e espaçamento dos elementos.