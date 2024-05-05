# Introdução ao CSS

&nbsp; Nesta primeira aula, vamos explorar o CSS (Cascading Style Sheets) e entender como ele é usado para estilizar elementos HTML. O CSS desempenha um papel fundamental ao dar vida e estilo a uma página da web.

&nbsp; O CSS foi desenvolvido pelo W3C (World Wide Web Consortium) em 1996 como uma extensão do HTML. Ele foi criado para superar as limitações do HTML, que se concentrava apenas na marcação do conteúdo, sem oferecer recursos avançados de formatação e estilização.

&nbsp; O CSS é responsável por toda a parte estética de um site ou aplicação web. Embora seja possível criar um site sem utilizar CSS, é praticamente impossível encontrar atualmente algo do tipo na Internet. O CSS se tornou uma ferramenta essencial para criar designs atraentes e profissionais.
Como o CSS funciona?

&nbsp; O CSS possui uma sintaxe simples. Para estilizar um elemento HTML, precisamos informar o nome da propriedade que desejamos alterar e o valor desejado para essa propriedade. Existem várias propriedades que podem ser alteradas em um elemento, e cada propriedade possui diversos valores possíveis.

&nbsp; Uma maneira de aplicar estilos CSS a um elemento HTML é utilizando o atributo style dentro da tag. Esse atributo recebe as propriedades desejadas, seguidas por dois pontos e o valor correspondente. Cada propriedade é separada por ponto e vírgula para indicar o seu encerramento.
Exemplo:

``` html
<div>
    <p style="color: red; font-size: 20px;">
        Este é apenas um parágrafo de exemplo!
    </p>
</div>
```

&nbsp; No exemplo acima, utilizamos o atributo style para definir o estilo do parágrafo. Definimos a cor do texto como vermelha (color: red) e o tamanho da fonte como 20 pixels (font-size: 20px).

## Dica

    É importante destacar que o uso do atributo style diretamente na tag é útil para estilizar elementos individuais. No entanto, quando precisamos aplicar estilos em várias partes do documento ou criar um design consistente, é recomendado utilizar folhas de estilo externas, também conhecidas como arquivos CSS separados. Isso permite uma melhor organização e reutilização dos estilos em todo o site.

&nbsp; O CSS oferece uma ampla gama de recursos e possibilidades para estilizar elementos HTML, desde cores e fontes até posicionamento e animações. Nos próximos módulos, exploraremos esses recursos com mais detalhes.