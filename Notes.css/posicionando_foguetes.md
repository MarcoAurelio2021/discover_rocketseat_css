# Position

Descrição

Posicionamentos
Controla onde, na página, o elemento irá ficar, alterando o fluxo normal dos elementos.

Name: position
Value: static | relative | absolute | fixed
Lembrando que o fluxo normal dos elementos é ficar um abaixo do outro, a não ser no caso de elementos inline, que ficam um ao lado do outro.
=======================================================================

# Relative

Descrição
O position indica onde o elemento vai ser posicionado na página. Ao usar o position podemos adicionar outras propriedades como top, right, bottom, left e z-index, que vão determinar o posicionamento final do elemento.

Quando o position é relative os elementos são deslocados do seu posicionamento normal, mas sem afetar o posicionamento de outros elementos da página.

HTML

<div class="box box1"></div>
<div class="box box2"></div>
<div class="box box3"></div>
CSS

.box {
width: 50px;
height: 50px;
margin-bottom: 8px;
}

.box1 {
background-color: red;
position: relative;
left: 100px;
top: 80px
}

.box2 {
background-color: green;
}

.box3 {
background-color: blue;
}

=======================================================================

# Absolute

Descrição

Quando o position é absolute o elemento é deslocado saindo do fluxo normal. O elemento de position absolute é posicionado em relação ao seu parent element mais próximo. Se esse elemento "pai" não existir, ele será posicionando em relação ao bloco contendo a raiz do elemento.

- Ele criar outra camada por cima dos outro elementos.

=======================================================================

# Fixed

Descrição
Quando aplicado o position fixed é como se criasse um elemento flutuante que fica fixo na página, independente do scrolling feito.

=======================================================================

# Element Stacking

Descrição

É o empilhamento de elementos. Podemos usar o z-index para determinar a ordem da posição do elemento. Quanto maior o z-index, mais "acima" vai aparecer o elemento.

=======================================================================

# Flex

Descrição

Nessa aula vamos ver uma introdução de como posicionar elementos usando o CSS Flexbox

Flexbox

Nos permite posicionar os elementos dentro da caixa
Controle em uma dimensão (horizontal ou vertical)
Alinhamento, direcionamento, ordenar e tamanhos
div.parent {
display: flex;
}

Flex-direction

Qual a direção do flex: horizontal ou vertical
row | column
Alinhamento
justify-content
align-items

=======================================================================

# Grid

- Posicionamento do elemento dentro da caixa.
- Posicionamento horizontal e vertical ao mesmo tempo.
- pode ser flexível ou fixo.
- cria espaços para os elementos filhos habitarem.

HTML

<body>
  <header>Topo</header>
  <main>Conteúdo</main>
  <aside>Informações adicionais</aside>
  <footer>Rodapé</footer>
</body>

CSS

body {
margin: 0;
height: 100vh;
display: grid;
grid-template-areas:
"header header"
"main aside" /_ as aspas vai definir quantas linhas vai ter meu layout, dentro vou definir as colunas. _/
"footer footer";

grid-template-rows: 80px 1fr 100px; /_ vai definir o tamanho das linhas _/
/_ 1fr => vai preencher tudo que tenho de espaço, ela é flexível ao tamanho da página..._/
grid-template-columns: 1fr 200px; /_ vai definir o tamanho das colunas_/
}

header {

grid-area: header; /_ vai definir a posição que cada um vai ocupar_/
background-color: green;
}

main { display:flex; /_ como teste coloquei um display: flex; para alinhar o conteúdo ao meio, junto com as propriedades_/
grid-area: main;
background-color: red;
justify-content: center; /_ teste_/
align-items: center; /_ teste_/

}

aside {
grid-area: aside;
background-color: blue;
}

footer {
grid-area: footer;
background-color: gray;
}

=======================================================================

# Grid ou Flexbox

Podemos usar o Display Flex e Display Grid ao mesmo tempo.
Mas não no mesmo elemento, um pode dar conflito com o outro.
