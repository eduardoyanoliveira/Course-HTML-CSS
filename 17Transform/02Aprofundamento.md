# Transformações 2D e 3D no CSS

As transformações no CSS permitem alterar a posição, rotação, escala e perspectiva de elementos em uma página web. Podemos dividir as transformações em 2D e 3D, cada uma com suas respectivas propriedades e efeitos.

## Transformações 2D

As transformações 2D são usadas para manipular elementos em um plano bidimensional.

### Rotação ``rotate()``

A função ``rotate()`` é usada para girar um elemento em um ângulo específico. O valor do ângulo é especificado em graus. Veja o exemplo abaixo:

```css
div {
  transform: rotate(45deg);
}
```

Nesse caso, a ``<div>`` será girada em 45 graus no sentido horário.

### Escala ``scale()``

A função ``scale()`` permite aumentar ou reduzir o tamanho de um elemento. Os valores especificados em porcentagem determinam a escala horizontal (eixo X) e vertical (eixo Y) do elemento. Veja o exemplo:

```css
div {
  transform: scale(1.5, 0.8);
}
```

Nesse exemplo, a ``<div>`` será aumentada em 150% no eixo X e reduzida em 20% no eixo Y.

### Translação ``translate()``

A função ``translate()`` é usada para mover um elemento ao longo dos eixos X e Y. Os valores especificados representam as distâncias horizontais e verticais em pixels ou porcentagem. Veja o exemplo:

```css
div {
  transform: translate(50px, 20px);
}
```

Nesse exemplo, a ``<div>`` será movida 50 pixels para a direita e 20 pixels para baixo.

## Transformações 3D

As transformações 3D permitem manipular elementos em um espaço tridimensional, adicionando profundidade e perspectiva.

### Rotação 3D ``rotate3d()``

A função ``rotate3d()`` permite rotacionar um elemento em um espaço tridimensional. Os valores especificados representam os componentes X, Y e Z do vetor de rotação. Veja o exemplo:

```css
div {
  transform: rotate3d(1, 1, 1, 45deg);
}
```

Nesse exemplo, a ``<div>`` será rotacionada em torno de um vetor diagonal (1, 1, 1) em 45 graus.
Perspectiva (perspective)

A propriedade perspective define a perspectiva tridimensional para os elementos filhos de um elemento pai. Ela determina a distância a partir da qual os elementos são vistos. Veja o exemplo:

```css
.container {
  perspective: 800px;
}

.container div {
  transform: rotateY(45deg);
}
```

Nesse caso, todos os elementos ``<div>`` dentro de um elemento com a classe .container serão rotacionados em torno do eixo Y em 45 graus, levando em consideração uma perspectiva definida de 800 pixels.

Esses são apenas alguns exemplos de transformações 2D e 3D disponíveis no CSS. Experimente combinar diferentes transformações e propriedades para criar efeitos visuais interessantes em seus elementos. Lembre-se de que as transformações podem ser animadas usando transições ou animações CSS, o que permite criar efeitos de movimento suaves e interativos em sua página web. Explore mais sobre as transformações no CSS e divirta-se criando elementos visualmente dinâmicos e cativantes!