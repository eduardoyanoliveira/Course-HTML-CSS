# Identificadores

No tópico de seletores, outra forma de selecionar elementos no documento HTML é atribuindo um identificador à tag.

A necessidade de adicionar um identificador a uma tag surge principalmente em duas situações.

A primeira situação é quando é necessário selecionar apenas um elemento dentro do documento, não sendo possível realizar esse processo utilizando apenas o nome da tag, especialmente se houver várias tags iguais no documento.

A segunda situação em que os identificadores são necessários é quando é preciso selecionar vários elementos de tags diferentes ao mesmo tempo. Por exemplo, se o desenvolvedor desejar alterar o tamanho da fonte de dois textos diferentes no site, como parágrafos e títulos.

## ID

No caso de selecionar apenas um elemento dentro do documento, utiliza-se o atributo "id". O "id" pode ser adicionado a qualquer tag dentro da tag "body" e deve ser único. Ou seja, não podem existir duas tags com o mesmo valor para o atributo "id".

O valor do atributo "id" é escolhido pelo desenvolvedor e deve ser curto, descritivo e facilmente identificável.

Para selecionar um ID tanto no CSS quanto no JavaScript, utiliza-se o símbolo de jogo da velha (hashtag) seguido pelo nome do ID.

Exemplo:

```html
<head>
    <style>
        #first-msg {
            color: blue;
        }
    </style>
</head>

<h1 id="first-msg">
    Primeiro parágrafo.
</h1>

<p>
    Segundo parágrafo.
</p>
```

No exemplo acima, apenas a primeira tag "p" que possui o ID com o valor "first-msg" será estilizada com a cor azul do texto.
Classes

Outra forma de identificar elementos dentro de um documento HTML é utilizando o atributo "class". A diferença entre "id" e "class" é que o atributo "class" pode ser reutilizado em outros elementos. Para classificar igualmente dois elementos dentro do documento, basta atribuir o mesmo valor ao atributo "class".

Para selecionar um atributo "class", utiliza-se um ponto seguido pelo valor do atributo.

Exemplo:

```html
<head>
    <style>
        .title {
            color: red;
        }
    </style>
</head>

<h1 class="title">
    Título.
</h1>

<h2 class="title">
    Subtítulo.
</h2>
```

Neste exemplo, ambos os elementos das tags "h1" e "h2" serão estilizados com a cor vermelha do texto. Isso ocorre porque ambos possuem o atributo "class" com o mesmo valor.

## Nível Hierárquico

Em casos onde um elemento possui tanto um ID quanto uma classe, e ambos são selecionados no CSS com valores diferentes para a mesma propriedade, o CSS presente no ID terá sempre prioridade sobre a classe.

Exemplo:

No exemplo abaixo, a cor do texto do parágrafo será azul:

```html
<head>
    <style>
        #test-id {
            color: blue;
        }
        .test-class {
            color: red;
        }
    </style>
</head>
<body>
    <p id="test-id" class="test-class">Lorem ipsum dolor sit amet consectetur adipisicing elit. Cum accusamus officiis quis quibusdam soluta, quas nisi veritatis. Error qui inventore ex dicta eveniet, doloremque facilis temporibus amet nam molestiae facere.</p>
</body>
```

Nesse exemplo, mesmo que a classe "test-class" atribua a cor vermelha ao texto, o ID "test-id" tem prioridade e a cor do texto será azul.

É importante entender que a especificidade do seletor também desempenha um papel na resolução de conflitos entre estilos, além da ordem de declaração dos estilos no CSS.

Os identificadores e classes são recursos poderosos para selecionar e estilizar elementos de forma precisa e flexível em um documento HTML. Ao dominar o uso de seletores por ID e classe, você terá maior controle sobre o estilo e o comportamento dos elementos em suas páginas web.