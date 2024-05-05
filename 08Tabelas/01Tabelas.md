# Tabelas em HTML e CSS

As tabelas são elementos essenciais em HTML para exibir dados tabulares de forma organizada. Elas consistem em linhas e colunas que formam células, onde os dados são inseridos.
Estrutura básica de uma tabela em HTML

Para criar uma tabela em HTML, é necessário utilizar as seguintes tags:

```html
<table>
  <tr>
    <th>Coluna 1</th>
    <th>Coluna 2</th>
    <th>Coluna 3</th>
  </tr>
  <tr>
    <td>Dado 1</td>
    <td>Dado 2</td>
    <td>Dado 3</td>
  </tr>
  <tr>
    <td>Dado 4</td>
    <td>Dado 5</td>
    <td>Dado 6</td>
  </tr>
</table>
```

- A tag ``<table>`` é usada para criar a tabela.
- A tag ``<tr>`` define uma linha na tabela.
- A tag ``<th>`` é usada para criar cabeçalhos de coluna.
- A tag ``<td>`` define células de dados.

Estilizando tabelas com CSS

As tabelas podem ser estilizadas usando CSS para melhorar sua aparência e legibilidade. Aqui estão algumas propriedades CSS comumente usadas para estilizar tabelas:
## Propriedades de estilo da tabela:

- ``border-collapse``: Define se as bordas das células devem ser colapsadas em uma única borda ou não. Os valores possíveis são collapse e separate.
- ``border-spacing``: Define o espaçamento entre as células da tabela quando border-collapse é definido como separate.
- ``width``: Define a largura da tabela.
- ``background-color``: Define a cor de fundo da tabela.

## Propriedades de estilo das células:

- ``text-align``: Define o alinhamento do texto dentro das células. Os valores possíveis são left, right, center e justify.
- ``vertical-align``: Define o alinhamento vertical do conteúdo dentro das células. Os valores possíveis são top, middle, bottom e baseline.
- ``padding``: Define o espaçamento interno das células.
- ``border``: Define as bordas das células.

Aqui está um exemplo de como estilizar uma tabela com CSS:

```html
<style>
  table {
    border-collapse: collapse;
    width: 100%;
    background-color: #f2f2f2;
  }

  th, td {
    padding: 8px;
    text-align: left;
    border: 1px solid #ccc;
  }

  th {
    background-color: #4CAF50;
    color: white;
  }
</style>

<table>
  <tr>
    <th>Nome</th>
    <th>Idade</th>
    <th>País</th>
  </tr>
  <tr>
    <td>João</td>
    <td>25</td>
    <td>Brasil</td>
  </tr>
  <tr>
    <td>Maria</td>
    <td>30</td>
    <td>Portugal</td>
  </tr>
</table>
```

&nbsp; Neste exemplo, a tabela possui um estilo de borda colapsada com ``border-collapse: collapse`` e uma largura de 100%. A cor de fundo da tabela é definida como ``#f2f2f2``. As células têm um espaçamento interno de 8 pixels, texto alinhado à esquerda e uma borda sólida de 1 pixel com cor ``#ccc``. Os cabeçalhos das colunas têm um fundo verde escuro ``#4CAF50`` e texto branco para destaque.