# Adicionando CSS ao documento HTML

&nbsp; Nesta segunda aula, vamos explorar as diferentes formas de adicionar CSS a um documento HTML. Além do <i>inline-css</i>, que já foi mencionado no artigo anterior, existem outras duas maneiras comuns de adicionar estilos CSS.

## Inline-CSS

&nbsp; O inline-css é a forma mais simples de adicionar CSS a um elemento HTML. Para isso, utilizamos o atributo style dentro da tag, que recebe as propriedades desejadas seguidas por dois pontos e o valor correspondente. Cada propriedade é separada por ponto e vírgula para indicar o encerramento.

Apesar de ser simples, essa abordagem não é recomendada devido às suas desvantagens:

### Vantagens:

- O CSS pode ser adicionado diretamente no mesmo documento HTML, evitando a necessidade de baixar um arquivo externo.

### Desvantagens:

- O código CSS não pode ser reutilizado e deve ser adicionado a cada elemento individualmente.
- Como o CSS é inserido diretamente nas tags, o tamanho do documento HTML pode aumentar, tornando o site mais lento.

## CSS Interno

&nbsp; Outra forma de adicionar CSS é utilizando a tag ``<style>`` dentro da tag ``<head>``. Essa abordagem permite aplicar estilos a vários elementos de uma vez e separar o CSS por componentes visuais.

Para usar o CSS interno, siga estas etapas:

1º Crie a tag ``<style>`` dentro da tag ``<head>``. <br>
2º Dentro da tag ``<style>``, selecione o elemento desejado pelo seu nome e, em seguida, abra e feche chaves.<br>
3º Dentro das chaves, escreva o código CSS para estilizar o elemento selecionado. Cada propriedade CSS é escrita com seu nome, seguido por dois pontos e o valor da propriedade. Termine cada propriedade com um ponto e vírgula.<br>

É importante observar algumas informações adicionais:

    Os nomes das propriedades não têm letras maiúsculas, e em caso de nomes compostos, usa-se hífen, como por exemplo, "font-size".
    Como o CSS não está diretamente nas tags que serão estilizadas, é necessário selecionar esses elementos de alguma forma. Isso será abordado em seções posteriores.

Essa abordagem também tem suas desvantagens:

- Adicionar o código CSS diretamente ao documento HTML pode aumentar o tamanho da página e o tempo de carregamento.

## CSS Externo

&nbsp; O CSS externo é considerado a melhor prática para adicionar estilos a um documento HTML, permitindo a criação de um arquivo separado com extensão ".css". Esse arquivo contém o código CSS e pode ser facilmente reutilizado e organizado.

Para utilizar o CSS externo, siga estas etapas:

1º Crie um arquivo CSS separado com a extensão ".css" (por exemplo, "style.css") na mesma pasta do documento HTML.<br>
2º Dentro da tag ``<head>``, adicione a tag ``<link>`` com o atributo rel definido como "stylesheet" e o atributo href definido como o caminho para o arquivo CSS.<br>

Exemplo:

```html
<head>
    <link rel="stylesheet" href="./style.css">
    <title>Document</title>
</head>
```

&nbsp; No exemplo acima, o arquivo CSS externo chamado "style.css" deve estar localizado na mesma pasta do documento HTML. Agora você pode escrever todo o código CSS no arquivo externo, o que permite uma melhor organização e reutilização do código em várias páginas.

### Vantagens do CSS Externo:

- Reutilização de código: O CSS externo pode ser vinculado a várias páginas HTML, permitindo que você aplique o mesmo estilo a todas elas sem duplicar o código.
- Organização: Ao separar o CSS em um arquivo externo, você mantém o HTML mais limpo e legível, focando-se apenas na estrutura e no conteúdo.
- Cache do navegador: O CSS externo é armazenado em cache pelo navegador, o que significa que, uma vez carregado, não precisa ser baixado novamente para páginas subsequentes, resultando em um carregamento mais rápido.

### Desvantagens do CSS Externo:

- Requer uma solicitação adicional: Ao usar um arquivo CSS externo, o navegador precisa fazer uma solicitação separada para buscá-lo, o que pode aumentar ligeiramente o tempo de carregamento da página.
- Dependência do arquivo CSS: Se o arquivo CSS externo não for encontrado ou houver um erro no link, o estilo não será aplicado corretamente.

É recomendado o uso do CSS externo na maioria dos casos, especialmente para projetos maiores ou em desenvolvimento colaborativo, onde a organização e a reutilização do código são fundamentais.