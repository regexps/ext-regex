# ext-regex [![NPM version](https://badge.fury.io/js/ext-regex.svg)](http://badge.fury.io/js/ext-regex)

> Regular expression for matching file extensions. Matches single and/or multiple file extensions, like `.min.js`.

## Install with [npm](npmjs.org)

```bash
npm i ext-regex --save
```

## Usage

```js
var extRegex = require('ext-regex');

'a/b/c.min.js'.match(extRegex());
//=> ['.min.js', '.js', 'js'];

'a/b/c/.gitignore'.match(extRegex());
//=> ['.gitignore', '.gitignore', 'gitignore']

'a/b/c'.match(extRegex());
//=> null

'a/b/c.js'.test(extRegex());
//=> true
```

## Run tests

Install dev dependencies:

```bash
node i -d && mocha
```

## Contributing
Pull requests and stars are always welcome. For bugs and feature requests, [please create an issue](https://github.com/regexps/ext-regex/issues)

## Author

**Jon Schlinkert**
 
+ [github/jonschlinkert](https://github.com/jonschlinkert)
+ [twitter/jonschlinkert](http://twitter.com/jonschlinkert) 

## License
Copyright (c) 2015 Jon Schlinkert  
Released under the MIT license

***

_This file was generated by [verb](https://github.com/assemble/verb) on January 12, 2015._
