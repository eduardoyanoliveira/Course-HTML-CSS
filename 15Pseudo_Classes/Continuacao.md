# Pseudo-classes em CSS (Continuação) ``:nth-child`` e ``:nth-of-type``

As pseudo-classes ``:nth-child`` e ``:nth-of-type`` permitem selecionar um elemento específico com base em sua posição em relação aos seus irmãos.

A pseudo-classe ``:nth-child`` seleciona o elemento que é o enésimo filho de seu elemento pai. Por exemplo, para selecionar o terceiro ``<p>`` dentro de uma ``<div>``, usamos:

```css
div p:nth-child(3) {
  /* estilos */
}
```

No entanto, é importante observar que essa seleção só funcionará se o terceiro filho da ``<div>`` for um elemento ``<p>``.

A pseudo-classe ``:nth-of-type`` é semelhante ao ``:nth-child``, mas seleciona o elemento com base em seu tipo em vez de sua posição em relação aos irmãos. Por exemplo, para selecionar o terceiro ``<p>`` dentro de uma ``<div>``, independentemente de sua posição em relação a outros elementos, usamos:

```css

div p:nth-of-type(3) {
  /* estilos */
}
```

Dessa forma, o seletor irá selecionar o terceiro elemento ``<p>`` dentro da ``<div>``, independentemente de haver outros elementos entre eles.

## ``:first-child`` e ``:last-child``

As pseudo-classes ``:first-child`` e ``:last-child`` selecionam, respectivamente, o primeiro e o último filho de um elemento pai.

Exemplo:

```css

div p:first-child {
  /* estilos */
}

div p:last-child {
  /* estilos */
}
```

No exemplo acima, o seletor ``div p:first-child`` seleciona o primeiro filho ``<p>`` de cada elemento ``<div>``, enquanto o seletor div p:last-child seleciona o último filho ``<p>`` de cada elemento ``<div>``.

## :not

A pseudo-classe :not permite selecionar todos os elementos, exceto aqueles que correspondem a um seletor específico.

Exemplo:

```css
p:not(.text) {
  /* estilos */
}
```

Nesse caso, o seletor ``p:not(.text)`` seleciona todos os elementos ``<p>`` que não possuem a classe ``.text``. Isso é útil quando queremos aplicar estilos a um conjunto de elementos, exceto alguns com características específicas.

Essas são apenas algumas das pseudo-classes disponíveis no CSS. Existem muitas outras pseudo-classes que você pode explorar e utilizar para estilizar seus elementos de maneira precisa e seletiva.

Lembre-se de consultar a documentação do CSS para obter informações mais detalhadas sobre cada pseudo-classe e suas aplicações.