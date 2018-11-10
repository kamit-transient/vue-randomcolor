# vue-randomcolor

Tiny Vue.js wrapper for the [randomcolor](https://github.com/davidmerfield/randomColor) package, less than `1 KB` minified.

## Installation

Install via npm:

```sh
npm install --save vue-randomcolor randomcolor
```

Then you can install it as a Vue plugin:

```js
import Vue from 'vue'
import VueRandomColor from 'vue-randomcolor'

Vue.use(VueRandomColor)
```

vue-randomcolor will take care of importing randomcolor automatically.

## Usage

After installation, randomcolor is bound to `this` in every single file component:

```js
this.$randomColor();
// outputs e.g. #ffda63
```

Of course, all [randomcolor options](https://github.com/davidmerfield/randomColor#options) can be used with the function:

```js
this.$randomColor({ luminosity: 'light', hue: 'red' })
// outputs e.g. #f293ac
```