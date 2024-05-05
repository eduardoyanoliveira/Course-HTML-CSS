# Animações

As animações em HTML e CSS funcionam de forma semelhante às transições que já vimos anteriormente. No entanto, as animações são aplicadas a partir de um evento específico, como um hover do mouse, um clique ou uma seleção. Além disso, as animações permitem mudanças mais complexas nos elementos, como alterações de tamanho, cor, borda, entre outros.

## Keyframes e Animation

As animações em CSS são definidas usando os conceitos de keyframes e animation. Keyframes são usados para criar a animação propriamente dita, enquanto a propriedade animation é usada para aplicar a animação a um elemento.

## Dicas

Aqui estão algumas dicas úteis ao lidar com animações:

- Somente valores numéricos podem ser animados, como ``10px``, ``.5``, ``58%``, ``10em``, ``#cf0`` e ``red``. Valores como ``auto``, ``Arial``, ``hidden`` e outros não numéricos não podem ser animados.
- As propriedades mais performáticas para animação são ``transform`` e ``opacity``.
- Se necessário, você pode usar a propriedade ``will-change`` para melhorar o desempenho da animação. No entanto, só utilize ``will-change`` se realmente for necessário.

## Sintaxe do Keyframes

A sintaxe para criar uma animação usando keyframes é a seguinte:

```css
@keyframes nome_da_animacao {
    from {
        /* estado inicial */
    }
    to {
        /* estado final */
    }
}
```

Você também pode definir os ``keyframes`` usando porcentagens para determinar em qual momento da animação uma mudança específica será aplicada:

```css
@keyframes minha_animacao {
    0% {
        /* estado inicial */
    }
    33% {
        /* mudança no meio da animação */
    }
    100% {
        /* estado final */
    }
}
```

Aplicando a Animação em um Elemento

Para aplicar a animação a um elemento, você pode usar a propriedade animation no seletor do elemento:

```css

.elemento {
    animation: minha_animacao 3s;
}
```

Propriedades da Animação

A propriedade animation possui várias subpropriedades que podem ser utilizadas para ajustar o comportamento da animação:

- ``animation-direction``: define a direção da animação, como alternate-reverse para iniciar a animação do final.
- ``animation-iteration-count``: determina o número de iterações da animação, podendo ser um valor numérico ou infinite para repetir indefinidamente.
- ``animation-fill-mode``: especifica como as propriedades CSS são aplicadas antes ou depois da animação, como backwards para aplicar as propriedades antes do início da animação.

Com essas técnicas, você pode criar animações interessantes e interativas em seu projeto, tornando-o mais dinâmico e atraente para os usuários.