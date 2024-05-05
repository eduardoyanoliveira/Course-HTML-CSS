# Introdução ao HTML - Aulas sobre Tags e Atributos

&nbsp; Nesta aula introdutória, vamos explorar as tags e atributos no HTML, que são fundamentais para a marcação de uma página web. As tags HTML são representadas por palavras-chave que são colocadas entre os símbolos de maior e menor ``<tag>``. É importante observar que, ao contrário da tag de abertura, a tag de fechamento possui uma barra invertida após o símbolo de menor ``</tag>``.

## Tags

&nbsp;As tags são usadas para estruturar e formatar o conteúdo de uma página HTML. Elas fornecem uma forma de organizar e categorizar diferentes partes do documento. Vamos analisar alguns exemplos de tags populares:

* ``<p>`` (parágrafo): Essa tag é utilizada para criar um parágrafo de texto. Todo o conteúdo dentro da tag <p> será exibido como um parágrafo no navegador. Por exemplo:

```html
<p>
    Este é apenas um parágrafo de exemplo!
</p>
```

* ``<h1>`` até ``<h6>`` (cabeçalhos): Essas tags são usadas para criar títulos e cabeçalhos de diferentes níveis. O ``<h1>`` é o cabeçalho mais importante, enquanto o ``<h6>`` é o menos importante. Por exemplo:

```html
<h1>Título Principal</h1>
<h2>Subtítulo</h2>
```
* ``<div>`` (divisão): Essa tag é usada para agrupar elementos e criar seções distintas na página. Ela não possui um significado semântico específico, mas é amplamente utilizada para fins de estilização e organização. Por exemplo:


```html
<div>
    <h3>Seção 1</h3>
    <p>Conteúdo da seção 1</p>
</div>
```

```html
<div>
    <h3>Seção 2</h3>
    <p>Conteúdo da seção 2</p>
</div>
```
    
* ``<a>`` (âncora): Essa tag é usada para criar links para outras páginas ou recursos. Ela possui um atributo "href" que especifica o destino do link. Por exemplo:

```html
<a href="https://www.exemplo.com">Visite o nosso site!</a>
```

&nbsp; Esses são apenas alguns exemplos das tags mais comumente utilizadas no HTML. Existem muitas outras tags disponíveis para atender a diferentes necessidades e propósitos.

## Atributos

As tags HTML podem receber atributos, que fornecem informações adicionais sobre as tags ou controlam seu comportamento. Os atributos são inseridos dentro da tag de abertura e possuem um nome e um valor, separados por um sinal de igual. Vamos explorar alguns atributos comuns:

* class: Esse atributo é usado para especificar uma ou mais classes CSS para um elemento. As classes podem ser usadas para aplicar estilos específicos aos elementos. Por exemplo:

```html
<p class="destaque">Este é um parágrafo com destaque</p>
```

* id: Este atributo é usado para atribuir um identificador único a um elemento HTML. O ID é usado principalmente para fins de manipulação do elemento por meio de JavaScript ou como alvo para links de âncora. Um ID deve ser exclusivo dentro de um documento HTML. Por exemplo:

```html
<h1 id="titulo-principal">Título Principal</h1>
```

&nbsp; No exemplo acima, o ID "titulo-principal" é atribuído ao cabeçalho de nível 1 (h1), permitindo que seja referenciado especificamente em scripts ou links.

* src: Este atributo é usado para especificar a origem (URL) de um recurso, geralmente usado em elementos de imagem ou vídeo. O valor do atributo "src" deve ser o caminho para o arquivo de imagem ou vídeo. Por exemplo:


```html
<img src="imagem.jpg" alt="Imagem de exemplo">
```

&nbsp; Neste exemplo, o atributo "src" é usado para especificar a localização da imagem "imagem.jpg" a ser exibida na página.

* href: Este atributo é usado para especificar o destino de um link em um elemento de âncora (<a>). O valor do atributo "href" deve ser um URL válido para a página ou recurso que você deseja vincular. Por exemplo:

```html
<a href="https://www.exemplo.com">Visite o nosso site!</a>
```

No exemplo acima, o atributo "href" é usado para definir o link para o site "https://www.exemplo.com".

Esses são apenas alguns exemplos de atributos comuns no HTML. Existem muitos outros atributos disponíveis, cada um com sua própria finalidade e efeito. Aprender a utilizar adequadamente os atributos é fundamental para criar páginas web interativas e funcionais.

## Atributos multi-valorados

&nbsp; Além disso, alguns atributos podem ter valores compostos, que consistem em um ou mais valores dentro do mesmo atributo. Vejamos um exemplo com a tag ``<div>``:

```html
<div class="container card">
```

Neste exemplo, o atributo "class" possui o valor "container card". Isso significa que o elemento ``<div>`` terá as classes "container" e "card", que podem ser usadas para estilizar o elemento com CSS.

    Dica: Ao utilizar atributos em suas tags HTML, é importante seguir as boas práticas e garantir que os valores atribuídos sejam relevantes e adequados ao contexto da página.

Espero que essas explicações sobre tags e atributos no HTML tenham sido úteis para você. Continue explorando e praticando para aprimorar suas habilidades de desenvolvimento web!