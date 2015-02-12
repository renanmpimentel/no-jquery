## Seletores

- id

```javascript
//jQuery
var obj1 = $("#nome-div");
console.log(obj1);

//Javascript
var obj2 = document.getElementById('nome-div');
console.log(obj2);

var obj3 = document.querySelector('#nome-div');
console.log(obj3);
```
Exemplo: http://jsfiddle.net/ismaelgasparin/0a2oo703/5/

- class

```javascript
//jQuery
var obj1 = $('.nome-class');
console.log(obj1);

//Javascript puro
var obj2 = document.getElementsByClassName('.nome-class');	
console.log(obj2);

var obj3 = document.querySelectorAll('.nome-class');
console.log(obj3);
```
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
