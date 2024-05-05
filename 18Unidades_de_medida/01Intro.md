# Unidades de Medida

As unidades de medida são utilizadas no CSS para definir o tamanho de diversas propriedades dos elementos, como margem ``margin``, largura ``width``, altura ``height`` e preenchimento ``padding``.

## Tipos de Unidades de Medida Absolutas

As unidades de medida absolutas possuem um valor fixo que não será alterado, mesmo que o tamanho da tela ou do elemento pai seja modificado. Alguns exemplos dessas unidades são:

- ``Pixels (px)``: é a unidade de medida mais comumente utilizada, representando um único ponto na tela. Por exemplo, width: 200px; define a largura de um elemento como 200 pixels.

- ``Polegadas (in)``: representa uma polegada física. Por exemplo, font-size: 0.5in; define o tamanho da fonte como 0.5 polegadas.

- Entre outras unidades de medida absolutas, como centímetros (cm), milímetros (mm) e pontos (pt).

## Tipos de Unidades de Medida Relativas

As unidades de medida relativas são baseadas em outros elementos, adaptando-se às mudanças de tamanho. Alguns exemplos dessas unidades são:

- ``EM (em)``: faz com que um elemento se comporte com base no tamanho do elemento pai. Por exemplo, se uma div possui font-size: 20px; e um parágrafo (p) dentro dela possui font-size: 1.5em;, o parágrafo terá o tamanho de fonte de 30 pixels, pois é 1.5 vezes o tamanho da fonte do elemento pai. Para especificar metade do tamanho, pode-se usar font-size: 0.5em;.

- ``REM (rem)``: funciona de maneira semelhante ao EM, mas baseia-se no tamanho do elemento raiz (root) do documento (geralmente o elemento HTML), não no elemento pai.

- ``VW (viewport width)``: representa uma porcentagem da largura da janela de visualização (viewport). Por exemplo, width: 50vw; define a largura de um elemento como 50% da largura da janela de visualização.

- ``VH (viewport height)``: representa uma porcentagem da altura da janela de visualização. Por exemplo, height: 75vh; define a altura de um elemento como 75% da altura da janela de visualização.

- ``Porcentagem (%)``: determina o tamanho do elemento com base em uma porcentagem do tamanho do elemento pai. Por exemplo, se um elemento pai possui width: 100px; e um elemento filho possui width: 50%;, o valor do width do filho será de 50 pixels.

## Outras Unidades de Medida

Além das unidades de medida mencionadas acima, existem outras disponíveis no CSS. Recomenda-se consultar a documentação oficial do CSS ou fontes confiáveis para obter uma lista completa e detalhada dessas unidades de medida.

Lembre-se de escolher a unidade de medida apropriada para cada situação, levando em consideração a adaptabilidade do layout, a acessibilidade e a experiência do usuário.