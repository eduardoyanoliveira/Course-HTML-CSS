# Seletores

Dentro do HTML, é frequentemente necessário acessar uma ou mais tags para aplicar estilos com CSS ou adicionar funcionalidades com JavaScript. Nesta seção, veremos alguns seletores e como eles são utilizados em conjunto com o CSS. Alguns desses seletores também podem ser usados com JavaScript.
Seletores por Elemento

Uma forma comum de selecionar uma tag no documento para aplicar estilos é pelo seu nome, conforme demonstrado no exemplo abaixo:

## Exemplo:

```html
<head>
    <style>
        p {
            color: blue;
        }
    </style>
</head>

<p>
    Primeiro parágrafo.
</p>

<div>
    <p> 
        Segundo parágrafo.
    </p>
</div>
```

No exemplo acima, ao utilizar o nome do elemento "p" no CSS, todos os elementos "p" do documento receberão a mesma estilização (cor do texto azul).
Encadeamento de Seletores

O encadeamento de seletores permite selecionar um elemento específico que é filho de outro elemento específico. Utilizando o exemplo acima, é possível usar o encadeamento de seletores para selecionar apenas o elemento "p" que é filho do elemento "div".

## Exemplo:

```html
<head>
    <style>
        div p {
            color: blue;
        }
    </style>
</head>

<p>
    Primeiro parágrafo.
</p>

<div>
    <p> 
        Segundo parágrafo.
    </p>
</div>
```

No exemplo acima, ao especificar "div p" no CSS, apenas o segundo parágrafo que está dentro do elemento "div" será estilizado.

É importante observar que, se houver outros encadeamentos de elementos (tags) no documento que correspondam ao padrão de seleção, esses elementos também serão selecionados. Ou seja, qualquer outra tag "p" que possua uma "div" como elemento pai também será selecionada.
Seleção Múltipla de Elementos (tags)

Uma outra possibilidade de seleção por meio de tags é a seleção múltipla, onde é possível aplicar uma estilização em mais de uma tag ao mesmo tempo. Para informar ao CSS quais tags receberão uma estilização em comum, basta separá-las por vírgulas.

## Exemplo:

```html
<head>
    <style>
        h1, p {
            color: purple;
        }
    </style>
</head>

<h1>
    Título.
</h1>

<div>
    <p> 
        Segundo parágrafo.
    </p>
</div>
```

No exemplo acima, tanto as tags "h1" quanto as tags "p" receberão a estilização que altera a cor do texto para roxo.

A seleção múltipla não se limita a tags. Ela também pode ser utilizada com outros elementos de seleção, como ids e classes (que serão abordados no próximo artigo).