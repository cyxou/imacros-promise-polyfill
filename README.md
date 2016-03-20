This is a port of [Taylor's Hakes](https://github.com/taylorhakes) [promise-polyfill](https://github.com/taylorhakes/promise-polyfill) for use with iMacros and Browserify.

## Node
```
npm install imacros-promise-polyfill
```

## Simple usage
```js
var Promise = require('imacros-promise-polyfill');

var promise = new Promise(function(resolve, reject) {
  // do a thing, possibly async, then…

  if (/* everything turned out fine */) {
    resolve("Stuff worked!");
  }  else {
    reject(new Error("It broke"));
  }
});

// Do something when async done
promise.then(function() {
  ...
});
```

## License
MIT
