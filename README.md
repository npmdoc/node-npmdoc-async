# npmdoc-async

#### basic api documentation for  [async (v2.3.0)](https://github.com/caolan/async#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-async.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-async) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-async.svg)](https://travis-ci.org/npmdoc/node-npmdoc-async)

#### Higher-order functions and common patterns for asynchronous code

[![NPM](https://nodei.co/npm/async.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/async)

- [https://npmdoc.github.io/node-npmdoc-async/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-async/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-async/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-async/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-async/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-async/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Caolan McMahon"
    },
    "bugs": {
        "url": "https://github.com/caolan/async/issues"
    },
    "dependencies": {
        "lodash": "^4.14.0"
    },
    "description": "Higher-order functions and common patterns for asynchronous code",
    "devDependencies": {
        "babel-cli": "^6.24.0",
        "babel-core": "^6.24.0",
        "babel-plugin-add-module-exports": "^0.2.1",
        "babel-plugin-istanbul": "^2.0.1",
        "babel-plugin-transform-es2015-modules-commonjs": "^6.3.16",
        "babel-preset-es2015": "^6.3.13",
        "babel-preset-es2017": "^6.22.0",
        "babelify": "^7.2.0",
        "benchmark": "^2.1.1",
        "bluebird": "^3.4.6",
        "chai": "^3.1.0",
        "cheerio": "^0.22.0",
        "coveralls": "^2.11.2",
        "es6-promise": "^2.3.0",
        "eslint": "^2.13.1",
        "fs-extra": "^0.26.7",
        "gh-pages-deploy": "^0.4.2",
        "jsdoc": "^3.4.0",
        "karma": "^1.3.0",
        "karma-browserify": "^5.1.0",
        "karma-firefox-launcher": "^1.0.0",
        "karma-mocha": "^1.2.0",
        "karma-mocha-reporter": "^2.2.0",
        "mocha": "^3.1.2",
        "native-promise-only": "^0.8.0-a",
        "nyc": "^7.0.0",
        "recursive-readdir": "^1.3.0",
        "rimraf": "^2.5.0",
        "rollup": "^0.36.3",
        "rollup-plugin-node-resolve": "^2.0.0",
        "rollup-plugin-npm": "^2.0.0",
        "rsvp": "^3.0.18",
        "semver": "^4.3.6",
        "uglify-js": "~2.7.3",
        "vinyl-buffer": "^1.0.0",
        "vinyl-source-stream": "^1.1.0",
        "watchify": "^3.7.0",
        "yargs": "~3.9.1"
    },
    "directories": {},
    "dist": {
        "shasum": "1013d1051047dd320fe24e494d5c66ecaf6147d9",
        "tarball": "https://registry.npmjs.org/async/-/async-2.3.0.tgz"
    },
    "gh-pages-deploy": {
        "staticpath": "docs"
    },
    "homepage": "https://github.com/caolan/async#readme",
    "keywords": [
        "async",
        "callback",
        "module",
        "utility"
    ],
    "license": "MIT",
    "main": "dist/async.js",
    "maintainers": [
        {
            "name": "caolan"
        },
        {
            "name": "beaugunderson"
        },
        {
            "name": "aearly"
        },
        {
            "name": "megawac"
        }
    ],
    "name": "async",
    "nyc": {
        "exclude": [
            "mocha_test"
        ]
    },
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/caolan/async.git"
    },
    "scripts": {
        "coverage": "nyc npm run mocha-node-test -- --grep @nycinvalid --invert",
        "coveralls": "npm run coverage && nyc report --reporter=text-lcov | coveralls",
        "jsdoc": "jsdoc -c ./support/jsdoc/jsdoc.json && node support/jsdoc/jsdoc-fix-html.js",
        "lint": "eslint lib/ mocha_test/ perf/memory.js perf/suites.js perf/benchmark.js support/build/ support/*.js karma.conf.js",
        "mocha-browser-test": "karma start",
        "mocha-node-test": "mocha mocha_test/ --compilers js:babel-core/register",
        "mocha-test": "npm run mocha-node-test && npm run mocha-browser-test",
        "test": "npm run lint && npm run mocha-node-test"
    },
    "version": "2.3.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
