# Transformações 2D no CSS

As transformações 2D são efeitos utilizados para alterar a posição e a aparência de um elemento. Vamos explorar algumas das principais transformações 2D disponíveis no CSS.

## Rotação ``rotate()``

Para girar um elemento em um ângulo específico, utilizamos a propriedade transform com a função rotate(). Dentro dos parênteses, informamos o ângulo de rotação desejado em graus.

```css
div {
  width: 200px;
  height: 100px;
  background-color: green;
  transform: rotate(90deg);
}
```

Nesse exemplo, a ``<div>`` será rotacionada em 90 graus.

## Eixo de Rotação ``transform-origin``

É possível alterar o ponto de rotação de um elemento utilizando a propriedade transform-origin. Com ela, especificamos o eixo x e y do ponto de rotação.

```css
div {
  width: 200px;
  height: 100px;
  background-color: green;
  transform: rotate(90deg);
  transform-origin: left top;
}
```

Nesse caso, o ponto de rotação será o canto superior esquerdo do elemento.

## Torção ``skew()``

A transformação ``skew()`` é utilizada para torcer um elemento ao longo do eixo x ou y. Ela também recebe um valor em graus para definir a intensidade da torção.

```css
div {
  width: 200px;
  height: 100px;
  background-color: green;
  transform: skew(30deg, -15deg);
}
```

Nesse exemplo, a ``<div>`` será torcida em 30 graus ao longo do eixo x e em -15 graus ao longo do eixo y.

## Escala ``scale()``

A transformação ``scale()`` é usada para aumentar ou diminuir o tamanho de um elemento. Ela recebe valores em porcentagem, variando de 0 a 1, onde 1 representa o tamanho original do elemento.

```css
div {
  width: 200px;
  height: 100px;
  background-color: green;
  transform: scale(1.5, 0.8);
}
```

Nesse caso, a ``<div>`` será aumentada em 150% no eixo x e reduzida em 20% no eixo y.

Essas são apenas algumas das transformações 2D disponíveis no CSS. É possível combinar várias transformações para criar efeitos mais complexos. Consulte a documentação do CSS para explorar mais opções e aprofundar-se no assunto.