Tipos numèricos e unidades comuns

# Tipos numéricos

- <integer> Número inteiro como -10 ou 223
- <number> Número decimal -2.4, 64 ou 0.234
- <dimension> È UM <number> com uma unidade junto: 90deg, 2s, 8px
- <percentagem> Representa a fração de outro número: 50%

## Unidades comuns

- <length> Representa um valor de distância: px. em, vw
- <angle> Representa um ângulo: deg, rad, turn
- <time> Representa um tempo: s, ms
- <resolution> Representa resoluções para dispositivos: dpi

=======================================================================

Distâncias absolutas e relativas

# Distâncias absolutas <length>

    São fixa e não alteram seu valor

| Unidade | Nome               | Equivalência        |
| ------- | ------------------ | ------------------- |
| cm      | Centímetros        | 1cm = 96px/2.54     |
| in      | Inches (polegadas) | 1in = 2.54cm = 96px |
| px      | Pixels             | 1px = 1/96th of 1in |

\*o mais comum e mais utilizado é o px

\*não é recomendado usar cm

Distâncias relativas
São relativas a um outro valor, pode ser o elemento pai, ou root, ou o tamanho da tela.
Benefício: Maior adaptação aos diferentes tipos de tela.
| Unidade | Relativo a |
|----------|-----------------------------------------------|
| em | Tamanho da font do elemento pai |
| rem | Tamanho da font do elemento raiz (root/html) |
| vw | 1% da viewport wid |  
| vh | 1% da viewport height |
Normalmente o tamanho da font padrão do navegador é de 16px e para mudar esse valor temos que fazer a alteração no root ou no elemento html.
:root {
font-size: 18px;
}

/_ OU _/

html {
font-size: 18px;
}
O viewport é a parte da tela que está sendo exibida. No caso dos navegadores web, é o que é exibido na janela/tela do documento. Conteúdos que estão fora do viewport só serão exibidos quando feito um scroll da área de visualização.

=======================================================================

Porcentagem

Porcentagens

Descrição
As porcentagens são valores bem flexíveis
Em muitos casos é tratado da mesma maneira que as distâncias <length>
Sempre será relativo a algum valor

💻 Exemplo

Relativo ao elemento pai

html

 <div>
      <p>Morena</p>
      <div>
        <p>Morena</p>   <!-- uma div dentro de outra div-->
        <div>
          <p>Morena</p>
        </div>
      </div>
      <div>

css

html {
font-size: 20px; /_ a font-size do navegador geralmente é de 16px_/
}

div {
font-size: 50%; /_ a porcentagem de cada <div> está sendo aplicada referente ao elemento pai, respeitanbdo a cascata._/
}

=======================================================================

Position

- Posições

<position>

Representa um conjunto de coordenadas 2D:
top, right, bottom, left e center

- Usado para alguns tipos de propriedades como o background-position

- Não confundir com a propriedade position

Exemplo:

.box {
width: 500px;
height: 500px;
background-image: url(http://source.unsplash.com/random);

background-repeat: no-repeat; /_está fazendo com que a imagem não se repita_/

background-position: center; /_está trabalhando com as posições da imagem dentro da caixa..._/

margin-left: 28em; /_está aplicando em volta da imagem_/
margin-top: 5em; /_está aplicando em volta da imagem_/
}

=======================================================================
