# Herança de Propriedades no CSS

No CSS, algumas propriedades são herdadas por padrão pelos elementos filhos. Isso significa que, ao aplicar uma propriedade a um elemento pai, essa propriedade será passada para seus elementos filhos.

Por exemplo, ao definir uma cor em uma ``<div>`` e essa ``<div>`` possuir vários elementos ``<p>`` como filhos, todos os elementos ``<p>`` terão a mesma cor:

```css
div {
  color: red;
}

div p {
  /* a cor será herdada do elemento pai (div) */
}
```

Da mesma forma, a propriedade ``font-size`` também é herdada. Se definirmos um tamanho de fonte em uma ``<div>``, os elementos ``<p>`` dentro dessa ``<div>`` terão o mesmo tamanho de fonte:

```css
div {
  font-size: 14px;
}

div p {
  /* o tamanho de fonte será herdado do elemento pai (div) */
}
```

No entanto, nem todas as propriedades são herdadas automaticamente. Por exemplo, a cor de um link ``<a>`` não será herdada do elemento pai. É necessário aplicar diretamente a cor desejada ao link.

```css
div {
  color: red;
}

div a {
  /* a cor do link não será herdada do elemento pai (div) */
  color: blue;
}
```

Além disso, é possível controlar explicitamente a herança de propriedades. Podemos forçar a herança especificando que o valor da propriedade é ``inherit``, o que significa que o valor será herdado do elemento pai:

```css
div {
  color: red;
  font-size: 14px;
}

div p {
  color: inherit; /* herda a cor do elemento pai (div) */
  font-size: inherit; /* herda o tamanho de fonte do elemento pai (div) */
}
```

Por outro lado, se quisermos remover a herança e definir uma propriedade de volta ao seu valor inicial, podemos usar ``initial``:

```css
div {
  color: red;
  font-size: 14px;
}

div p {
  color: initial; /* remove a herança e define a cor de volta ao valor inicial */
  font-size: initial; /* remove a herança e define o tamanho de fonte de volta ao valor inicial */
}
```

É importante consultar a documentação do CSS para saber quais propriedades são herdadas por padrão e quais exigem a aplicação direta em cada elemento.

Essa é uma noção fundamental para entender como as propriedades são propagadas e afetam a estilização dos elementos em uma estrutura de árvore no HTML.