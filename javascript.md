# JavaScript and jQuery Snippets

### Debugging

Put in Ajax to help find errors:

```js
error: function(xhr){
       console.log(xhr.responseText)
     }
 ```

 Pry.js:

 ```js
 pry = require('pryjs')
 eval(pry.it)
 ```