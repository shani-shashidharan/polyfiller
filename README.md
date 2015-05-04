# Polyfiller

[![npm version](https://badge.fury.io/js/polyfiller.svg)](http://badge.fury.io/js/polyfiller)
[![Build Status](https://travis-ci.org/monolithed/polyfiller.png)](https://travis-ci.org/monolithed/polyfiller)
[![Coverage Status](https://coveralls.io/repos/monolithed/polyfiller/badge.svg)](https://coveralls.io/r/monolithed/polyfiller)
[![Dependency Status](https://david-dm.org/monolithed/polyfiller.svg)](https://david-dm.org/monolithed/polyfiller)
[![License](https://img.shields.io/badge/license-MIT-brightgreen.svg)](LICENSE.txt)


[![Sauce Test Status](https://saucelabs.com/browser-matrix/monolithed.svg)](https://saucelabs.com/u/monolithed)

> A polyfill combinator

## Getting Started
This package requires Node `~0.10.0`

If you haven't used [npm](https://www.npmjs.com/) before, be sure to check out the [Getting Started](https://nodejs.org/community/) guide, as it explains how to install [npm](https://docs.npmjs.com/getting-started/installing-node) and use a [package.json](https://docs.npmjs.com/files/package.json) file. 
Once you're familiar with that process, you may install this package with this command:

```shell
npm install polyfiller --save-dev
```

Once the package has been installed, it may be used inside your files with this line of JavaScript:

```js
var Polyfiller = require('polyfiller');
```

### Usage Example

```js
var polyfiller = new Polyfiller;

var list = polyfiller.find([ 'Promise' ]),
	code = polyfiller.pack(list);
```


### Catalog

A list of all of available features

|           Feature             |                 What's included?                 |
|:------------------------------|:------------------------------------------------ |
| Array.from                    | [Array.from](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Array/from) |
| Array.prototype.find          | [Array.prototype.find](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Array/find) |
|  Array.prototype.findIndex    | [Array.prototype.findIndex](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Array/findIndex) |
|  Collections                  | [Set](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Set)<br /> [Map](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Map)<br /> [WeakSet](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/WeakSet)<br /> [WeakMap](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/WeakMap)<br />  |
|  CSS.escape                   | [CSS.escape](https://developer.mozilla.org/en-US/docs/Web/API/CSS/escape) |
|  DOM4                         | [CustomEvent](https://developer.mozilla.org/en-US/docs/Web/API/CustomEvent)<br /> [Element#prepend()](https://dom.spec.whatwg.org/#dom-parentnode-prependnodes)<br /> [Element#append()](https://dom.spec.whatwg.org/#dom-parentnode-appendnodes)<br /> [Element#before()](https://dom.spec.whatwg.org/#dom-childnode-beforenodes)<br /> [Element#after()](https://dom.spec.whatwg.org/#dom-childnode-afternodes)<br /> [Element#replaceWith()](https://dom.spec.whatwg.org/#dom-childnode-replacewithnodes)<br /> [Element#remove()](https://dom.spec.whatwg.org/#dom-childnode-remove)<br /> [Element#query](https://dom.spec.whatwg.org/#dom-elements-queryrelativeselectors)<br /> [Element#queryAll](https://dom.spec.whatwg.org/#dom-elements-queryallrelativeselectors)<br /> [Element#matches](https://dom.spec.whatwg.org/#dom-element-matchesselectors)<br /> [Element#closest](https://dom.spec.whatwg.org/#dom-element-closestselectors)<br /> [Element.classList](https://developer.mozilla.org/en-US/docs/Web/API/Element/classList) |
|  EventSource                  | [EventSource](https://developer.mozilla.org/en-US/docs/Web/API/EventSource) |
|  Promise                      | [Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise) |
|  Reflect                      | [Reflect](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Reflect) |
|  URL                          | [URL](https://developer.mozilla.org/en-US/docs/Web/API/URL) |
|  WindowBase64                 | [WindowBase64](https://developer.mozilla.org/en-US/docs/Web/API/WindowBase64) |
|  Fetch                        | [window.fetch](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API) <br /> [GlobalFetch](https://developer.mozilla.org/en-US/docs/Web/API/GlobalFetch) <br /> [Body](https://developer.mozilla.org/en-US/docs/Web/API/Body) <br /> [Headers](https://developer.mozilla.org/en-US/docs/Web/API/Headers) <br /> [Request](https://developer.mozilla.org/en-US/docs/Web/API/Request) <br /> [Response](https://developer.mozilla.org/en-US/docs/Web/API/Response) |
|  Object.getOwnPropertySymbols | [Object.getOwnPropertySymbols](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Object/getOwnPropertySymbols) | 
| String/fromCodePoint          | [String/fromCodePoint](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/String/fromCodePoint) | 
| RegExp.prototype.search       | [RegExp.prototype.search](http://people.mozilla.org/~jorendorff/es6-draft.html#sec-regexp.prototype.search) | 
| RegExp.prototype.match        | [RegExp.prototype.match](http://people.mozilla.org/~jorendorff/es6-draft.html#sec-regexp.prototype.match) | 
|  String.prototype.includes    | [String.prototype.includes](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/String/includes) | 
|  String.prototype.at    | [String.prototype.at](https://github.com/mathiasbynens/String.prototype.at) | 
|  String.prototype.codePointAt    | [String.prototype.codePointAt](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/String/codePointAt) | 
|  String.prototype.normalize   | [String.prototype.normalize](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/String/normalize) | 
|  String.prototype.startsWith  | [String.prototype.startsWith](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/String/startsWith) | 
|  String.prototype.endsWith  | [String.prototype.endsWith](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/String/endsWith) | 
|  String.prototype.repeat  | [String.prototype.repeat](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/String/repeat) | 
|  window.requestAnimationFrame | [window.requestAnimationFrame](https://developer.mozilla.org/ru/docs/DOM/window.requestAnimationFrame)| 
|  document.scrollingElement    | [document.scrollingElement](http://dev.w3.org/csswg/cssom-view/#dom-document-scrollingelement) |
|  window.setImmediate          | [window.setImmediate](https://developer.mozilla.org/ru/docs/Web/API/Window/setImmediate) |
|  TextEncoder                  | [TextEncoder](https://developer.mozilla.org/en-US/docs/Web/API/TextEncoder) |


### Compatibility

Theoretically compatible with all contemporary browsers since **IE9**<br />
For **IE8** only it's recommended to include [ie8](https://github.com/WebReflection/ie8) script before your build

### Methods

#### find

Type: `Function (feature, name)` <br />
Returns: `Array`

Returns an unordered bundle of polyfills as an array of objects

```js
var polyfiller = new Polyfiller;

var list = polyfiller.find(['Promise'], function (feature, name) {
	console.log(name, feature.source, feature.config);
});

list[0].source; // source code
list[0].config.name; // Promise
```


Also available the second format (it may be useful in the future versions):

```js
var polyfiller = new Polyfiller;

var list = polyfiller.find([
	{ 
		name: 'Promise'
	}
],
function (feature, name) {
	console.log(name, feature.source, feature.config);
});
```

#### list

Type: `Function ([extended=false])` <br />
Returns: `Array`

Return a list of all of available features as an array of strings.

```js
var polyfiller = new Polyfiller;

polyfiller.list(); // ['Promise', 'Reflect', 'URL', ...]
```

*extended* option

```js
var polyfiller = new Polyfiller;
var list = polyfiller.list(true);

list; // [{ config }, ...]
list[0].name; // Array.from
list[0].author; // Mathias Bynens
list[0].licenses[0].type; // MIT
...
```

For information see `index.json` file

#### pack

Type: `Function (features)` <br />
Returns: `String`

Packs a list of polyfills into one string

```js
var polyfiller = new Polyfiller;

var list = polyfiller.find([ 'Promise' ]),
	code = polyfiller.pack(list);
```


### Options

#### catalog

Type: `Array` <br />
Default: `[trunk/catalog]`

Have custom polyfills? Add paths to their location here.

```js
var path = require('path');

var polyfiller = new Polyfiller({
	catalog: [ 
		path.resolve(__dirname, '../your/catalog') 
	]
});
```

#### exclude

Type: `Array` <br />
Default: `[]`

Some polyfills have dependencies that you can exclude here

```js
var polyfiller = new Polyfiller({
	exclude: ['setImmediate']
});
```

#### verbose

Type: `Boolean` <br />
Default: `false`

Verbose mode is an option that provides additional details as to what the package is doing.

```js
var polyfiller = new Polyfiller({
	verbose: true
});
```

#### wrapper

Type: `Function` <br />
Default: `None`

A custom wrapper for your environment

```js
var polyfiller = new Polyfiller({
	wrapper: function (source) {
		return ';(function () {' + source + '}.call(self));'
	}
});
```

### Tests

```
grunt test
```

### Contributing

1. Fork the one
2. Create a topic branch
3. Make your commits
4. Write the tests and run `grunt test`
5. Submit Pull Request once Tests are Passing


### license

MIT

Task submitted by [Alexander Abashkin](https://github.com/monolithed)
