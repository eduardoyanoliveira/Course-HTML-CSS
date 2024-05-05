# Listas 

&nbsp; Listas em HTML são utilizadas tal como listas normais. Como por exemplo lista de produtos, lista de imagens, etc. 

&nbsp; Muitos podem ser os motivos que levam a necessidade de utilização de uma lista em uma aplicação web. Desde a necessidade de criar uma lista de opções em menu para o usuário navegar pelo site, até listas comuns de valores que precisam ser apresentados na tela.


## Listas Ordenadas (Ordered List)

&nbsp; Listas ordenadas são comumente utilizadas para demonstrar eventos em espaço de tempo lienear, ordenar items por sua relevância, tal como outras necessidades.

&nbsp; Para Criar uma lista ordenada é necessário implementar os seguintes passos:

1º Deve-se utilizar a tag "ol". Esta tag será uma tag container, isto é, ela conterá os items da lista.(o nome da tag "ol" significa "ordered list")

2º Dentro da tag "ol" deve-se criar os itens da lista com a tag "li". Pode-se utilizar quantas tags li's necessárias de acordo com o tamanho da lista.(o nome da tag "li" significa "list item")

    - É possível afirmar que o próprio passo a passo acima adotado para criar uma lista ordenada, é por si só também uma lista ordenada. 


### Exemplo

```
    <h2> Vendedores com maiores vendas no mês: </h2> 
    <ol>
        <li> Julia </li>
        <li> Robert </li>
        <li> Smith </li>
        <li> Maria </li>
        <li> Emilly </li>
    </ol>
```

&nbsp; Quando renderizado o exemplo acima é possível notar que cada item da lista (li) receberá um número. O número será aplicado de forma crescente de cima para baixo. Logo o primeiro item terá o número 1, o segundo o número 2, e assim por diante de maneira ordenada.


## Lista Desordenada (unordered list)

&nbsp; Durante a utilização do HTML deve-se lembrar que a maioria das tags possuem também um peso semântico, que pode mudar o comportamento do browser, sistemas de buscas, etc. 

&nbsp; Em vista da semântica, muita das vezes pode ser necessário criar listas onde todos os elementos possuem a mesma relevância. Isto é, que os elementos não possuam ordem.

&nbsp; Para realizar a criação de uma lista sem ordem deve-se utilizar a tag "ul" no lugar da tag "ol".


### Exemplo

```
    <h2> Vendedores com maiores vendas no mês: </h2> 
    <ul>
        <li> Julia </li>
        <li> Robert </li>
        <li> Smith </li>
        <li> Maria </li>
        <li> Emilly </li>
    </ul>
```

&nbsp; Ao renderizar o exemplo acima, ao contrário do exemplo utilizado no tópico de lista ordenada, os items da lista não receberão um número de ordenação e sim um ponto. O ponto antes de cada item representa que o item não possui uma ordem.

&nbsp; Listas desordenadas são mais utilizadas do que listas ordenadas, pois não maioria dos casos não é desejado criar uma hierárquia entre os items. Como por exemplo ao criar um menu.

&nbsp; Também é possível remover tanto o ponto da lista desordenada quanto o número da lista ordenada via CSS utilizando a propriedade "list-style: none".
