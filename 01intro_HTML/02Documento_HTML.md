# Estrutura do Documento HTML

&nbsp; Nesta segunda aula, vamos abordar a estrutura básica de um documento HTML. É importante ressaltar que esta aula complementa o conteúdo da aula anterior, então, caso haja alguma referência a conceitos já apresentados, é recomendado revisitar a aula anterior para mais detalhes.

## Passos para criar um documento HTML:

Para criar um documento HTML que seja interpretado corretamente pelo navegador, siga os seguintes passos:

    A primeira linha do documento HTML deve conter a tag <!doctype html>. Essa tag indica ao navegador que o documento é um arquivo HTML. Por exemplo:

```html
<!doctype html>
```

É importante observar que a falta dessa tag não irá gerar um erro, mas é uma boa prática incluí-la para garantir a correta interpretação do documento pelo navegador.

    Em seguida, crie uma tag <html> com um atributo lang que especifica o idioma do documento. Por exemplo:

```html
<html lang="en">
</html>
```

O atributo lang permite indicar a linguagem utilizada no documento (por exemplo, "pt-BR" para português brasileiro).

A primeira tag filha da tag ``<html>`` é a tag ``<head>``, que contém as informações sobre os metadados do documento. Por exemplo:

```html
<head>
</head>
```

* Os metadados são passados como tags filhas da tag ``<head>``. A única tag que todo documento HTML deve possuir dentro da tag ``<head>`` é a tag ``<title>``. Essa tag define o título do documento, que será exibido na aba do navegador. Por exemplo:

```html
<title>Meu Documento</title>
```

* Além da tag ``<title>``, existem outras tags de metadados importantes, como a tag ``<meta>`` com o atributo charset, que especifica a codificação de caracteres utilizada no documento. Sem essa tag, caracteres especiais, como acentos, podem não ser exibidos corretamente. Por exemplo:

```html
<meta charset="UTF-8">
```

* Por fim, a última tag que todo documento HTML deve conter é a tag ``<body>``. Essa tag recebe todo o conteúdo da página que será renderizado pelo navegador. Por exemplo:

```html
<body>
</body>
```

## Resultado

Após seguir todos os passos acima, o resultado será um documento HTML vazio, pronto para ser utilizado. Veja o exemplo completo:

```html
<!doctype html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>Meu Documento</title>
    </head>
    <body>
    </body>
</html>
```

### Dica

Ao analisar o exemplo acima, é possível notar que todas as tags filhas são indentadas com um nível a mais em relação à sua tag mãe. Essa técnica de indentação, também conhecida como formatação ou identação do código, não é obrigatória no HTML, mas é uma boa prática para facilitar a leitura e compreensão do código.

Ao utilizar a indentação, é possível identificar facilmente as tags filhas e as tags mães. Também é possível observar que as tags que possuem a mesma quantidade de tabulações são consideradas tags irmãs, pois têm a mesma tag mãe.

Continue praticando e explorando!!!