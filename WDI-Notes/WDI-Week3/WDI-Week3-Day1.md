bind - when you use foreach for a this object - usually it is undefined.
now it is in context

class Person {
  hello () {
    console.log(this)
    this.name.split('')
      // .forEach(function (character) {
      //   console.log(this)
      // }, this)
      .forEach(character => {
        console.log(this)
      })
  }
}

var seb = new Person()
seb.name = 'Sebastiaan'
seb.hello()

var cheryl = new Person()
cheryl.name = 'Cheryl'
cheryl.hello()

// var firstname = 'sebastiaan'
// var lastname = "deckers"
// var fullname = firstname + lastname
// function greet (name) {
//   return 'My name is ' + name
// }
// function toHtml () {
//   console.log(arguments)
// }
// var greeting = toHtml`Hello ${greet(fullname)} + 'test'`

// console.log(`System error ${error}`)

// 'sebastiaan'.split('')
//   .map(value => {
//     let upper = value.toUpperCase()
//     return upper + upper
//   })
//   .map(function (value) { return value.toUpperCase() })

// const namedFunction = value => value.toUpperCase()
// function iterator (value) {
//   return value.toUpperCase()
// }

- import looks for package.json file. e.g import express. 
