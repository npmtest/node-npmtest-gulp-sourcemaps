# npmtest-gulp-sourcemaps

#### basic test coverage for  [gulp-sourcemaps (v2.6.0)](http://github.com/gulp-sourcemaps/gulp-sourcemaps)  [![npm package](https://img.shields.io/npm/v/npmtest-gulp-sourcemaps.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-gulp-sourcemaps) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-gulp-sourcemaps.svg)](https://travis-ci.org/npmtest/node-npmtest-gulp-sourcemaps)

#### Source map support for Gulp.js

[![NPM](https://nodei.co/npm/gulp-sourcemaps.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/gulp-sourcemaps)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-gulp-sourcemaps/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-gulp-sourcemaps/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-gulp-sourcemaps/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-gulp-sourcemaps/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-gulp-sourcemaps/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-gulp-sourcemaps/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-gulp-sourcemaps/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-gulp-sourcemaps/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-gulp-sourcemaps/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-gulp-sourcemaps/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-gulp-sourcemaps/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-gulp-sourcemaps/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-gulp-sourcemaps/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-gulp-sourcemaps/build/test-report.html](https://npmtest.github.io/node-npmtest-gulp-sourcemaps/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-gulp-sourcemaps/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-gulp-sourcemaps/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-gulp-sourcemaps/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-gulp-sourcemaps/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-gulp-sourcemaps/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-gulp-sourcemaps/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-gulp-sourcemaps/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-gulp-sourcemaps/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Florian Reiterer"
    },
    "bugs": {
        "url": "https://github.com/gulp-sourcemaps/gulp-sourcemaps/issues"
    },
    "dependencies": {
        "@gulp-sourcemaps/identity-map": "1.X",
        "@gulp-sourcemaps/map-sources": "1.X",
        "acorn": "4.X",
        "convert-source-map": "1.X",
        "css": "2.X",
        "debug-fabulous": "0.1.X",
        "detect-newline": "2.X",
        "graceful-fs": "4.X",
        "source-map": "0.X",
        "strip-bom-string": "1.X",
        "through2": "2.X",
        "vinyl": "1.X"
    },
    "description": "Source map support for Gulp.js",
    "devDependencies": {
        "bootstrap": "3.3.7",
        "coveralls": "2.X",
        "faucet": "0.0.X",
        "gulp": "3.X",
        "gulp-concat": "2.X",
        "gulp-if": "2.0.2",
        "gulp-less": "3.3.0",
        "gulp-load-plugins": "1.X",
        "hook-std": "0.2.X",
        "http-server": "0.9.0",
        "istanbul": "0.X",
        "jshint": "2.X",
        "lodash": "4.17.4",
        "mississippi": "^1.3.0",
        "object-assign": "^4.1.0",
        "tape": "4.X",
        "yargs": "6.6.0"
    },
    "directories": {},
    "dist": {
        "shasum": "7ccce899a8a3bfca1593a3348d0fbf41dd3f51e5",
        "tarball": "https://registry.npmjs.org/gulp-sourcemaps/-/gulp-sourcemaps-2.6.0.tgz"
    },
    "engines": {
        "node": ">=4"
    },
    "files": [
        "index.js",
        "src"
    ],
    "gitHead": "65d099a3f318f4f6cfbbf2f087118dd3f68025b7",
    "homepage": "http://github.com/gulp-sourcemaps/gulp-sourcemaps",
    "keywords": [
        "gulpplugin",
        "gulp",
        "source maps",
        "sourcemaps"
    ],
    "license": "ISC",
    "main": "index.js",
    "maintainers": [
        {
            "name": "floridoo"
        },
        {
            "name": "nmccready"
        },
        {
            "name": "phated"
        }
    ],
    "name": "gulp-sourcemaps",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/gulp-sourcemaps/gulp-sourcemaps.git"
    },
    "scripts": {
        "cover": "istanbul cover --dir reports/coverage tape \"test/*.js\"",
        "coveralls": "istanbul cover tape \"test/*.js\" --report lcovonly && cat ./coverage/lcov.info | coveralls && rm -rf ./coverage",
        "lint": "jshint ./src/**/*.js test/*.js",
        "serve": "http-server",
        "tap": "tape test/*.js",
        "test": "npm run lint && faucet test/*.js $@",
        "test:int": "rm -rf ./tmp && tape ./test/integration.js"
    },
    "version": "2.6.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
