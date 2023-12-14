     ## HTML ##

# FORM, INPUTM PLACEHOLDER
* Colocamos o mesmo texto que o do `LABEL`, dessa forma ira aparecer o texto dentro da caixa do `INPUT`, como o leitor de tela nao o ler, deixaremos o label 'invisivel' servindo apenas para o leitor de tela (pensando em acessibilidade)


     ## CSS ##

# Suavização de fontes CSS (principalmente quando se da muito zoom)
-webkit-font-smoothing: antialiased; chrome, edge, safari
-moz-osx-font-smoothing: grayscale; mozila, macos

# APP
* grid-template-rows: max-content 1fr max-content;
- 1,3- maximo tamanho de acordo ao conteudo, 2- o restante da area toda para o 'header'

# MAIN
* overflow-y: scroll;
- fara com que a barra de rolagem aconteca apenas no conteudo do main de forma vertical 'y'

# HEADER FORM
* flex: 1; Faz com que o item preencha todo o espaco disponivel para ele

# .INPUT-WRAPPER LABEL
- Escondendo o label -
     width: 1px;
     height: 1px;
     overflow: hidden;
hidden – Corta o conteúdo que ultrapassa o tamanho da DIV (tamanho definido no width e height)
     position: absolute; 

# .ITEM
* overflow: hidden; Sem ele nao aparecera bordas na parte superior, pois a img esta transbordando

# .ITEM IMG
*   width: 100%; Ocupando toda a largura disponivel 
*   aspect-ratio: 16/9; Definindo a proporcao da imagem
*   object-fit: cover; Para melhorar a qualidade ocupando corretamente o espaco definido

*   transition-property: transform; Para mais de uma propriedade, so usar a ',', caso seja todas, usamos o 'all'
*   transition-duration: 300ms; Tempo que ira durar essa transicao
*   transition-delay: 0; Delay de resposta para iniciar o transform
*   transition-timing-function:; 'substittui' o delay com opcoes ja pre-definidas, cubic bezier, ease, in, in-out, out

*   transition: filter 300ms ease-in, trsnform 500ms ease-out;
/*Posso juntar todos nesse e fazer definicoes de forma separada ou junta*/

# .ITEM IMG:HOVER 
*   filter: hue-rotate(7deg) contrast(101%) saturate(200%);
- Hue dara uma rotacao de cores na img, aumentando o contraste e a satracao
*   transform: scale(1.1) rotate(-2deg);
- Aumentando o tamanho da img com uma leve rotacao,
# Termo DEG ou degrees
- é a medida para ângulos, nada mais é do que graus em inglês.

## Aplicando DELAY individualmente nas imagens
1- Apos criarmos o 'Keyframes', na invocacao, criamos uma variavel para receber o valor do delay
2- Depois no HTML, a partir da segunda img, usamos o 'style: variavel' para que aplique o delay individualmente
