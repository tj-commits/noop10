# noop10

> No operation as a module using an arrow function.

## Installation

```sh
# Using npm
npm install noop10

# Using yarn
yarn add noop10

# Using PNPM
pnpm add noop10
```
## Usage

```js
const noop = require('noop10')

noop() // Nothing happened, yay!

function wait(duration, callback) {
  callback = callback || noop
  setTimeout(callback, duration)
}

wait(1000, () => {
  console.log('waited one second')
})

wait(1000) // No error, even though we didn't pass the callback function
```

## Why?
For some reason, `noop6` doesn't actually use an arrow function in the published NPM package (it does in the GitHub repo, however). This package does. 

Still, there are so many noop modules out there. I'm actually working on creating a chart of all of them and their pros and cons and stuff like that. I'll change this README when I'm done with that.

## See also
- [noop6](https://npmjs.com/package/noop6)
- [n0p3](https://npmjs.com/package/n0p3)
- [yanoop](https://npmjs.com/package/yanoop)
- [noop2](https://npmjs.com/package/noop2)
- [noop3](https://npmjs.com/package/noop3)
- [noop4](https://npmjs.com/package/noop4)
- [nop](https://npmjs.com/package/nop)
- [no-op](https://npmjs.com/package/no-op)
- [noop](https://npmjs.com/package/noop)