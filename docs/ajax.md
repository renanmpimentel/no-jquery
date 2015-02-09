## Ajax

- Post

```javascript
// jQuery
$.ajax({
  type: 'POST',
  url: 'www.example.com',
  data: data
});

// Javascript puro
var request = new XMLHttpRequest();
request.open('POST', 'www.example.com', true);
request.setRequestHeader('Content-Type', 'application/x-www-form-urlencoded');
request.send(data);
```
