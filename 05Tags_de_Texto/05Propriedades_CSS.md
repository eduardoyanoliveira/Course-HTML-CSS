# Propriedades CSS para Texto

- ``Color``: Altera a cor do texto.

- ``Direction``: Configura a direção do texto.

- ``letter-spacing``:  	Aumenta ou diminui o espaço entre os caracteres. 

- ``text-aling``: Alinha o texto dentro do elemento pai.

### Exemplo

```html
<head>
    <style>
        h1{
            color: green;
            text-align: center;
        }
        p{
            direction: rtl;
            letter-spacing: 5px;
        }
    </style>
</head>
<body>
    <h1>Titulo</h1>
    <p>
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Amet magnam fuga, velit aspernatur unde alias hic recusandae quidem laboriosam illum soluta adipisci reprehenderit! Qui, officiis dolor dolore eius vel officia?
    </p>
</body>
```

- ``text-indent``: Recua a primeira linha de um texto num elemento.

- ``text-shadow``: Aplica sombra a fonte.

- ``text-transform``: Configura o caracteres em maiúsculo, minúsculo ou capitalizado.

- ``word-spacing``: Configura o espaço entre as palavras.


### Exemplo

```html
<head>
    <title>Document</title>
    <style>
        h1{
            text-shadow: 5px 2px 5px rgb(41, 80, 138);
            text-align: center;
            color: rgb(60, 60, 61);
        }
        #firstP{
            text-transform: uppercase;
        }
        #secondP{
            text-transform: capitalize;
            word-spacing: 10px;
        }
    </style>
</head>
<body>
    <h1>Titulo</h1>
    <p id="firstP">
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Amet magnam fuga, velit aspernatur unde alias hic recusandae quidem laboriosam illum soluta adipisci reprehenderit! Qui, officiis dolor dolore eius vel officia?
    </p>
    <p id="secondP">
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Amet magnam fuga, velit aspernatur unde alias hic recusandae quidem laboriosam illum soluta adipisci reprehenderit! Qui, officiis dolor dolore eius vel officia?
    </p>
</body>

```

- ``text-decoration``: Adiciona uma decoração ao texto, como sublinhado.

- ``font-style``: Configura o estilo da fonte, como por exemplo em itálico.

- ``font-size``: Configura o tamanho da fonte.

- ``font-weight``: Configura a espessura da fonte. Podendo colocar a fonte em negrito.

- ``line-height``: Configura o tamanho da linha do texto.

### Exemplo

```html
<head>
    <style>
        h1{
            text-decoration: dashed;
        }
        #firstP{
            font-style: italic;
            font-size: 20px;
            font-weight: bold;
            line-height: 35px;
        }
    </style>
</head>
<body>
    <h1>Titulo</h1>
    <p id="firstP">
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Amet magnam fuga, velit aspernatur unde alias hic recusandae quidem laboriosam illum soluta adipisci reprehenderit! Qui, officiis dolor dolore eius vel officia?
    </p>
</body>
```

&nbsp; Por final pode-se configurar a fámilia da fonte utilizando a propriedade:

- ``font-family``.

&nbsp; Existem ainda maiores possibilidades de estilização para textos. Este artigo compromete-se a apresentar as propriedades CSS mais utilizadas no que se refere a estilização de caracteres em geral.