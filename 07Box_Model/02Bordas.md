# Border (Bordas)

&nbsp; O Artigo anterior desta seção apresenta como as margens podem ser utilizadas. Este artigo apresenta propriedades CSS relacionadas as bordas, que por sua vez também podem ser aplicadas em todas as direções de um elemento.

&nbsp; A forma mais básica de uma borda é a borda sólida em todas as direções, para configurá-la deve-se aplicar os seguintes passos:

- Estilo da borda ``border-style``: Neste caso o valor será "solid".

- Espessura da borda ``border-width``: Por exemplo "2px".

- Configurar a cor da borda ``border-color``: Por exemplo "purple".

### Exemplo

&nbsp; Abaixo é demonstrado o exemplo de um elemento cuja borda foi criada seguindo os passos acima.


```html
    <head>
        <style>
            #container{
                width: 40px;
                height: 40px;
                border-style: solid;
                border-width: 2px;
                border-color: purple;
            }
        </style>
        <title>Document</title>
    </head>
    <body>
        <div id="container">

        </div>
    </body>
```

&nbsp; Também é possível juntar todas as configurações da borda na propriedade "border". A propriedade border receberá os três valores na ordem seguinte: 

    1º Estilo
    2º Espessura
    3º Cor


### Exemplo

```html
    <head>
        <style>
            #container{
                width: 40px;
                height: 40px;
                border: solid 2px purple;
            }
        </style>
        <title>Document</title>
    </head>
    <body>
        <div id="container">

        </div>
    </body>
```

## Configurando lados da borda

&nbsp; Tal como as propriedades margin e padding é possível aplicar bordas em lados específicos de um elemento. Para obter tal resultado deve-se utilizar a sintaxe da propriedade border em uma ou mais das seguintes subpropriedades (border-top, border-right, border-bottom, border-left).

### Exemplo:

&nbsp; Neste exemplo será aplicado a borda apenas na parte de baixo e na esquerda do elemento.

```html
    <head>
        <style>
            #container{
                width: 40px;
                height: 40px;
                border-left: solid 2px purple;
                border-bottom: solid 2px purple;
            }
        </style>
        <title>Document</title>
    </head>
    <body>
        <div id="container">

        </div>
    </body>
```

## Opções de Estilo de borda

- ``dotted`` - Define uma borda pontilhada.
- ``dashed`` - Define uma borda tracejada.
- ``solid`` - Define uma borda sólida.
- ``double`` - Define uma borda dupla. 
- ``groove`` - Define uma borda ranhurada 3D. O efeito depende do valor da cor da borda.
- ``ridge`` - Define uma borda sulcada 3D. O efeito depende do valor da cor da borda.
- ``inset`` - Define uma borda de inserção 3D. O efeito depende do valor da cor da borda.
- ``outset`` - Define uma borda de início 3D. O efeito depende do valor da cor da borda.
- ``none`` - Não define nenhuma borda.
- ``hidden`` - Define uma borda oculta.


## Borda Arredondada (border-radius)

&nbsp; Ao utilizar a proprieade border-radius é possível arrendondar a borda de um elemento de acordo com o valor atribuído a propriedade.

&nbsp; Também é possível arredondar a borda de apenas um ou mais lados específicos utilizando as subpropriedades:

- ``border-radius-top``: Arredonda a borda do Topo.
- ``border-radius-right``: Arredonda a borda da direita.
- ``border-radius-bottom``: Arredonda a borda do lado inferiro.
- ``border-radius-left``: Arredonda a borda da esquerda.

### Exemplo 

```html
    <head>
        <style>
            #container{
                width: 40px;
                height: 40px;
                border: solid 2px purple;
                border-radius: 5px;
            }
        </style>
        <title>Document</title>
    </head>
    <body>
        <div id="container">

        </div>
    </body>
```

    * Não é necesário que qualquer outra propriedade de borda seja configurada para aplicar a propriedade border-raidus.


#### Dica

&nbsp; Ao criar um elemento com o mesmo tamanho de largura (width) e altura (height) e configurar a propriedade border-radius recebendo o valor de 50%. O elemento se transformará em um circulo.