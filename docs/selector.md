## Elemento de seleção

-  id
	
```javascript
	//jQuery
	jQuery("#nome-div");
	
	//Javascript puro
	document.getElementById('nome-div');

	document.querySelector('#nome-div');
```
Exemplo: http://jsfiddle.net/renanmpimentel/0a2oo703/

- class
```javascript
	//jQuery
	jQuery('.nome-class');

	//Javascript puro
	document.getElementsByClassName('.nome-class'); 	
	
	document.querySelectorAll('.nome-class');
```
Exemplo: http://jsfiddle.net/renanmpimentel/nyez204L/

- tag name
```javascript
	//jQuery
	jQuery('div');

	//Javascript puro
	document.getElementsByTagName('div'); 
	
	document.querySelectorAll('div');
```

Exempĺo:  http://jsfiddle.net/renanmpimentel/0h5vcyah/

- pseudo-class

```javascript
	//jQuery
	jQuery ('#nome-div :first-child');
	
	//Javascript puro
	document.querySelectorAll('#nome-div :first-child');
```

Exemplo: http://jsfiddle.net/renanmpimentel/nd31ov1n/1/

- children

```javascript

	// jQuery
	jQuery('#div-parent').children();

	//Javascript puro
	document.getElementById('div-parent').childNodes;

	document.getElementById('div-parent').children
```

Exemplo: http://jsfiddle.net/renanmpimentel/7o5gcga0/