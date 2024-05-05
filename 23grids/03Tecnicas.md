# Layouts e Técnicas Profissionais com Grid

Na aula anterior, aprendemos sobre os tópicos avançados em Grid. Agora, vamos explorar a criação de layouts profissionais e aplicar técnicas avançadas com o Grid para criar designs flexíveis e responsivos.

1. Layouts em Grade

Uma das principais vantagens do Grid é a capacidade de criar layouts em grade complexos e personalizados. Combinando várias linhas e colunas, podemos criar diferentes áreas para posicionar e organizar elementos em nosso layout.

### Exemplo:

```css

.container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: repeat(2, 200px);
  gap: 20px;
}

.item {
  background-color: #f2f2f2;
  padding: 20px;
}
```

Nesse exemplo, criamos uma grade com 3 colunas e 2 linhas, cada uma com uma altura de 200 pixels. Os elementos dentro da grade serão espaçados por uma margem de 20 pixels.

2. Grid Áreas

Outra técnica poderosa do Grid é o uso de áreas. Podemos atribuir nomes às áreas específicas da grade e posicionar os elementos nessas áreas para criar layouts mais intuitivos e flexíveis.

### Exemplo:

```css

.container {
  display: grid;
  grid-template-columns: 1fr 2fr;
  grid-template-rows: repeat(3, 200px);
  gap: 20px;
  grid-template-areas:
    "header header"
    "sidebar main"
    "footer footer";
}

.header {
  grid-area: header;
}

.sidebar {
  grid-area: sidebar;
}

.main {
  grid-area: main;
}

.footer {
  grid-area: footer;
}
```

Nesse exemplo, definimos áreas nomeadas para o cabeçalho, a barra lateral, o conteúdo principal e o rodapé. Em seguida, usamos a propriedade ``grid-area`` para posicionar os elementos nas áreas desejadas.

3. Responsividade com Grid

Uma das grandes vantagens do Grid é sua capacidade de criar layouts responsivos de maneira fácil e eficiente. Podemos usar as propriedades do Grid, como ``grid-template-columns`` e ``grid-template-rows``, juntamente com a unidade de medida fr, para criar layouts fluidos que se ajustam automaticamente ao tamanho da tela.

### Exemplo:

```css

.container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  grid-template-rows: repeat(2, 200px);
  gap: 20px;
}
```

Nesse exemplo, usamos a função ``repeat`` juntamente com ``auto-fit`` e minmax para criar colunas fluidas que têm um tamanho mínimo de 200 pixels e se ajustam automaticamente ao espaço disponível.

Essa abordagem permite que o Grid se adapte de forma inteligente a diferentes dispositivos e tamanhos de tela. À medida que a largura do ``contêiner`` diminui, o Grid automaticamente ajusta o número de colunas para preencher o espaço disponível, mantendo o layout responsivo.

Além disso, podemos usar media queries para ajustar ainda mais o layout com base em breakpoints específicos.

### Exemplo:

```css

.container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: repeat(2, 200px);
  gap: 20px;
}

@media (max-width: 768px) {
  .container {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (max-width: 480px) {
  .container {
    grid-template-columns: 1fr;
  }
}
```

Nesse exemplo, definimos breakpoints em 768 pixels e 480 pixels usando media queries. Quando a largura da tela estiver abaixo de 768 pixels, o Grid será alterado para ter duas colunas. E quando a largura estiver abaixo de 480 pixels, teremos uma única coluna.

Essas técnicas nos permitem criar layouts flexíveis e adaptáveis, garantindo que nosso conteúdo seja apresentado da melhor forma em diferentes dispositivos e tamanhos de tela.

## Técnicas Profissionais com Grid

Ao dominar as funcionalidades básicas do Grid, podemos explorar técnicas mais avançadas e profissionais para criar layouts complexos e dinâmicos. Nesta aula, vamos explorar algumas dessas técnicas.

1. Grid com Níveis de Aninhamento

Uma das vantagens do Grid é sua capacidade de criar layouts com vários níveis de aninhamento. Podemos criar subgrids dentro de grids existentes, permitindo layouts mais detalhados e flexíveis.

