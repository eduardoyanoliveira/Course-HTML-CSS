# Listas

Em HTML, as listas são usadas para representar informações em formato de lista, como listas de produtos, listas de imagens, etc.

Muitas vezes, há a necessidade de usar listas em aplicações web, desde a criação de um menu com opções de navegação até a exibição de valores em uma lista na tela.

## Listas Ordenadas (Ordered List)

As listas ordenadas são comumente usadas para demonstrar eventos em ordem cronológica, ordenar itens por relevância, entre outros.

Para criar uma lista ordenada, siga estes passos:

1º Use a tag ``<ol>``. Essa tag será um contêiner para os itens da lista (o nome "ol" significa "ordered list").

2º Dentro da tag ``<ol>``, crie os itens da lista com a tag ``<li>``. Você pode usar quantas tags ``<li>`` forem necessárias, dependendo do tamanho da lista (o nome "li" significa "list item").

3º É possível afirmar que o próprio passo a passo acima, adotado para criar uma lista ordenada, é por si só uma lista ordenada.

Exemplo:

```html
<h2>Vendedores com maiores vendas no mês:</h2>
<ol>
  <li>Julia</li>
  <li>Robert</li>
  <li>Smith</li>
  <li>Maria</li>
  <li>Emilly</li>
</ol>
```

No exemplo acima, cada item da lista ``<li>`` receberá um número, que será aplicado de forma crescente de cima para baixo. O primeiro item terá o número 1, o segundo o número 2 e assim por diante, de maneira ordenada.

## Listas Desordenadas (Unordered List)

Às vezes, é necessário criar listas em que todos os elementos têm a mesma relevância, ou seja, os elementos não possuem uma ordem específica.

Para criar uma lista desordenada, substitua a tag ``<ol>`` pela tag ``<ul>``.

Exemplo:

```html

<h2>Vendedores com maiores vendas no mês:</h2>
<ul>
  <li>Julia</li>
  <li>Robert</li>
  <li>Smith</li>
  <li>Maria</li>
  <li>Emilly</li>
</ul>
```

Ao renderizar o exemplo acima, ao contrário do exemplo usado na lista ordenada, os itens da lista não receberão um número de ordem, mas um ponto. O ponto antes de cada item indica que os itens não possuem uma ordem específica.

As listas desordenadas são mais utilizadas do que as listas ordenadas, pois na maioria dos casos não é necessário criar uma hierarquia entre os itens, como ao criar um menu.

Também é possível remover o ponto da lista desordenada ou o número da lista ordenada usando CSS com a propriedade list-style: none.