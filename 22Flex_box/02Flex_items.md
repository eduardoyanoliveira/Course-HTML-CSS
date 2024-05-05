# Propriedades dos Flex Items

Até agora, vimos apenas as propriedades aplicadas ao ``flex container``, que é o elemento pai. Agora, vamos explorar as propriedades dos flex items, que são os elementos filhos dentro do container.

## ``flex-grow``

A propriedade ``flex-grow`` define a proporção em que um elemento filho irá crescer em relação aos outros flex items. Quando aplicada a um elemento filho, ela distribui os espaços disponíveis para o crescimento entre os flex items.

### Exemplo:

```css
.child {
    flex-grow: 1;
}
```

Ao utilizar ``flex-grow: 1;``, o elemento filho irá ocupar qualquer espaço extra disponível no container.

Se ``flex-grow`` for aplicado a vários flex items, o espaço extra será dividido igualmente entre eles.

## ``flex-shrink``

A propriedade ``flex-shrink`` funciona de maneira oposta ao ``flex-grow``. Ela define como um elemento filho irá encolher em relação aos outros flex items quando o espaço é limitado.

## ``order``

A propriedade ``order`` permite alterar a ordem dos elementos filhos em relação aos outros. Por padrão, todos os elementos têm a ordem 0. Ao aplicar a propriedade order com um valor diferente, é possível modificar a sequência dos flex items.

### Exemplo:

```css
.child {
    order: 1;
}
```

Ao utilizar ``order: 1;``, o elemento filho será posicionado depois dos elementos com order menor ou igual a 0.

## ``align-self``

A propriedade ``align-self`` é semelhante ao ``align-items``, mas é aplicada individualmente a cada elemento filho. Ela permite alinhar um flex item em relação à vertical dentro do container.

### Exemplo:

```css
.child {
    align-self: flex-start;
}
```

Ao utilizar ``align-self: flex-start;``, o elemento filho será alinhado no início vertical do container.

Essas são algumas das propriedades dos flex items. Elas permitem um controle refinado sobre o posicionamento e o comportamento individual de cada elemento filho dentro do flex container. Experimente essas propriedades para criar layouts flexíveis e adaptáveis em seus projetos.