### Exemplo:

```css

.container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: repeat(2, 200px);
  gap: 20px;
}

.subgrid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-template-rows: repeat(3, 1fr);
  gap: 10px;
}
```

Nesse exemplo, criamos um subgrid dentro de uma célula do grid principal. O subgrid possui duas colunas e três linhas, e pode conter seu próprio conteúdo e estilos. Essa técnica é útil quando queremos criar layouts mais complexos, com elementos agrupados e organizados em diferentes áreas.

2. Posicionamento Manual de Elementos

Além do fluxo padrão do Grid, também podemos posicionar manualmente os elementos em células específicas usando as propriedades ``grid-row`` e ``grid-column``.

### Exemplo:

```css

.item {
  grid-row: 2 / 4;
  grid-column: 2 / 4;
}
```

Nesse exemplo, o elemento com a classe .item será posicionado nas células das linhas 2 a 4 e das colunas 2 a 4 do Grid. Essa técnica nos dá controle total sobre a posição dos elementos e é útil quando queremos criar layouts personalizados e não dependemos do fluxo automático do Grid.

3. Alinhamento Preciso com Grid

O Grid também oferece recursos avançados de alinhamento que nos permitem controlar a posição dos elementos com precisão.

Podemos utilizar as propriedades ``justify-self`` e ``align-self`` para alinhar horizontalmente e verticalmente os elementos individualmente dentro de suas células.

### Exemplo:

```css
.item {
  justify-self: center;
  align-self: end;
}
```

Nesse exemplo, o elemento com a classe .item será centralizado horizontalmente e alinhado na parte inferior verticalmente dentro de sua célula.


4. Grid para Posicionamento Visual

Uma técnica interessante é utilizar o Grid não apenas para o posicionamento estrutural, mas também para o posicionamento visual dos elementos. Podemos criar áreas vazias no Grid e usar essas áreas para criar espaçamento entre elementos ou para criar elementos de sobreposição.

Exemplo:

```css

.container {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-template-rows: repeat(3, 100px);
}

.item {
  grid-column: 2 / 4;
  grid-row: 2 / 3;
}
```

Nesse exemplo, criamos uma célula vazia no canto superior esquerdo do Grid e posicionamos o elemento com a classe .item nas células 2 a 3 das colunas 2 a 4. Essa técnica pode ser usada para criar espaçamento visual entre elementos, criar áreas de destaque ou até mesmo para criar elementos de sobreposição, como menus e modais.

5. Grid com Animações e Transições

Uma combinação poderosa é usar o Grid juntamente com animações e transições CSS para criar efeitos visuais dinâmicos e interativos.

Podemos aplicar animações e transições em propriedades como ``grid-column`` e ``grid-row ``para criar transições suaves entre diferentes layouts ou para animar o posicionamento dos elementos no Grid.

Exemplo:

```css
.item {
  grid-column: 1 / 3;
  transition: grid-column 0.3s ease-in-out;
}

.item:hover {
  grid-column: 2 / 4;
}
```

Nesse exemplo, quando o elemento com a classe .item é hover, a propriedade ``grid-column`` é animada suavemente, criando um efeito de transição entre duas posições do Grid. Essa técnica pode ser usada para adicionar interatividade aos layouts e melhorar a experiência do usuário.

6. Grid Responsivo

Assim como o Flexbox, o Grid também pode ser usado para criar layouts responsivos. Podemos usar as media queries para alterar a estrutura do Grid em diferentes tamanhos de tela e dispositivos.

### Exemplo:

```css

.container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: 200px;
}

@media (max-width: 768px) {
  .container {
    grid-template-columns: 1fr;
  }
}
```

Nesse exemplo, o Grid é definido com três colunas no layout padrão, mas quando a largura da tela for menor que 768px, ele é alterado para uma única coluna. Isso permite que o layout se ajuste de acordo com o tamanho da tela e garante uma boa experiência em dispositivos móveis.

Essas são apenas algumas das técnicas profissionais que podem ser aplicadas com o Grid. A medida que você ganha mais experiência e conhecimento, é possível explorar ainda mais recursos e funcionalidades para criar layouts avançados e personalizados.