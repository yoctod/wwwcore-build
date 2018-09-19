# wwwcore-build

A helper to add tasks to gulp.

## Getting started

Install with:

```sh
npm install wwwcore-build
```

and use and require in your gulp file: 

```javascript
var gulp = require('gulp');
var wwwcoreTasks = require('wwwcore-build');

wwcoreTasks('submodule');
gulp.task('default', ['lint', 'test', 'browser', 'coverage']);
```w

### Notes

* There's no default task to allow for each submodule to set up their own configuration
* If the module is node-only, avoid adding the browser tasks with:
```javascript
var wwwcoreTasks = require('wwwcore-build');
litecoreTasks('submodule', {skipBrowsers: true});
```

## Contributing

See [CONTRIBUTING.md](https://github.com/yoctod/wwwcore) on the main litecore repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/yoctod/wwwcore/blob/master/LICENSE).

Copyright 2015 BitPay, Inc. Bitcore is a trademark maintained by BitPay, Inc.
Copyright 2016 The Wwwcoin Core Developers
