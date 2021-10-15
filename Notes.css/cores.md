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
