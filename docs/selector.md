## Seletores

- id

```javascript
//jQuery
var obj1 = $("#nome-div");
console.log(obj1);

//Javascript
var obj2 = document.getElementById('nome-div');
console.log(obj2);

// IE8 suporta apenas seletores CSS 2.1
var obj3 = document.querySelector('#nome-div');
console.log(obj3);
```

Caso os elementos não sejam encontrados, `obj2` e `obj3` retornam `null`.

```js
var obj2 = document.getElementById('nome-div');

obj2 == false // false
obj2 == null // true
typeof obj2 // "object"
```

Exemplo: http://jsfiddle.net/ismaelgasparin/0a2oo703/5/

- class

```javascript
//jQuery
var obj1 = $('.nome-class');
console.log(obj1);

//Javascript puro
// IE9+
var obj2 = document.getElementsByClassName('nome-class'); // Retorna um objeto HTMLCollection
console.log(obj2);

// Query
// Throws a SYNTAX_ERR exception if the specified group of selectors is invalid.
var obj3 = document.querySelectorAll('.nome-class'); // Retorna um objeto NodeList
console.log(obj3);

obj2 === obj3 // false
```

Caso os elementos não sejam encontrados, `obj2` retorna um `HTMLCollection` vazio e `obj3` um `NodeList` vazio.

```js
var obj2 = document.getElementsByClassName('nome-class');
!!obj2 // true
obj2.length // 0
obj2.namedItem // function

var obj3 = document.querySelectorAll('nome-class');
!!obj3 // true
obj3.length // 0
obj3.namedItem // undefined

obj2 === obj3 // false
```

Mais diferenças sobre HTMLCollection e NodeList [aqui](http://stackoverflow.com/questions/15763358/difference-between-htmlcollection-nodelists-and-arrays-of-objects)

Exemplo: http://jsfiddle.net/ismaelgasparin/nyez204L/1/

- tag

```javascript
//jQuery
var obj1 = $('div');
console.log(obj1);

//Javascript puro
var obj2 = document.getElementsByTagName('div');
console.log(obj2);

var obj3 = document.querySelectorAll('div');
console.log(obj3);
```

Mais uma vez, `obj2` será uma HTMLCollection e `obj3` uma NodeList.

Exemplo: http://jsfiddle.net/ismaelgasparin/0h5vcyah/1/

- pseudo-class

```javascript
//jQuery
var obj1 = $('#nome-div :first-child');
console.log(obj1);

//Javascript puro
var obj2 = document.querySelectorAll('#nome-div :first-child');
console.log(obj2);
```
Exemplo: http://jsfiddle.net/ismaelgasparin/nd31ov1n/2/

- children

```javascript
// jQuery
var obj1 = $('#div-parent').children();
console.log(obj1);

//Javascript puro
var obj2 = document.getElementById('div-parent').childNodes;
console.log(obj2);

var obj3 = document.getElementById('div-parent').children;
console.log(obj3);
```

Novamente, `obj2` é uma NodeList enquanto `obj3` é uma HTMLCollection.

Exemplo: http://jsfiddle.net/ismaelgasparin/7o5gcga0/1/

- multiple selectors

```javascript
// jQuery
var obj1 = $('div, a, li');
console.log(obj1);

// Javascript puro
var obj2 = document.querySelectorAll('div, a, li');
console.log(obj2);
```

Exemplo: http://jsfiddle.net/ismaelgasparin/ovdtrg1r/1/
