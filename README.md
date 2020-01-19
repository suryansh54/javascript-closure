# Javascript Closure

- JavaScript variables can belong to the local or global scope.
- Global variables can be made local (private) with closures.

```javascript
var add = (function () {
  var counter = 0;
  return function () {counter += 1; return counter}
})();

add();
add();
add();

console.dir(add)
// the counter is now 3
```
