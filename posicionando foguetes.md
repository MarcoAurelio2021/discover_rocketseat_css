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
