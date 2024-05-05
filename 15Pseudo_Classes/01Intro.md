# Pseudo-classes em CSS

As pseudo-classes em CSS permitem selecionar elementos com base em seu estado ou posição no documento. Elas são representadas por dois pontos (:) seguidos do nome da pseudo-classe.

## ``::before`` e ``::after``

As pseudo-classes ``::before`` e ``::after`` são usadas para inserir conteúdo antes e depois de um elemento, respectivamente. Para usá-las, precisamos definir a propriedade content em conjunto.

Exemplo:

```css
div::before {
  content: "Antes";
}

div::after {
  content: "Depois";
}
```

Nesse caso, o texto "Antes" será inserido antes do conteúdo do elemento ``<div>`` e o texto "Depois" será inserido após o conteúdo.
`
## Outras Pseudo-classes

Além das pseudo-classes ::before e ::after, existem muitas outras pseudo-classes que permitem selecionar elementos com base em diferentes critérios, como estado, posição ou conteúdo.

Aqui estão alguns exemplos:

- ``:checked``: Seleciona um elemento quando está marcado ou selecionado, geralmente usado com elementos ``<input>`` do tipo checkbox ou radio.
- ``:disabled``: Seleciona um elemento quando está desativado, como um botão com o atributo disabled.
- ``:empty``: Seleciona um elemento que não contém nenhum conteúdo.
- ``:enabled``: Seleciona um elemento que está habilitado ou ativo.
- ``:first-child``: Seleciona o primeiro filho de um elemento pai.
- ``:focus``: Seleciona um elemento quando está em foco, geralmente usado com elementos interativos como ``<input>`` ou ``<textarea>``.

Essas são apenas algumas das pseudo-classes disponíveis. Existem muitas outras que você pode explorar e utilizar para estilizar seus elementos de acordo com diferentes estados e características.

Experimente combinar as pseudo-classes com outras propriedades CSS para criar estilos dinâmicos e interativos em seu site. Lembre-se de consultar a documentação do CSS para obter informações detalhadas sobre cada pseudo-classe e suas aplicações.