## Conseguindo e modificando informações dos elementos do DOM

- Conseguindo e modificando valores de inputs.

```javascript
  //jQuery

  // Conseguindo
  var TextboxValue = $("#TextboxID").val(); 
  // Modificando
  $("#TextboxID").val("Seu novo texto aqui.");

  //Javascript puro
  
  // Conseguindo
  var TextboxValue = document.getElementById('#TextboxID').value;
  // Modificando
  document.getElementById('#TextboxID').value = "Seu novo texto aqui.";	
```
Exemplo:  http://jsfiddle.net/jhonylucas74/9fuo1cmo/2/

- Adicionando css a um componente.

Do mesmo modo que foi feito no exemplo anterior é possível atribuir um novo estilo aos elementos da sua página.

```javascript
  //jQuery
  $("#target").css("color", "red"); 
  
  //Javascript puro
  document.getElementById("target").style = "color: red; ";   
```
Exemplo: http://jsfiddle.net/jhonylucas74/7bga826L/1/


- Alterando o html de um componente.

```javascript
  //jQuery
   var DivHTML = $("#DivID").html();
   $("#DivID").html("<p>Esse é nosso novo html.</p>");
  
  //Javascript puro
  document.getElementById("DivHTML").innerHTML = "Esse é nosso novo html.";
```
Exemplo: http://jsfiddle.net/jhonylucas74/37heuzwx/


- Conseguindo e alterando a altura(height) e a largura(width) dos elementos.

```javascript
  //jQuery
  var ElementHeight = $("#DivID").height();
  $("#DivID").height(300);
  
  var ElementWidth = $("#DivID").width();
  $("#DivID").width(300);

  //Javascript puro
  var ElementHeight = document.getElementById("DivID").clientHeight;
  document.getElementById("DivID").style.height = '300px';

  var ElementWidth  = document.getElementById("DivID").clientWidth ;
  document.getElementById("DivID").style.width = '300px';  
```
Exemplo: http://jsfiddle.net/jhonylucas74/6r18kq9w/