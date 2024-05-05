# Seletores

&nbsp; Os artigos anteriores delatlham alguns do tipos de seletores comumente utilizados no HTML. Este artigo tem como intuito apresentar alguns seletores que apesar de não tão comuns, por vezes se tornam muito úteis no dia a dia de desenvolvimento.

## Adjacent sibling combinator. (Irmão Adjacente)

&nbsp; O seletor Adjacent sibling combinator permite selecionar um elemento html que seja irmão direto de outro elemento específico. 

### Sintaxe

&nbsp; Para utilizar este seletor, deve-se:
 
1º Informar o elemento irmão que virá primeiro na árvore HTML.

2º Informar o símbolo de adição.

3º Informar o elemento que será selecionado. Uma vez que o mesmo esteja ao lado do primeiro elemento informado.

&nbsp; É importante atentar ao fato que apenas o   elemento irmão subsequente ao elemento informado será selecionado.

### Exemplo:

```
    <head>
        <style>
            h1+p{
                color: aqua;
            }
        </style>
        <title>Document</title>
    </head>
    <body>

        <h1>
            Titulo
        </h1>
        <p>
            Irmão Adjacente
        </p>

        <p>
            Irmão Não Adjacente
        </p>

        <h1>
            Outro Titulo
        </h1>
        <p>
            Terceiro Adjacente
        </p>

    </body>
```

&nbsp; No Exemplo acima é possível notar que os elementos p's irmãos e adjacentes de elementos h1's são selecionados. Já o segundo elemento "p" do documento, mesmo sendo irmão de elementos h1's não é selecionado, pois não é adjacente de um elemento "h1".

## General sibling combinator. (Irmãos Adjacentes)

&nbsp; Ao utilizar o seletor Adjacente sibling combinator, tal como descrito acima. Nota-se que como o nome sugere, apenas o irmão adjacente é selecionado. Caso seja necessário selecionar todos elementos irmãos de um determinado elemento, que sigam um padrão, deve-se utilizar o General sibling combinator.

### Sintaxe

&nbsp; A sintaxe será identica ao Adjacente sibling combinator, porém ao invés do símbolo de adição deve-se utilizar o símbolo do til (~).

### Exemplo:

```
    <head>
        <style>
            h1~p{
                color: aqua;
            }
        </style>
        <title>Document</title>
    </head>
    <body>

        <h1>
            Titulo
        </h1>
        <p>
            Irmão Adjacente
        </p>

        <p>
            Irmão Não Adjacente
        </p>

        <p>
            Terceiro Adjacente
        </p>

    </body>
```

&nbsp; No exemplo acima todas as tags p's são selecionadas, porque todas estão no memso nível hierárquico de um elemento h1. Tal como no padrão utilizado para selecionar e aplicar o código CSS.

## Seletor por atributo e valor

&nbsp; Mais uma forma de selecionar um elemento html é pelo valor de um determinado atributo e valor. Ao utilizar este seletor, todo elemento que possua o determinado atributo com mesmo valor indicado será selecionado.

### Sintaxe

1º Deve-se abrir colchetes.

2º Dentro dos colchetes informar o atributo desejado, seguido pelo símbolo de igualidade (=).

3º Após o símbolo de igual deve-se informar o valor que o atributo deve conter para ser selecionado.


### Exemplo

&nbsp; No exemplo abaixo apenas o input cuja o atributo "type" é igual a "text" será selecionado. 

```
    <head>
        <style>
            [type="text"]{
                border-radius: 5px;
                height: 40px;
                width: 300px;
                outline: none;
                border: 2px solid rgb(46, 112, 79);
            }
        </style>
        <title>Document</title>
    </head>
    <body>
        <div>
            <label for="name"> Nome: </label>
            <input type="text" name="name">
        </div>
        <br/>
        <div>
            <label for="age"> Idade: </label>
            <input type="number" name="age">
        </div>

    </body>
```

&nbsp; Este seletor pode ser utilizado com qualquer atributo. Caso necessário o programador pode criar um atributo para realizar sua seleção.

## Seletor por atributo

&nbsp; Ao contrário do seletor por atributo e valor abordado no ultimo tópico.No caso do seletor por atributo, todo elemento que contiver determinado atributo será selecionado, não importanto o valor atribuído ao atributo.

### Sintaxe

&nbsp; A sintaxe é igual a sintaxe do Seletor por atributo e valor, entretanto não se pode informar o sinal de igual seguido pelo valor.

### Exemplo


```
    <head>
        <style>
            [type]{
                border-radius: 5px;
                height: 40px;
                width: 300px;
                outline: none;
                border: 2px solid rgb(46, 112, 79);
            }
        </style>
        <title>Document</title>
    </head>
    <body>
        <div>
            <label for="name"> Nome: </label>
            <input type="text" name="name">
        </div>
        <br/>
        <div>
            <label for="age"> Idade: </label>
            <input type="number" name="age">
        </div>

    </body>
```

&nbsp; No exemplo acima ambos os imputs serão selecionados por possuirem o atributo "type" não importando o valor atribuído ao mesmo.


## Primeiro e ultimo filho

&nbsp; Ainda é possível selecionar o primeiro e ultimo filho de um elemento HTML. Este tipo de seletor é muito utilizado com listas.

### Sintaxe

&nbsp; Deve-se utilizar os atributo css first-child e last-child para selecionar o primeiro e ultimo filho respectivamente.

### Exemplo

```
    <head>
        <style>
            li:first-child{
                color: purple;
            }
        </style>
        <title>Document</title>
    </head>
    <body>
        <ul>
            <li>Esse item não é afetado pelo estilo.</li>
            <li>Esse também não.</li>
            <li>Esse item é! :)</li>
        </ul>
    </body>
```