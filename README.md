# latest-javascript


## Optional Chaining

Allows the dev to check for nulls in property chains

```javascript
let a = {b: "x"}
if (a?.b) console.log (a.b) // Logs "x"
if (a?.c) console.log (a.c) // Will not log as a.c is null
```
## Destructuring
Allows creating named variables from an incoming object
```javascript
// props: {name: "John", age: 35, height: 187}
let {name, age} = props
console.log(name) // logs "John"
console.log(height) // undefined!
console.log(props.height) // logs 187
```

### Defaulting
You may default a destructuring, in case something is not defined
```javascript
// props: {name: "John", age: 35, height: 187}
let {name, lastName= "Doe"} = props
console.log(name) // logs "John"
console.log(props.lastName) // undefined!
console.log(lastName) // logs "Doe"
```
