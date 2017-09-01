Bcccore Build
=======

A helper to add tasks to gulp.

## Attribution

This repository was created by copy forking [btccore-build 54e79cf](https://github.com/owstack/btccore-build/commit/54e79cfe5404c37ead8073e13cff2a4574ded952).

## Getting started

Install with:

```sh
npm install bcccore-build
```

and use and require in your gulp file: 

```javascript
var gulp = require('gulp');
var bcccoreTasks = require('bcccore-build');

bcccoreTasks('submodule');
gulp.task('default', ['lint', 'test', 'browser', 'coverage']);
```

### Notes

* There's no default task to allow for each submodule to set up their own configuration
* If the module is node-only, avoid adding the browser tasks with:
```javascript
var bcccoreTasks = require('bcccore-build');
bcccoreTasks('submodule', {skipBrowsers: true});
```

## Contributing

See [CONTRIBUTING.md](https://github.com/owstack/bcccore-lib) on the main bcccore-lib repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/owstack/bcccore-lib/blob/master/LICENSE).

Copyright 2017 Open Wallet Stack. Bcccore is a trademark maintained by Open Wallet Stack.
