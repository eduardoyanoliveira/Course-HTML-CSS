# Imagens no HTML e CSS

## Imagem no HTML: <img>

Para adicionar uma imagem em HTML, você pode usar a tag ``<img>``. Essa tag não possui uma tag de fechamento e tem dois atributos principais:

- ``src``: Esse atributo define a fonte da imagem, ou seja, o caminho para o arquivo de imagem que você deseja exibir.
- ``alt``: Esse atributo especifica o texto alternativo da imagem. É importante fornecer um texto descritivo aqui para acessibilidade e casos em que a imagem não pode ser carregada.

Exemplo:

``` html

<img src="caminho/para/imagem.jpg" alt="Texto alternativo da imagem">
```

## Imagem com CSS: background-image

Uma outra forma de exibir uma imagem no seu site é usando CSS. Para isso, você pode usar a propriedade background-image. Essa propriedade permite definir uma imagem como plano de fundo de um elemento HTML.

Exemplo:

```css

.seletor {
  background-image: url(caminho/para/imagem.jpg);
}
```

## Escolhendo entre HTML e CSS

A escolha de usar HTML ou CSS para adicionar uma imagem depende do propósito da imagem:

- Se a imagem é informativa e possui algum conteúdo relevante, como um gráfico ou uma foto, ela é considerada uma imagem semântica e deve ser inserida usando a tag ``<img>`` em HTML.
- Se a imagem é meramente ilustrativa e não possui um conteúdo informativo, como um ícone decorativo ou uma imagem de fundo, você pode adicioná-la usando CSS e a propriedade background-image.

## Tipos de arquivos de imagem

Existem vários formatos de arquivo de imagem com características diferentes. Alguns dos formatos mais comuns são:

- ``.jpg `` ``.jpeg``: Esses arquivos são ideais para imagens com muitas cores e compressão. Eles são amplamente usados para fotografias e imagens realistas.
- ``.png``: Esse formato também suporta uma ampla gama de cores, mas é especialmente útil quando você precisa de transparência em sua imagem. É comumente usado para logotipos e elementos gráficos com transparência.
- ``.gif``: O formato GIF também suporta transparência, mas geralmente tem uma qualidade menor em comparação com o formato PNG. É frequentemente usado para imagens animadas e elementos simples.
- ``.svg``: Esse formato é baseado em vetores, o que significa que as imagens SVG não perdem qualidade quando ampliadas. São ótimas para gráficos escaláveis, ícones e ilustrações.
- ``.webp``: Esse é um formato desenvolvido pelo Google que oferece alta compressão, resultando em arquivos menores e tempos de carregamento mais rápidos.

Cada formato de imagem tem suas próprias características e casos de uso adequados. É importante escolher o formato certo com base nas necessidades do seu projeto, considerando fatores como qualidade, tamanho do arquivo e suporte do navegador.