# Atributos e Técnicas para Imagens

## Posicionamento de Imagens com float

Se você precisa posicionar uma imagem ao lado de um texto, é possível usar a propriedade ``float`` do CSS. Defina o valor de float como ``left`` ou ``right`` para posicionar a imagem à esquerda ou à direita do texto, respectivamente.

Exemplo:

```html

<img src="caminho/para/imagem.jpg" alt="Texto alternativo da imagem" style="float: left;">
<p>Texto que acompanha a imagem.</p>
```

## Imagem de Fundo e Repetição com CSS

Ao utilizar uma imagem como plano de fundo usando <i>CSS</i>, é comum que a imagem não preencha todo o tamanho da tela ou do contêiner, resultando no comportamento padrão de repetição da imagem para preencher todo o contêiner.

Para evitar esse comportamento de repetição, você pode usar a propriedade background-repeat do CSS e definir seu valor como ``no-repeat``.

Exemplo:

```css
.container {
  background-image: url('caminho/para/imagem.jpg');
  background-repeat: no-repeat;
}
```

Isso fará com que a imagem apareça apenas uma vez, deixando o restante do contêiner em branco.
Imagem de Fundo e Preenchimento com CSS

Para fazer com que a imagem de fundo ocupe todo o tamanho do contêiner, você pode usar a propriedade background-size com o valor ``cover``. Isso fará com que a imagem seja dimensionada proporcionalmente para cobrir todo o contêiner, sem distorções.

Além disso, você pode usar a propriedade background-position para definir a posição mais importante da imagem, ou seja, a parte que nunca deve ser cortada da tela. Geralmente, você pode definir seu valor como ``center``.

Para garantir que a imagem de fundo permaneça fixa no lugar à medida que o conteúdo é rolado, você também pode usar a propriedade ``background-attachment`` com o valor ``fixed``.

Exemplo:

```css

.container {
  background-image: url('caminho/para/imagem.jpg');
  background-size: cover;
  background-position: center;
  background-attachment: fixed;
}
```

Dessa forma, a imagem de fundo preencherá todo o contêiner, não perderá nenhuma parte importante e permanecerá fixa mesmo quando o conteúdo for rolado.