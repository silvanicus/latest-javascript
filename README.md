# latest-javascript


#optional chaining
Allows the dev to check for nulls in property chains
```javascript
let a = {b: "x"}
if (a?.b) console.log (a.b) // Logs "x"
if (a?.c) console.log (a.c) // Will not log as a.c is null
```
