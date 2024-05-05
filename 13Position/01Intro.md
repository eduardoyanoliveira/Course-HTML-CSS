# Position e Posicionamento de Elementos

A propriedade position do CSS permite controlar o posicionamento de elementos em uma página. Ela aceita quatro valores principais: static, relative, absolute e fixed.
Position Static

O valor padrão da propriedade position é static. Com position: static, os elementos são posicionados em relação ao fluxo normal do documento. Isso significa que eles serão colocados no local em que estão no HTML ou conforme definido pelo uso de outras propriedades CSS, como display, margin e padding.

## Position Relative

Com position: relative, o elemento será posicionado em relação a si mesmo. No entanto, para que essa propriedade funcione corretamente, são necessárias outras propriedades, como left, right, top e bottom. Essas propriedades permitem mover o elemento em relação à sua posição original.

Por exemplo, se você aplicar o seguinte CSS a uma ``<div>``, ela se moverá 15px para a esquerda e 15px para cima em relação à sua posição original:

```css

div {
  position: relative;
  left: 15px;
  top: 15px;
}
```

## Position Absolute

Com position: absolute, o elemento será posicionado em relação ao primeiro elemento pai que tenha uma propriedade position diferente de static. Isso permite um posicionamento mais preciso e específico na página.

Por exemplo, se uma ``<div>`` receber o seguinte CSS e essa ``<div>`` estiver dentro de uma ``<section>`` com position: relative, a ``<div>`` será posicionada no canto superior direito do elemento ``<section>``:

```css
div {
  position: absolute;
  top: 0;
  right: 0;
}
```

## Position Fixed

Com ``position: fixed``, o elemento será posicionado em relação à janela do navegador. Ele permanecerá fixo em sua posição, mesmo quando a página é rolada. Isso é útil para criar elementos que devem ser exibidos constantemente na tela, como barras de navegação ou rodapés.

O uso de ``position: fixed`` também altera o fluxo normal do documento, assim como position: absolute.
Escolhendo o Posicionamento Adequado

Ao usar a propriedade position, é importante escolher o valor adequado para o posicionamento desejado. Considere a estrutura do seu documento HTML, as relações de posicionamento entre elementos e os efeitos desejados.

Experimente diferentes valores de position e utilize as propriedades auxiliares, como ``left``, ``right``, ``top`` e ``bottom``, para posicionar seus elementos de forma precisa e criar layouts personalizados.

Lembre-se de que ``position: relative``, ``position: absolute`` e ``position: fixed`` podem alterar o fluxo normal do documento DOM. Portanto, certifique-se de testar e ajustar adequadamente seu código para obter o resultado desejado.