# Formulários

Os formulários são usados em HTML quando é necessário receber informações do usuário para serem enviadas ao servidor.

A tag ``<form>`` é usada para envolver todo o formulário. Por padrão, ela ocupará toda a largura da tela.

Importante: Não é possível aninhar uma tag ``<form>`` dentro de outra tag ``<form>``.

## Atributos da tag ``<form>``

- ``action``: Define o destino para onde o formulário será enviado quando for submetido.
- ``method``: Define o método de envio do formulário. Os métodos mais comuns são GET e POST.
- ``autocomplete``: Define se o preenchimento automático dos campos do formulário está habilitado ou desabilitado.

## Tags comumente usadas dentro da tag ``<form>``

- `` <h1> a <h6> ``: Usadas para o título do formulário.
- ``<fieldset>``: Usada para agrupar campos relacionados.
    - ``<legend>``: Usada dentro da tag ``<fieldset>`` para fornecer uma legenda para os campos agrupados.
    - ``<p>``: Usada para separar os campos dentro do ``<fieldset>``.
- ``<input>``: Usada para criar campos de entrada onde o usuário pode inserir valores.

Exemplo:

```html
<form action="#" method="get" autocomplete="off">
  <h1>Formulário Teste</h1>
  <fieldset>
    <legend>Nome</legend>
    <p>
      <input type="text" name="name">
    </p>
  </fieldset>
</form>
```

## Atributos da tag ``<input>``

- ``name``: Define o nome do campo de entrada, usado no backend para processar os dados enviados.
- ``id``: Define o identificador único do campo de entrada, usado no frontend para associar rótulos ou estilos.
- ``type``: Define o tipo de campo de entrada, como text, number, date, etc.
- ``placeholder``: Define um texto de exemplo ou dica dentro do campo de entrada.
- ``value``: Define o valor inicial do campo de entrada.