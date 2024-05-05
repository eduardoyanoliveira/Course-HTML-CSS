# Campos

## Campo de entrada de texto (input)

O campo de entrada de texto é usado para que o usuário insira informações em formato de texto. É possível configurar diversos atributos nesse campo para personalizar seu comportamento.

- ``disabled``: Quando definido como disabled, o campo de entrada de texto fica desativado, o que significa que o usuário não poderá interagir com ele.
- ``readonly``: Quando definido como readonly, o campo de entrada de texto fica apenas para leitura, o que significa que o usuário poderá ver o valor, mas não poderá alterá-lo.
- ``required``: Quando definido como required, o campo de entrada de texto se torna obrigatório, o que significa que o usuário deve preenchê-lo antes de enviar o formulário.
- ``type="text"``: Esse atributo define o tipo de campo como texto.

## Botão (button)

Os botões são usados para executar ações dentro do formulário. Podemos configurar diferentes tipos de botões para diferentes finalidades.

- ``type="submit"``: Esse tipo de botão é usado para enviar ou gravar as informações do formulário. Ao clicar nele, os dados serão enviados ao servidor para processamento.
- ``type="reset"``: Esse tipo de botão é usado para redefinir o formulário para seus valores padrão. Ao clicar nele, todos os campos serão limpos e voltarão aos valores iniciais.

## Rótulo (label)

Os rótulos são usados para fornecer uma descrição ou rótulo aos campos de entrada. Existem duas formas de associar um rótulo a um campo de entrada.

    Usando o atributo for no rótulo e definindo-o com o mesmo valor do atributo name do campo de entrada. Ao clicar no rótulo, o campo de entrada correspondente será selecionado.

```html
<label for="name">Nome</label>
<input type="text" name="name">
```

Envolver o campo de entrada com a tag ``<label>``. Nesse caso, não é necessário usar o atributo for, pois o campo de entrada está implicitamente associado ao rótulo.

```html
<label>
  Nome
  <input type="text" name="name">
</label>
```

## Tipos de campo de entrada (input)

Existem diferentes tipos de campos de entrada que podem ser usados em formulários, cada um com seu propósito específico.

- ``type="text"``: Esse tipo de campo permite ao usuário inserir texto. É o tipo de campo padrão quando nenhum tipo é especificado.
- ``type="password"``: Esse tipo de campo é usado para inserir senhas, ocultando o texto digitado.
- ``type="email"``: Esse tipo de campo é usado para inserir endereços de e-mail e valida se o formato inserido é um endereço de e-mail válido.
- ``type="number"``: Esse tipo de campo é usado para inserir valores numéricos. Você pode especificar um valor mínimo usando o atributo min e um valor máximo usando o atributo max.
- ``type="date"``: Esse tipo de campo é usado para inserir datas. Ele pode exibir um seletor de data nativo no navegador.
- ``type="checkbox"``: Esse tipo de campo exibe uma caixa de seleção que representa um valor booleano (verdadeiro ou falso). É possível usar o atributo checked para definir se o campo já deve vir selecionado.
- ``type="radio"``: Esse tipo de campo exibe uma lista de opções em que apenas uma pode ser selecionada. Para que apenas uma opção seja selecionada, todos os campos de opção devem ter o mesmo atributo name. É possível usar o atributo checked para definir qual opção deve vir selecionada.
- ``type="file"``: Esse tipo de campo permite ao usuário selecionar um ou vários arquivos para serem enviados ao servidor. Quando usado com o atributo multiple, é possível selecionar vários arquivos de uma vez.
- ``type="color"``: Esse tipo de campo exibe um seletor de cores que permite ao usuário escolher uma cor.
- ``type="range"``: Esse tipo de campo exibe uma barra de rolagem horizontal que permite ao usuário selecionar um valor dentro de um intervalo especificado usando os atributos min, max e step.
- ``type="submit"``: Esse tipo de campo é usado para enviar o formulário ao servidor quando o usuário clica nele. Geralmente é usado em botões de envio.
- ``type="reset"``: Esse tipo de campo é usado para redefinir todos os campos do formulário para seus valores iniciais quando o usuário clica nele.

Esses são apenas alguns dos tipos mais comuns de campos de entrada. Cada tipo de campo possui seus próprios atributos e comportamentos específicos, permitindo que você personalize ainda mais seus formulários de acordo com as necessidades do seu projeto.