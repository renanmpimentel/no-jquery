##Efeitos

- show

```javascript
//jQuery
$(el).show();

//Javascript puro
//IE8+
el.style.display = '';
```

Exemplo: [http://jsfiddle.net/felfis/21chns8e/](http://jsfiddle.net/felfis/21chns8e/)

- hide

```javascript
//jQuery
$(el).hide();

//Javascript puro
//IE8+
el.style.display = 'none';
```

Exemplo: [http://jsfiddle.net/felfis/u7dpsfrk/2/](http://jsfiddle.net/felfis/u7dpsfrk/2/)

- fadeIn

```javascript
//jQuery
$(el).fadeIn();

//Javascript puro
//IE9+
function fadeIn(el) {
  el.style.opacity = 0;

  var last = +new Date();
  var tick = function() {
    el.style.opacity = +el.style.opacity + (new Date() - last) / 400;
    last = +new Date();

    if (+el.style.opacity < 1) {
      (window.requestAnimationFrame && requestAnimationFrame(tick)) || setTimeout(tick, 16)
    }
  };

  tick();
}

fadeIn(el);
```

Exemplo: [http://jsfiddle.net/felfis/3prqegc0/2/](http://jsfiddle.net/felfis/3prqegc0/2/)

- fadeOut

```javascript
//jQuery
$(el).fadeOut();

//Javascript puro
//IE9+
function fadeOut() {
  var effect = setInterval(function() {
    if (!el.style.opacity) {
      el.style.opacity = 1;
    }
    if (el.style.opacity < 0.1) {
      clearInterval(effect);
    } else {
      el.style.opacity -= 0.1;
    }
  }, 50);
};

var el = document.getElementById('nome-da-div');
fadeOut();

```

Exemplo: [http://jsfiddle.net/guuibayer/dq00f8wj/](http://jsfiddle.net/guuibayer/dq00f8wj/)

