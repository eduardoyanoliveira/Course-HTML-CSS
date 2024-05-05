# Display - Elementos de Nível de Bloco e de Linha

Os elementos em HTML podem ser classificados em elementos de nível de bloco e elementos de nível de linha. Essa classificação define como os elementos ocupam espaço na página e se geram quebras de linha.

## Elementos de Nível de Bloco

Os elementos de nível de bloco ocupam por padrão toda a largura disponível em uma linha e geram uma quebra de linha antes e depois deles. Alguns exemplos de elementos de nível de bloco são:

- ``<p>``: parágrafos de texto.
- ``<h1> - <h6>``: títulos de diferentes níveis.
- ``<ul>``: listas não ordenadas.
- ``<ol>``: listas ordenadas.
- ``<li>``: itens de listas.
- ``<footer>``: rodapé do documento.
- ``<div>``: um contêiner genérico.

Esses elementos ocupam toda a largura disponível e são usados para estruturar e organizar o conteúdo da página.

## Elementos de Nível de Linha

Os elementos de nível de linha não geram quebras de linha e ocupam apenas o espaço necessário para o conteúdo que eles contêm. Alguns exemplos de elementos de nível de linha são:

- ``<a>``: links.
- ``<span>``: marcações de texto genéricas.
- ``<em>``: ênfase no texto.
- ``<i>``: texto em itálico.
- ``<img>``: imagens.

Esses elementos não geram quebras de linha e são usados para aplicar estilos e marcações específicas dentro de outros elementos.

## Alterando o Comportamento com a Propriedade display

Para alterar o comportamento padrão dos elementos, podemos utilizar a propriedade CSS display. Essa propriedade permite definir se um elemento se comportará como um elemento de nível de bloco ou de linha.

- ``display: inline``: faz com que o elemento se comporte como um elemento de nível de linha, sem gerar quebras de linha. Ele ocupará apenas o espaço necessário para o conteúdo.
- ``display: block`` : faz com que o elemento se comporte como um elemento de nível de bloco, ocupando toda a largura disponível e gerando quebras de linha antes e depois dele.
- ``display: inline-block`` : combina características de elementos de nível de linha e de bloco. O elemento ocupa apenas o espaço necessário, mas também respeita as propriedades do ``box-model``, como margens e preenchimentos.

Além disso, existem outras propriedades relacionadas ao display:

- ``display: none``: retira completamente o elemento do DOM (Document Object Model), fazendo com que ele não seja exibido nem ocupe espaço na página.
- ``visibility: hidden``: esconde o elemento, mas ainda ocupa espaço na página. Ele permanece no DOM e pode ser revelado posteriormente.

Essas propriedades do display permitem controlar o comportamento dos elementos e ajustar sua exibição de acordo com as necessidades do layout e do design da página.