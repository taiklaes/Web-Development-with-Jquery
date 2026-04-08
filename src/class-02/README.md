# Manipulação de Elementos com jQuery
Este conteúdo apresenta métodos do jQuery para manipulação de elementos HTML, focando em eventos e efeitos visuais.

## Eventos com on
- Define um ou mais eventos para um elemento
- Permite associar funções a interações do usuário

## Exibir e ocultar elementos
- `hide`: oculta o elemento
- `show`: mostra o elemento
- Parâmetros opcionais:
  - velocidade (speed)
  - função callback (executada ao final)

## Alternância de exibição
- `toggle`: alterna entre ocultar e mostrar um elemento
- Também aceita speed e callback

## Efeitos de fade
- Aplicam transições suaves de opacidade
- Métodos:
  - `fadeIn`: exibe gradualmente
  - `fadeOut`: oculta gradualmente
  - `fadeToggle`: alterna entre mostrar e ocultar
  - `fadeTo`: ajusta a opacidade
- Aceitam parâmetros opcionais (speed e callback)

## Efeitos de slide
- Criam animações de deslizamento
- Métodos:
  - `slideDown`: exibe deslizando para baixo
  - `slideUp`: oculta deslizando para cima
  - `slideToggle`: alterna entre slideDown e slideUp
- Aceitam parâmetros opcionais (speed e callback)

## Exemplo
```js
$(document).ready(function() {
  $("#botao").on("click", function() {
    $("#elemento").fadeToggle(500);
  });

  $("#mostrar").on("click", function() {
    $("#elemento").show(300);
  });

  $("#ocultar").on("click", function() {
    $("#elemento").hide(300);
  });
});
```