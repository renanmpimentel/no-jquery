# #NOJQUERY

A ideia aqui não é crucificar o jQuery que ajudou e ajuda muitos desenvolvedores na hora de programar e etc. Mas sim, mostrar que antes de usar qualquer _framework_ ou _biblioteca_ __javascript__ devemos ter um conhecimento da linguagem base. 

Muitas vezes, carregamos o _jQuery_ para utilizar um evento _click_ ou _ajax_, então vamos mostrar exemplos de como usar o__ javascript__ puro, para tarefas básicas no seu desenvolvimento.


## Elemento de seleção

-  id
	
```javascript
	//jQuery
	$("#name-div");
	
	//Javascript puro
	document.getElementById('nome-div');

	document.querySelector('#nome-div');
```

- class
```javascript
	//jQuery
	$('.nome-class')

	//Javascript puro
	document.getElementsByClassName('.nome-class') 	
	
	document.querySelectorAll('.nome-class')
```
