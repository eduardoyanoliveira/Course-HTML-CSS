# Aula sobre HTML e CSS: Incorporando Mídia

Nesta aula, aprenderemos como incorporar mídia, como vídeos e áudios, em páginas HTML utilizando as tags ``<iframe>``, ``<audio>``, e ``<video>``. Também abordaremos algumas técnicas para melhorar a compatibilidade entre diferentes navegadores.

## Tag ``<iframe>``

A tag ``<iframe>`` permite inserir um pedaço de outra página da web ou um arquivo HTML local em uma página. Para isso, utilizamos o atributo src, que especifica o endereço da página que desejamos incorporar.

### Exemplo básico de uso da tag ``<iframe>``:

```html
<iframe src="www.meusite.com"></iframe>
```

É possível também definir a largura e altura do iframe utilizando os atributos width e height, respectivamente.

### Exemplo com tamanho personalizado do iframe:

```html

<iframe src="www.meusite.com" width="100%" height="500px"></iframe>
```

Outra utilização comum da tag ``<iframe>`` é a incorporação de vídeos do YouTube. Nesse caso, basta utilizar a tag ``<iframe>`` e fornecer o código de incorporação fornecido pelo YouTube.

## Tag ``<audio>``

A tag ``<audio>`` é utilizada para incorporar arquivos de áudio em páginas HTML. Utilizamos o atributo src para especificar o local onde o arquivo de áudio está armazenado, e o atributo controls para exibir um player de áudio na tela.

### Exemplo básico de uso da tag ``<audio>``:

```html
<audio src="minha_pasta/meu_arquivo.mp3" controls></audio>
```

No entanto, ao utilizar apenas o atributo src, podemos enfrentar problemas de compatibilidade entre navegadores, já que diferentes navegadores suportam diferentes tipos de arquivo de áudio (ex: mp3, ogg, etc.).

Para contornar esse problema, podemos adicionar múltiplas fontes de áudio na tag ``<audio>``, utilizando a tag ``<source>``. Cada ``<source>`` especifica um arquivo de áudio com seu próprio atributo src.

### Exemplo de uso da tag ``<audio>`` com múltiplas fontes de áudio:

```html
<audio controls>
    <source src="media/meu_arquivo.mp3" type="audio/mp3">
    <source src="media/meu_arquivo.ogg" type="audio/ogg">
</audio>
```

Além disso, é recomendado informar o tipo de arquivo de áudio utilizando o atributo type na tag ``<source>``, para que o navegador possa escolher a fonte correta.

Também é possível adicionar um elemento dentro da tag ``<audio>``, que será exibido caso o navegador não ofereça suporte à tag ``<audio>``, semelhante ao atributo alt da tag ``<img>``.

### Exemplo com elemento alternativo para navegadores sem suporte à tag ``<audio>``:

```html
<audio controls>
    <source src="media/meu_arquivo.mp3" type="audio/mp3">
    <source src="media/meu_arquivo.ogg" type="audio/ogg">
    <p>Seu navegador não suporta este recurso.</p>
</audio>
```

Também existem atributos adicionais que podem ser utilizados com a tag ``<audio>``:

- ``autoplay``: reproduz o áudio automaticamente quando a página é carregada.
- ``loop``: permite que o áudio seja reproduzido em loop, repetindo continuamente.

## Tag ``<video>``

A tag ``<video>`` é utilizada para incorporar vídeos em páginas HTML. Assim como a tag ``<audio>``, podemos utilizar o atributo src para especificar o local onde o arquivo de vídeo está armazenado, e o atributo controls para exibir controles de vídeo na tela.

### Exemplo básico de uso da tag ``<video>``:

```html
<video src="meu_video.mp4" controls></video>
```

Assim como a tag ``<audio>``, podemos adicionar múltiplas fontes de vídeo utilizando a tag ``<source>``, especificando diferentes formatos de arquivo de vídeo.

### Exemplo de uso da tag ``<video>`` com múltiplas fontes de vídeo:

```html
<video controls>
    <source src="meu_video.mp4" type="video/mp4">
    <source src="meu_video.webm" type="video/webm">
</video>
```

Também podemos utilizar o atributo muted para deixar o vídeo mudo, ou seja, sem som.

### Exemplo de uso da tag ``<video>`` com o atributo muted:

```html
<video src="meu_video.mp4" controls muted></video>
```

Além disso, assim como no caso da tag ``<audio>``, podemos adicionar um elemento alternativo dentro da tag ``<video>``, que será exibido caso o navegador não ofereça suporte à tag ``<video>``.

### Exemplo com elemento alternativo para navegadores sem suporte à tag ``<video>``:

```html
<video controls>
    <source src="meu_video.mp4" type="video/mp4">
    <source src="meu_video.webm" type="video/webm">
    <p>Seu navegador não suporta este recurso.</p>
</video>
```

Existem também outros atributos que podem ser utilizados com a tag ``<video>``, como autoplay para reproduzir o vídeo automaticamente quando a página é carregada e loop para reproduzir o vídeo em loop.

### Exemplo de uso da tag ``video>`` com os atributos autoplay e loop:

```html
<video src="meu_video.mp4" controls autoplay loop></video>
```

Lembre-se de que é importante fornecer diferentes formatos de arquivo de vídeo para garantir uma melhor compatibilidade entre navegadores.