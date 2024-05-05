# Textos

## Parágrafos

Para criar um parágrafo em um documento HTML, o desenvolvedor deve utilizar a tag ``<p>``. Um parágrafo sempre será exibido em uma nova linha e o navegador adicionará por padrão uma quantidade predefinida de margem ao seu final.

Exemplo:

```html
<p>Primeiro parágrafo</p>
<p>Segundo parágrafo</p>
```

## Linha Horizontal (hr)

A tag ``<hr>`` é utilizada para adicionar uma linha horizontal entre dois conteúdos de texto. Ela é útil para separar seções ou adicionar uma divisão visual no texto.

Exemplo:

```html
<h2>Primeiro conteúdo</h2>
<p>Primeiro parágrafo</p>
<p>Segundo parágrafo</p>
<hr>
<h2>Segundo conteúdo</h2>
<p>Primeiro parágrafo</p>
<p>Segundo parágrafo</p>
```

## Quebra de Linha

Outra necessidade comum ao criar texto em um documento HTML é realizar uma quebra de linha entre frases. Para isso, pode-se utilizar a tag ``<br>``.

Exemplo:

```html
<p>
  Este é apenas um parágrafo de teste.<br>
  Aqui está outra frase de teste.
</p>
```

## Código

Para exibir um trecho de código de programação em um artigo ou site, deve-se utilizar a tag ``<code>``.

Exemplo:

```html
<p>
  Para criar uma variável em JavaScript, pode-se utilizar as palavras reservadas "var" ou "let", como é apresentado no código abaixo.
</p>
```

```html
<code>
  var name = "Yan";
  let role = "Developer";
</code>
```

## Texto Pré-formatado

A tag ``<pre>`` é útil quando se deseja preservar a formatação exata do texto dentro do documento HTML. Qualquer espaçamento em branco, tabulação ou quebras de linha presentes dentro da tag ``<pre>`` serão renderizados no navegador.

Exemplo:

```html
<pre>
  Este texto possui uma pré-formatação.
  Logo, todos os espaços em branco dentro da tag serão renderizados pelo navegador.
</pre>
```

Dessa forma, você pode utilizar essas tags para formatar corretamente o conteúdo de texto em seu documento HTML.