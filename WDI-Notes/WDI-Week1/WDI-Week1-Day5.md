# WDI DAY 5
```js
if (true) { console.log('ok') }
else if(false) {}
else {}
```
```js
if (...) console.log('ok')
```
```js
if (person === 'cheryl') {console.log('girl')}
else if (person === 'zi') {console.log('girl')}
else if (person === 'eddie') {console.log('guy')}
else if (person === 'seb') {console.log('guy')}
else console.og('wut')
```
```js
switch(person) {
  case 'cheryl': console.log('girl'); break;
  case 'zi': console.log('girl'); break;
  case 'eddie': console.log('guy'); break;
  case 'seb': console.log('guy'); break;
  default: console.log('wut')
}
```
```js
switch(person) {
  case 'cheryl': console.log('girl'); break;
  case 'zi': console.log('girl'); break;
  case 'eddie':
  case 'seb': console.log('guy'); break;
  default: console.log('wut')
}
```
```js
(person = 'irvin') ? console.log('hello'): console.log('sup')
```

```js
var allowed = age > 18 ? 'yes':
  age > 21 ? 'totally':
  age > 31 ? 'totally':
  age > 41 ? 'totally':
  age > 51 ? 'totally':
  "no";
```

```js
var age = 12
switch(age){
  case age > 18: console.log("yes");
  break
  default: console.log('no')
}
```
#Try & Catch Good Example
```js
var irv = 'irvin'
try {
  irv.toUpperase()
}
catch(err) {
  console.log(err.message)
}

```
#Accessing Object Properties
```js
var person = {
  name:'seb',
  age: 55
}
function foo (o){
  var name = o && o.name
  var age = o && o.age
  console.log(name)
  console.log(age)
}
foo(person)
```
#ES6 Syntax
```js
a = [1,2,3,4,5]
[1, 2, 3, 4, 5]
a.forEach(function(num){ console.log(num) })
a.forEach(num => console.log(num))
a.map(number => number * 2)
```

-LUNCH-

```js
document.querySelectorAll('img')
document.querySelectorAll('footer .grid-row .column p:nth-of-type(2) a')
```
```js
Inserting into HTML - creating new elements
var seb = document.createElement('div')
seb.innerHTML = 'Hello there'
var footer = document.querySelector('footer')
footer.appendChild(seb)
```
```js
var people = ['alice','bob', 'charlie']
people.forEach(function(person){
  var element = document.createElement('h1')
  //<h1>Person</h1>
  element.textContent = person
  document.querySelector('header').appendChild(element)
})
```
innerHTML VS textContent -> Links
impt. user profile inject malicious
force it to be text

-REMOVE ELEMENT-
```js
Array.from(document.querySelectorAll('header h1'))
  .filter(function (element) {
    console.log(element.id)
})
Array.from(document.querySelectorAll('header h1'))
  .filter(function (element) {
    return(element.id !== 'singapore_title')
})
document.querySelectorAll('header h1:not(#singapore_title)')
```
```js
Array.from(document.querySelectorAll('header h1')).filter(
  element => element.id != 'singapore_title').forEach(
    element => element.remove())
```
