# Introdução ao Grid

O Grid é um sistema de layout bidimensional que permite criar estruturas de grade flexíveis e alinhadas. Com o Grid, você pode organizar os elementos em linhas e colunas, proporcionando um controle preciso sobre o posicionamento e o alinhamento dos itens.

1. Definindo o Container do Grid

Para começar a usar o Grid, é necessário definir o container do Grid, que é o elemento pai dos itens que serão organizados na grade. Isso é feito aplicando a propriedade display: grid ao elemento.

### Exemplo:

```css

.container {
  display: grid;
}
```

2. Criando as Colunas e Linhas

Uma vez que o container do Grid está definido, você pode especificar o número de colunas e linhas desejadas. Isso é feito usando as propriedades ``grid-template-columns`` e ``grid-template-rows``, respectivamente.

### Exemplo:

```css
.container {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-template-rows: 100px 200px;
}
```

Nesse exemplo, definimos três colunas com largura igual (1fr) e duas linhas, uma com altura de 100 pixels e outra com altura de 200 pixels.

3. Posicionando os Itens no Grid

Uma vez que o Grid está definido, você pode posicionar os itens dentro dele. Existem várias formas de fazer isso, como usando as propriedades ``grid-column`` e ``grid-row`` ou as abreviações ``grid-area`` e ``grid-template-areas``.

### Exemplo:

```css

.container {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-template-rows: 100px 200px;
}

.item {
  grid-column: 2 / 4;
  grid-row: 1 / 3;
}
```

Nesse exemplo, o item está posicionado nas colunas 2 e 3 e nas linhas 1 e 2.

O Grid oferece uma variedade de propriedades e recursos para criar layouts avançados e responsivos. Nas próximas aulas, exploraremos tópicos mais avançados do Grid, como alinhamento, posicionamento automático de itens e criação de layouts complexos.