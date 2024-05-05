# Tag ``<picture>``

A tag ``<picture>`` é utilizada quando a imagem faz parte do conteúdo e desejamos fornecer diferentes versões da imagem para diferentes tamanhos de tela ou resoluções. Ela permite que especificemos múltiplas fontes de imagem e o navegador irá escolher a mais adequada para exibir.

### Exemplo básico de uso da tag ``<picture>``:

```html
<picture>
    <source media="(min-width: 480px)" sizes="33vw" type="image/png"
            srcset="images/large.jpg 1280w">
    <source sizes="100vw"
            srcset="images/outra_imagem_large.jpg 820w">
    <img src="images/img.png">
</picture>
```

Neste exemplo, temos duas fontes de imagem dentro da tag ``<picture>``, especificadas através das tags ``<source>``. A primeira fonte de imagem é escolhida quando a largura mínima da tela é de 480px ou mais, e o tamanho da imagem será de 33% da largura da viewport (33vw). A segunda fonte de imagem é escolhida para todos os outros casos, e o tamanho da imagem será de 100% da largura da viewport (100vw).

Cada ``<source>`` pode especificar um atributo srcset contendo uma lista de URLs de imagens separados por vírgulas. Também podemos adicionar o atributo type para informar o tipo de arquivo da imagem.

É importante mencionar que a tag ``<img>`` no final é obrigatória e será exibida caso nenhuma das fontes de imagem dentro da tag ``<picture>`` seja suportada pelo navegador.

Você pode obter mais informações sobre a tag ``<picture>`` na documentação oficial do MDN: Elemento ``<picture>`` (em inglês)

- A utilização da tag ``<picture>`` juntamente com a especificação do tamanho e tipo de imagem através dos atributos ``srcset`` e ``sizes`` é uma abordagem recomendada para garantir uma melhor responsividade das imagens em diferentes dispositivos e resoluções de tela.

```html

<picture>
    <source media="(min-width: 768px)" sizes="50vw" type="image/jpeg"
            srcset="images/grande.jpg 1200w">
    <source media="(min-width: 480px)" sizes="33vw" type="image/jpeg"
            srcset="images/medio.jpg 800w">
    <source sizes="100vw" type="image/jpeg"
            srcset="images/pequeno.jpg 400w">
    <img src="images/default.jpg" alt="Imagem padrão">
</picture>
```

Neste exemplo, estamos utilizando a tag ``<picture>`` para garantir a responsividade da imagem em diferentes dispositivos e resoluções de tela. Temos três fontes de imagem especificadas dentro da tag ``<picture>``, cada uma utilizando a tag ``<source>``.

- A primeira fonte de imagem é escolhida quando a largura mínima da tela é de 768px ou mais. O tamanho da imagem será de 50% da largura da viewport (50vw). Estamos utilizando o formato JPEG e o arquivo de imagem grande.jpg com uma largura de 1200 pixels.
- A segunda fonte de imagem é escolhida quando a largura mínima da tela é de 480px ou mais. O tamanho da imagem será de 33% da largura da viewport (33vw). Estamos utilizando o formato JPEG e o arquivo de imagem medio.jpg com uma largura de 800 pixels.
- A terceira fonte de imagem é escolhida para todos os outros casos. O tamanho da imagem será de 100% da largura da viewport (100vw). Estamos utilizando o formato JPEG e o arquivo de imagem pequeno.jpg com uma largura de 400 pixels.

Caso nenhuma das fontes de imagem seja suportada pelo navegador, a tag ``<img>`` será exibida, utilizando o arquivo de imagem default.jpg como imagem padrão e com um texto alternativo "Imagem padrão".

Este exemplo ilustra como a tag ``<picture>`` e os atributos ``srcset`` e ``sizes`` permitem que você forneça diferentes versões da imagem com base no tamanho da tela e resolução, garantindo uma melhor responsividade.