# Flexbox: Layouts Clássicos e Técnicas Profissionais

No mundo do desenvolvimento web, o Flexbox é uma ferramenta poderosa para criar layouts flexíveis e responsivos. Nesta aula, vamos explorar layouts clássicos e técnicas profissionais usando o Flexbox.

## Layouts Clássicos

1. Layout de Colunas Simples

O layout de colunas simples é um dos usos mais básicos do Flexbox. Ele consiste em ter uma única coluna de conteúdo que se ajusta automaticamente ao tamanho do container.

### Exemplo:

```html
<div class="container">
  <div class="column">Coluna 1</div>
  <div class="column">Coluna 2</div>
  <div class="column">Coluna 3</div>
</div>
```

```css

.container {
  display: flex;
}

.column {
  flex: 1;
  margin: 10px;
  background-color: #e0e0e0;
}
```

Nesse exemplo, a propriedade ``flex: 1`` faz com que as colunas ocupem proporções iguais dentro do container. O resultado é um layout de colunas que se ajusta automaticamente.

2. Layout de Barra Lateral Fixa

O layout de barra lateral fixa é amplamente utilizado em sites e blogs, onde uma barra lateral permanece fixa enquanto o conteúdo principal rola.

### Exemplo:

```html
<div class="container">
  <div class="sidebar">Barra Lateral</div>
  <div class="content">Conteúdo Principal</div>
</div>
```

```css

.container {
  display: flex;
}

.sidebar {
  width: 200px;
  background-color: #e0e0e0;
}

.content {
  flex: 1;
  margin-left: 20px;
}
```

Nesse exemplo, a barra lateral tem uma largura fixa de 200px, enquanto o conteúdo principal ocupa o espaço restante no container devido à propriedade ``flex: 1.``

## Técnicas Profissionais

1. Layout Responsivo com Media Queries

Uma técnica profissional para criar layouts flexíveis é combinar o Flexbox com media queries. Isso permite ajustar o layout com base no tamanho da tela.

### Exemplo:

```css

.container {
  display: flex;
  flex-wrap: wrap;
}

.item {
  flex: 1 0 200px;
  margin: 10px;
}

@media screen and (max-width: 768px) {
  .item {
    flex-basis: 100%;
  }
}
```

Nesse exemplo, o layout se adapta quando a largura da tela é menor que 768px. Os itens passam a ocupar a largura total do container devido à propriedade ``flex-basis: 100%`` aplicada nas media queries.

2. Layouts com Alinhamento Avançado

O Flexbox também permite alinhamentos avançados dos elementos, como centralizar verticalmente e alinhar na base.

### Exemplo:

```css

.container {
  display: flex;
  justify-content: center;
  align-items: baseline;
}
```

Nesse exemplo, o ``justify-content: center`` centraliza os elementos horizontalmente e o ``align-items: baseline`` os alinha na base verticalmente.

3. Layout de Grade Flexível

O Flexbox é especialmente útil para criar layouts de grade flexíveis, onde os elementos se ajustam automaticamente em várias configurações de tela.

### Exemplo:

```html

<div class="grid-container">
  <div class="grid-item">Item 1</div>
  <div class="grid-item">Item 2</div>
  <div class="grid-item">Item 3</div>
  <div class="grid-item">Item 4</div>
</div>
```

```css

.grid-container {
  display: flex;
  flex-wrap: wrap;
}

.grid-item {
  flex: 1 0 200px;
  margin: 10px;
  background-color: #e0e0e0;
}
```

Nesse exemplo, o ``flex-wrap: wrap`` permite que os elementos sejam quebrados em várias linhas, caso não caibam em uma única linha. A propriedade ``flex: 1 0 200px`` define que os itens possuem uma base flexível de 200 pixels, mas podem crescer para preencher o espaço disponível.

4. Layouts Responsivos com Orientação Diferente

O Flexbox permite alterar a orientação do layout com facilidade, o que é útil para criar layouts responsivos com diferentes disposições.

### Exemplo:

```css

.container {
  display: flex;
  flex-wrap: wrap;
}

.item {
  flex: 1;
  margin: 10px;
}

@media screen and (max-width: 768px) {
  .container {
    flex-direction: column;
  }
}
```

Nesse exemplo, a disposição padrão é uma linha horizontal de elementos. No entanto, quando a largura da tela é menor que 768 pixels, a regra de media query ``flex-direction: column`` é aplicada, alterando o layout para uma coluna vertical.

Essas são apenas algumas das técnicas e layouts avançados que você pode criar com o Flexbox. O Flexbox oferece flexibilidade e controle sobre o posicionamento dos elementos, permitindo que você crie designs criativos e responsivos em seus projetos web.