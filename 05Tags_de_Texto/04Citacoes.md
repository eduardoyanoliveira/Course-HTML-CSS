# Citações

Ao construir um artigo, é comum a necessidade de inserir citações de outros artigos, trabalhos ou frases, bem como citar endereços e títulos.

## Citação curta ``<q>``

Para realizar uma citação curta, como uma frase dita por alguém, pode-se utilizar a tag ``<q>``.

Exemplo:

```html
<p>
  <q>
    Ainda que meus maiores críticos vissem me caminhar
    sobre as águas do rio Tâmisa, diriam que o faço por
    não saber nadar.
  </q>
  <cite>Margaret Thatcher</cite>
</p>
```

No exemplo acima, a tag ``<cite>`` é utilizada para citar o nome do autor da citação. A tag ``<cite>`` geralmente é usada para citar nomes de pessoas, trabalhos, empresas, etc. Além disso, o texto dentro da tag ``<cite>`` é renderizado em itálico.

## Blocos de citações ``<blockquote>``

Às vezes, é necessário criar blocos de citações que referenciam um todo, como um trecho de um artigo científico. Para isso, utiliza-se a tag ``<blockquote>``.

Exemplo:

```html
<p>
  Segundo esta citação do site do governo brasileiro, esta é a descrição da síndrome do burnout:
</p>

<blockquote cite="https://www.gov.br/saude/pt-br/assuntos/saude-de-a-a-z/s/sindrome-de-burnout">
  Síndrome de Burnout ou Síndrome do Esgotamento Profissional é um distúrbio emocional com sintomas de exaustão extrema, estresse e esgotamento físico resultante de situações de trabalho desgastante, que demandam muita competitividade ou responsabilidade.
</blockquote>
```

## Abreviações ``<abbr>``

Ao utilizar a tag ``<abbr>``, é possível atribuir semântica a uma abreviação, fornecendo informações úteis para o navegador, mecanismos de busca e sistemas de SEO.

Exemplo:

```html
<p>
  O <abbr title="Cascade Style Sheet">CSS</abbr> é utilizado para estilizar o documento HTML.
</p>
```

Endereços ``<address>``

Para citar endereços dentro de um artigo ou site de forma semanticamente correta, utiliza-se a tag ``<address>``. Dentro da tag, devem ser informados todos os dados do endereço.

Exemplo:

```html
<address>
  Rua: Exemplo rua.<br>
  Site:<br>
  Exemplo.com<br>
  Nº 00, California<br>
  USA
</address>
```

Essas tags de citação, abreviação e endereço podem ser utilizadas para adicionar formatação e semântica adequada ao conteúdo de um documento HTML.