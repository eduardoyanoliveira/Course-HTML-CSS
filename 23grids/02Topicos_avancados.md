# Tópicos Avançados em Grid

Na aula anterior, aprendemos os conceitos básicos do Grid e como criar um layout simples. Agora, vamos explorar tópicos mais avançados do Grid, como o alinhamento dos itens, o posicionamento automático de itens e a criação de layouts mais complexos.

1. Alinhamento dos Itens

O Grid oferece várias propriedades para controlar o alinhamento dos itens dentro das células do Grid. Algumas dessas propriedades incluem:

- ``justify-items``: define o alinhamento horizontal dos itens.
- ``align-items``: define o alinhamento vertical dos itens.
- ``place-items``: define o alinhamento horizontal e vertical dos itens em uma única propriedade.

Exemplo:

```css

.container {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-template-rows: 200px;
  justify-items: center;
  align-items: center;
}
```

Nesse exemplo, os itens do Grid serão centralizados tanto horizontalmente quanto verticalmente dentro das células.

2. Posicionamento Automático de Itens

O Grid também oferece a capacidade de posicionar automaticamente os itens, permitindo que eles se adaptem ao espaço disponível no layout. Isso é feito usando as propriedades ``grid-auto-rows`` e ``grid-auto-columns``.

Exemplo:

```css
.container {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-template-rows: 200px;
  grid-auto-rows: 100px;
  grid-auto-columns: 200px;
}
```

Nesse exemplo, os itens que não foram explicitamente posicionados ocuparão automaticamente uma altura de 100 pixels e uma largura de 200 pixels.

3. Grid Implícito e Explícito

No Grid, existem duas formas de definir as células: o grid implícito e o grid explícito. O grid explícito é definido por meio das propriedades ``grid-template-columns`` e ``grid-template-rows``, enquanto o grid implícito é criado automaticamente para preencher o espaço restante.

### Exemplo:

```css

.container {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-template-rows: 200px;
  grid-auto-columns: 200px;
  grid-auto-rows: 100px;
}
```

Nesse exemplo, definimos explicitamente duas colunas e uma linha, e as células restantes serão geradas automaticamente para preencher o Grid.

O Grid oferece uma variedade de recursos avançados para criar layouts complexos e responsivos. Na próxima aula, exploraremos a criação de layouts profissionais e técnicas avançadas com o Grid.