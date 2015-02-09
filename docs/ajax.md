## Ajax

- Post

```javascript
// jQuery
jQuery.ajax({
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

- Request
```javascript
// jQuery
jQuery.ajax({
  type: 'GET',
  url: 'www.example.com',
  success: function(data) {
    console.log(data)
  },
  error: function() {

  }
});

// Javascript puro
var request = new XMLHttpRequest();
request.open('GET', 'www.example.com');

request.onreadystatechange = function(){
    if (request.status === 200 && request.readyState === 4){
        console.log(request.responseText);
    }
};

request.send();
```
