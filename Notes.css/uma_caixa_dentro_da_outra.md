# Display-block-inline

Descrição

display: block; vs display: inline;
Como as caixas se comportam em relação as outras caixas
Comportamento externo das caixas

## Display Block

Ocupa toda a linha, colocando o próximo elemento abaixo

    * width e height são respeitados
    * padding, margin, border irão funcionar normalmente
    * <p> <div> <section>, todos os headings <h1> <h2>...

## Display Inline

Os elementos ficam ao lado do outro e não empurram outros elementos para baixo
_ width e height não funcionam
_ Somente valores horizontais de margin

<a> <strong> <span> <em>

========================================================================================

# Margin

    é o espaço (margem) entre os elementos

Podemos dividir o margin em 4 valores:
/_ margin-top | margin-right | margin-bottom | margin-left _/
values: <length> | <percentage> | auto

Geralmente usamos uma forma abreviada (shorthand) para escrever o margin. Esse formato segue o sentido horário iniciando pelo top, seguindo para right, bottom e left.

margin: 12px 16px 10px 4px; /_ TOP = 12px | RIGHT = 16px | BOTTOM = 10px | LEFT = 4px _/
margin: 12px 16px 0; /_ TOP = 12px | RIGHT = 16px | BOTTOM = 0px | LEFT = 16px _/
margin: 8px 16px; /_ TOP = 8px | RIGHT = 16px | BOTTOM = 8px | LEFT = 16px _/
margin: 8px; /_ TOP = 8px | RIGHT = 8px | BOTTOM = 8px | LEFT = 8px _/
O margin é aplicado em elementos com display block
Cuidado com o margin collapsing que é quando o top se junta ao bottom

========================================================================================

# Padding

Descrição
O padding é o preenchimento interno da caixa.

A propriedade padding pode ser escrita como nos formatos apresentados abaixo:
padding-top | padding-right | padding-bottom | padding-left
Geralmente usamos uma forma abreviada (shorthand) para escrever o padding. Esse formato segue o sentido horário iniciando pelo top, seguindo para right, bottom e left.

padding: 12px 16px 10px 4px; /_ TOP = 12px | RIGHT = 16px | BOTTOM = 10px | LEFT = 4px _/
padding: 12px 16px 0; /_ TOP = 12px | RIGHT = 16px | BOTTOM = 0px | LEFT = 16px _/
padding: 8px 16px; /_ TOP = 8px | RIGHT = 16px | BOTTOM = 8px | LEFT = 16px _/
padding: 8px; /_ TOP = 8px | RIGHT = 8px | BOTTOM = 8px | LEFT = 8px _/
O padding pode ter valores (values) de comprimento (px, em, rem) ou de porcentagem (%)

O padding poderá causar diferença na largura de um elemento
obs.: Na aula sobre box-xizing aprendemos como resolver essa diferença na largura do elemento

# https://app.rocketseat.com.br/node/uma-caixa-dentro-da-outra/lesson/box-sizing

# Border-outline

Descrição
São as bordas da caixa

Documentação do MDN: https://developer.mozilla.org/en-US/docs/Web/CSS/border

value: <border-style> | <border-width> | <border-color>

style: solid | dotted | dashed | double | groove | ridge | inset | outset
width: <length>
color: <color>
div {
/_ shorthand _/
border-top: solid 2px; /_ top | right | bottom | left _/

    /* style */
    border: solid;

    /* width <length> | style */
    border: 2px dotted;

    /* style | color */
    border: outset #f33;

    /* width | style | color */
    border: medium dashed green;

}
E o outline?
O outline é muito semelhante ao border, mas difere em 4 sentidos:
Não modifica o tamanho da caixa, pois não é parte do Box Model
Poderá ser diferente de retangular
Não permite ajuste individuais
Mais usado pelo user agent para acessibilidade
