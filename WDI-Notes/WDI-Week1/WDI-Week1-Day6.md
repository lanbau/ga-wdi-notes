- create branch
- Recursive needs
  - base case to end recursion
  - function(n - 1) - to bring n towards base case
```js
function factorial(n) {
  if (n < 0) {
    return;
  }
  // Base case
  if (n === 0) {
    return 1;
  }
  return n * factorial(n-1);
}
factorial(6);
```
---LUNCH---
//Detach child from parent
//before parent had to figure out how to //accomodate child
//fixing to the viewport of the screen
position:fixed
//relative to main/body - nearest ancestor with position:relative
position:absolute
//body is the screen - 5000px element inside will overflow
//if there is no nearest ancestor with relative, element follows viewport

div::before {
  content:'a'
}

JS
#Timers - timeout
```js
setTimeout(function() { console.log('hello') }, 3000) - timeout id: # used to stop timer
setInterval(function() { console.log('hello') }, 1000)
var timer = setInterval(function(){ console.log('are we there yet'), 50})
clearInterval(timer)
```
parseInt('25px') + 10 + 'px'

canvas
