## Utilidades

- now

```javascript
//jQuery
$.now();

//Javascript
(new Date).getTime();
```

- isArray

```javascript
//jQuery
$.isArray(arr);

//Javascript (IE9+)
Array.isArray(arr);
```

- inArray

```javascript
//jQuery
$.inArray(searchElement, arr);

//Javascript (IE9+)
(arr.indexOf(searchElement) !== -1) ? true : false;
```

- noop

```javascript
//jQuery
$.noop();

//Javascript
function(){};
```