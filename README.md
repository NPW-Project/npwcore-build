# npwcore-build

A helper to add tasks to gulp.

## Getting started

Install with:

```sh
npm install npwcore-build
```

and use and require in your gulp file: 

```javascript
var gulp = require('gulp');
var npwcoreTasks = require('npwcore-build');

npwcoreTasks('submodule');
gulp.task('default', ['lint', 'test', 'browser', 'coverage']);
```

### Notes

* There's no default task to allow for each submodule to set up their own configuration
* If the module is node-only, avoid adding the browser tasks with:
```javascript
var npwcoreTasks = require('npwcore-build');
npwcoreTasks('submodule', {skipBrowsers: true});
```

## Contributing

See [CONTRIBUTING.md](https://github.com/npw-projcet/npwcore) on the main npwcore repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/npw-project/npwcore/blob/master/LICENSE).

Copyright 2018 NewPowerCoin, Inc. NPW is a trademark maintained by NewPowerCoin, Inc.

