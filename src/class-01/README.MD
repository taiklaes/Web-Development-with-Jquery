# Introdução à jQuery
Esta repositório contém os conceitos iniciais do jQuery, incluindo sua finalidade, formas de utilização e sintaxe básica para manipulação de elementos HTML.

## O que é jQuery?
- Biblioteca JavaScript muito popular;
- Simplifica tarefas comuns como:
  - Manipulação de HTML/DOM
  - CSS
  - Eventos
  - Animações e efeitos
  - Ajax
  - Utilitários

## Instalação
### Download
- Baixar em: https://jquery.com
- Incluir o arquivo no projeto via `<script>`

### CDN
- Carrega de servidores externos
- Vantagens:
  - Mais rápido (cache)
  - Servidor mais próximo do usuário

## Origem do nome
- **J** = JavaScript  
- **Query** = consulta  
- - Permite selecionar elementos e aplicar ações

## Sintaxe básica
```js
$(seletor).acao()
```
- `$` → indica uso do jQuery
- `seletor` → elemento HTML (tag, classe, id…)
- `acao` → método aplicado

## Exemplos
```js
$(this).hide()        // Oculta o elemento atual
$("p").hide()         // Oculta todos os parágrafos
$(".test").hide()     // Oculta elementos com classe "test"
$("#test").hide()     // Oculta elemento com id "test"
```

## Execução do jQuery
```js
$(document).ready(function(){});
```
ou
```js
$(function(){});
```
Garante que o código execute após o carregamento da página

## Seletores
- Baseados em CSS
- Selecionam elementos para manipulação

### Tipos comuns
```js
$("p")              // Elemento
$(".classe")        // Classe
$("#id")            // ID
```

### Outros seletores
```js
$("*")                     // Todos elementos
$(this)                    // Elemento atual
$("p.intro")               // <p> com classe intro
$("p:first")               // Primeiro <p>
$("ul li:first")           // Primeiro <li> dentro de <ul>
$("[href]")                // Elementos com atributo href
$("a[target='_blank']")    // Links com target _blank
$(":button")               // Botões
$("tr:even")               // Linhas pares
$("tr:odd")                // Linhas ímpares
```

## Onde declarar
- Dentro da tag `<script>`
- Preferencialmente no `<head>`
- Ou em arquivo JS separado

## Eventos (DOM)
Ações do usuário na página:
- Mouse: `click`, `dblclick`, `mouseenter`, `mouseleave`
- Teclado: `keypress`, `keydown`, `keyup`
- Formulário: `submit`, `change`, `focus`, `blur`
- Janela: `load`, `resize`, `scroll`, `unload`

## Evento click
Executa uma função ao clicar no elemento
```js
$("p").click(function(){
  // ação aqui
});
```
