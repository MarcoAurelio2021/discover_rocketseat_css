# Introdução

Descrição
Cores
Usamos CSS para alterar cores do nosso documento.

Tipos
background-color (para caixas)
color (para textos)
border-color (para caixas)
outros...

Valores

Podemos definir valores por:
palavra-chave (blue, transparent)
hexadecimal (#990011)
funções: rgb, rgba, hsl, hsla

==========================================================================

# Hexadecimal

Descrição
Nessa aula vamos aprender a trabalhar com valores hexadecimal

/_<hex-color> values 0-9 e A-F_/
color: #090; /_ RED, GREEN, BLUE _/
color: #009900;
color: #090a;
color:#009900aa;

==========================================================================

# RGB

Descrição

RGB → Red, Green e Blue
O alpha representa a transparência da cor
/_<rgb()> values _/

color: rgb(34, 12, 64, 0.6) /_ 0-255 _/
color: rgba(34, 12, 64, 0.6)

==========================================================================

# HSL → Hue - Saturation - Lightness

color: hsl(180, 100%, 50%, 60%)
color: hsla(180, 100%, 50%, 60%)
==========================================================================

# Global values

Descrição
Nessa aula vamos ver sobre os valores globais da propriedade color.

/_ Global values _/
color: inheritr; /_ Herda a cor do elemento anterior _/
color: initial; /_ Volta a sua cor inicial _/
color: unset; /_ Pega a cor do contexto _/

==========================================================================

# Background

Para mudar o tamanho da imagem do background usamos a propriedade background-size.

/_ Values _/
background-size: cover;
background-size: contain;

/_ Podemos usar 2 valores, o primeiro é para a largura da imagem e o segundo é para a altura _/
background-size: 40% auto;
background-size: 2em 25%;
background-size: auto 8px;
background-size: auto auto;

==========================================================================

# Background-origin

Descrição
A propriedade background-origin é quem define o ponto de origem de uma imagem específica.
/_ Principais valores _/
background-origin: border-box;
background-origin: padding-box;
background-origin: content-box;

### O background-clip

define se a cor ou imagem do background iniciam debaixo de sua área de borda, preenchimento ou conteúdo.
/_ Principais valores _/

background-clip: border-box;
background-clip: padding-box;
background-clip: content-box;
background-clip: text;

==========================================================================

# Background-attachment

Descrição
A propriedade background-attachment determina se a posição da imagem vai ser fixa ou se vai rolar junto com o conteúdo.

/_ Principais valores _/
background-attachment: scroll;
background-attachment: fixed;
background-attachment: local;
==========================================================================

# Gradient

Descrição

linear-gradient() é a função usada para criar gradient linear com o CSS.
background: linear-gradient(45deg, red, yellow)

radial-gradient() é a função usada para criar gradient circular.
background: radial-gradient(green, red, yellow)
background: radial-gradient(rgba(255, 255, 255, 0), rgba(255, 0, 0, 0.2))
==========================================================================

# Múltiplos valores

Descrição
Podemos aplicar múltiplos backgrounds em um mesmo elemento, podendo ter cor sólida, gradiente ou imagem. Para isso basta separar por vírgula cada background.
