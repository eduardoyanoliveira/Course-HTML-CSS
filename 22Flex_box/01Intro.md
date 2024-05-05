# Flexbox

O Flexbox é utilizado para posicionar os elementos do documento, criando uma estrutura. Diferentemente de outras propriedades CSS, para utilizar o Flexbox, é necessário aplicar essas propriedades no elemento pai.

## ``display: flex;``

A propriedade display com o valor flex é a primeira propriedade a ser aplicada para utilizar o Flexbox. Ao aplicá-la, os elementos filhos se comportarão de maneira diferente.

Exemplo:

```css
.container {
    display: flex;
    height: 400px;
    border: 2px solid red;
}

.child {
    width: 200px;
    background-color: seagreen;
}
```

Ao aplicar a propriedade ``display: flex;``, todos os filhos da div com a classe "container" deixarão de se posicionar um abaixo do outro e ficarão um ao lado do outro.

A propriedade ``display: flex;`` significa que o elemento pai agora é um flex container e os elementos filhos são flex items.

## ``flex-direction``

Ao aplicar display: flex;, os elementos mudam sua orientação na tela. Para voltar à orientação padrão, "um abaixo do outro", e ainda continuar com o flex container, utilize a propriedade ``flex-direction`` com o valor column (o valor padrão é row, que posiciona os filhos um ao lado do outro). Lembre-se de que ao mudar a orientação do ``flex-direction``, o eixo do flex container será alterado.

### Valores possíveis:

- ``row-reverse``: inverte a ordem dos filhos e eles continuam um ao lado do outro.
- ``row``: padrão.
- ``column-reverse``: um abaixo do outro com a ordem alterada do último para o primeiro.

## ``flex-wrap``

Por padrão, os elementos filhos do flex container são reajustados de acordo com a largura do container. Portanto, se um elemento não couber no container, o flexbox irá diminuir sua largura. Isso é evidente quando diminuímos o tamanho da tela. No entanto, não é possível colocar elementos filhos com tamanho que ultrapasse o container.

Para mudar esse comportamento, podemos utilizar a propriedade ``flex-wrap`` com o valor wrap. Isso fará com que, quando o container não tiver tamanho suficiente para conter os filhos, eles sejam quebrados para a próxima linha.

## ``justify-content``

A propriedade ``justify-content`` posiciona os elementos dentro do container de acordo com a horizontal (ou vertical, se o eixo estiver invertido). Por exemplo, podemos centralizar os filhos no centro horizontal do container utilizando ``justify-content: center;``.

### Outros valores possíveis para justify-content incluem:

- ``start``: posiciona no começo do container.
- ``end``: posiciona no final do container.
- ``space-between``: coloca espaço entre os elementos filhos, empurrando um para cada canto.
- ``space-around``: coloca espaço ao redor dos elementos filhos.
- ``space-evenly``: coloca espaço ao redor dos elementos de forma mais equilibrada.


## ``align-items``

A propriedade ``align-items`` posiciona os elementos dentro do container de acordo com a vertical (ou horizontal, se o eixo estiver invertido). Ela possui as mesmas propriedades do ``justify-content``.

Exemplo:

```css
.container {
    display: flex;
    align-items: center;
}
```

Ao utilizar ``align-items: center;``, os elementos filhos serão alinhados verticalmente no centro do container.

### Outros valores possíveis para align-items incluem:

- ``flex-start``: alinha no início do container.
- ``flex-end``: alinha no final do container.
- ``baseline``: alinha pela linha de base.
- ``stretch``: estica os elementos para preencher o container verticalmente.

Essas são apenas algumas das propriedades básicas do Flexbox. Combinando-as e utilizando outras propriedades específicas do Flexbox, como ``flex-grow``, ``flex-shrink`` e ``flex-basis``, é possível criar layouts complexos e responsivos de maneira mais fácil e eficiente.

O Flexbox oferece um poderoso conjunto de ferramentas para a criação de layouts flexíveis e adaptáveis. É uma habilidade essencial para qualquer desenvolvedor front-end que deseja criar interfaces web modernas e responsivas. Com a prática e a experimentação, você poderá dominar o Flexbox e utilizá-lo de forma eficaz em seus projetos