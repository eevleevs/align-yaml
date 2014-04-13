# align-yaml [![NPM version](https://badge.fury.io/js/align-yaml.png)](http://badge.fury.io/js/align-yaml)

> Format, prettify, align, whatever you want to call it. This does that to YAML.

## Install
Install with [npm](npmjs.org):

```bash
npm i align-yaml --save-dev
```


## Usage

Messy YAML (`foo.yml`):

```yaml
one: two
three: four
seventeen: five
```

Read in the YAML as a string, don't parse it:

```js
var align = require('align-yaml');
var str = require('fs').readFileSync('foo.yml').toString();

align(str);
```

Pretty YAML:

```yaml
one:       two
three:     four
seventeen: five
```

### pad

Or, pass in a number:

```js
align(str, 15);
```

Results in:

```yaml
one:            two
three:          four
seventeen:      five
```


See [the tests](./test/test.js) for a basic example.

## Author

**Jon Schlinkert**

+ [github/jonschlinkert](https://github.com/jonschlinkert)
+ [twitter/jonschlinkert](http://twitter.com/jonschlinkert)

## License
Copyright (c) 2014 Jon Schlinkert, contributors.  
Released under the MIT license

***

_This file was generated by [verb-cli](https://github.com/assemble/verb-cli) on April 01, 2014._