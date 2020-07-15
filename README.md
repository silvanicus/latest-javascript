# Latest Javascript

## Nullish Coalescing
Truly check nullish values instead of falsey values
```javascript
false ?? 'My name is' // false
NaN ?? 'Hello' // NaN
null ?? 'Hello people' // 'Hi'
```

## Optional chaining syntax
Allows to check for nullish values in chains. If if doesn't exist will return `null`
```javascript
const a = {b: "x"}
if (a?.b) console.log (a.b) // Logs "x"
if (a?.c) console.log (a.c) // Will not log as a.c is null

const b = { one: { two: 1, three: null } };
if (b.one?.two) console.log (b.one) // Logs object
if (b.one?.three) console.log (b.one) // Will not log
```

## globalThis
The global object varies depending on the Js platform: `window` for browsers, `global` for Node, and `self` for web workers.
```javascript
// For the browser
globalThis.setTimeout === window.setTimeout;
```

