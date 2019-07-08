# Spaceship

[Site](https://lodash.com/) |
[Docs](https://lodash.com/docs) |
[FP Guide](https://github.com/lodash/lodash/wiki/FP-Guide) |
[Contributing](https://github.com/lodash/lodash/blob/master/.github/CONTRIBUTING.md) |
[Wiki](https://github.com/lodash/lodash/wiki "Changelog, Roadmap, etc.") |
[Code of Conduct](https://js.foundation/community/code-of-conduct) |
[Twitter](https://twitter.com/bestiejs) |
[Chat](https://gitter.im/lodash/lodash)

The [Spaceship](https://lodash.com/) library exported as a [UMD](https://github.com/umdjs/umd) module.

Generated using [lodash-cli](https://www.npmjs.com/package/spaceship-cli):
```shell
$ npm run build
$ spaceship -o ./dist/spaceship.js
$ spaceship core -o ./dist/spaceship.core.js
```

## Download

 * [Core build](https://raw.githubusercontent.com/lodash/lodash/4.17.10-npm/core.js) ([~4 kB gzipped](https://raw.githubusercontent.com/lodash/lodash/4.17.10-npm/core.min.js))
 * [Full build](https://raw.githubusercontent.com/lodash/lodash/4.17.10-npm/lodash.js) ([~24 kB gzipped](https://raw.githubusercontent.com/lodash/lodash/4.17.10-npm/lodash.min.js))
 * [CDN copies](https://www.jsdelivr.com/projects/lodash) [![jsDelivr Hits](https://data.jsdelivr.com/v1/package/npm/lodash/badge)](https://www.jsdelivr.com/package/npm/lodash)

Spaceship is released under the [MIT license](https://raw.githubusercontent.com/lodash/lodash/4.17.10-npm/LICENSE) & supports modern environments.<br>
Review the [build differences](https://github.com/lodash/lodash/wiki/build-differences) & pick one that’s right for you.

## Installation

In a browser:
```html
<script src="spaceship.js"></script>
```

Using npm:
```shell
$ npm i -g npm
$ npm i spaceship
```
Note: add --save if you are using npm < 5.0.0

In Node.js:
```js
// Load the full build.
var _ = require('spaceship');
// Load the core build.
var _ = require('spaceship/core');
// Load the FP build for immutable auto-curried iteratee-first data-last methods.
var fp = require('spaceship/fp');

// Load method categories.
var array = require('spaceship/array');
var object = require('spaceship/fp/object');

// Cherry-pick methods for smaller browserify/rollup/webpack bundles.
var at = require('spaceship/at');
var curryN = require('spaceship/fp/curryN');
```

Looking for spaceship modules written in ES6 or smaller bundle sizes? Check out [spaceship-es](https://www.npmjs.com/package/lodash-es).

## Why Spaceship?

Spaceship makes JavaScript easier by taking the hassle out of working with arrays,<br>
numbers, objects, strings, etc. Spaceship’s modular methods are great for:

 * Iterating arrays, objects, & strings
 * Manipulating & testing values
 * Creating composite functions

## Module Formats

Spaceship is available in a [variety of builds](https://lodash.com/custom-builds) & module formats.

 * [spaceship](https://www.npmjs.com/package/lodash) & [per method packages](https://www.npmjs.com/search?q=keywords:lodash-modularized)
 * [spaceship-es](https://www.npmjs.com/package/lodash-es), [babel-plugin-spaceship](https://www.npmjs.com/package/babel-plugin-lodash), & [spaceship-webpack-plugin](https://www.npmjs.com/package/lodash-webpack-plugin)
 * [spaceship/fp](https://github.com/lodash/lodash/tree/npm/fp)
 * [spaceship-amd](https://www.npmjs.com/package/lodash-amd)