# api-documentation for  [async (v2.1.5)](https://github.com/caolan/async#readme)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-async.svg)](https://travis-ci.org/npmdoc/node-npmdoc-async)
#### Higher-order functions and common patterns for asynchronous code

[![NPM](https://nodei.co/npm/async.png?downloads=true)](https://www.npmjs.com/package/async)

# html version

- [https://npmdoc.github.io/node-npmdoc-async/build..beta..travis-ci.org/apidoc.html](https://npmdoc.github.io/node-npmdoc-async/build..beta..travis-ci.org/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-async/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-async_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-async/build..beta..travis-ci.org/apidoc.html)

# package listing

![package-listing](https://npmdoc.github.io/node-npmdoc-async/build/screen-capture.npmPackageListing.svg)



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
        "babel-cli": "^6.16.0",
        "babel-core": "^6.3.26",
        "babel-plugin-add-module-exports": "^0.2.1",
        "babel-plugin-istanbul": "^2.0.1",
        "babel-plugin-transform-es2015-modules-commonjs": "^6.3.16",
        "babel-preset-es2015": "^6.3.13",
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
        "shasum": "e587c68580994ac67fc56ff86d3ac56bdbe810bc",
        "tarball": "https://registry.npmjs.org/async/-/async-2.1.5.tgz"
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
            "name": "caolan",
            "email": "caolan.mcmahon@gmail.com"
        },
        {
            "name": "beaugunderson",
            "email": "beau@beaugunderson.com"
        },
        {
            "name": "aearly",
            "email": "alexander.early@gmail.com"
        },
        {
            "name": "megawac",
            "email": "megawac@gmail.com"
        }
    ],
    "name": "async",
    "nyc": {
        "exclude": [
            "mocha_test"
        ]
    },
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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
    "version": "2.1.5"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module async](#apidoc.module.async)
1.  [function <span class="apidocSignatureSpan">async.</span>all (obj, iteratee, callback)](#apidoc.element.async.all)
1.  [function <span class="apidocSignatureSpan">async.</span>allLimit (obj, limit, iteratee, callback)](#apidoc.element.async.allLimit)
1.  [function <span class="apidocSignatureSpan">async.</span>allSeries (iterable, iteratee, callback)](#apidoc.element.async.allSeries)
1.  [function <span class="apidocSignatureSpan">async.</span>any (obj, iteratee, callback)](#apidoc.element.async.any)
1.  [function <span class="apidocSignatureSpan">async.</span>anyLimit (obj, limit, iteratee, callback)](#apidoc.element.async.anyLimit)
1.  [function <span class="apidocSignatureSpan">async.</span>anySeries (iterable, iteratee, callback)](#apidoc.element.async.anySeries)
1.  [function <span class="apidocSignatureSpan">async.</span>apply ()](#apidoc.element.async.apply)
1.  [function <span class="apidocSignatureSpan">async.</span>applyEach ()](#apidoc.element.async.applyEach)
1.  [function <span class="apidocSignatureSpan">async.</span>applyEachSeries ()](#apidoc.element.async.applyEachSeries)
1.  [function <span class="apidocSignatureSpan">async.</span>asyncify (func)](#apidoc.element.async.asyncify)
1.  [function <span class="apidocSignatureSpan">async.</span>auto (tasks, concurrency, callback)](#apidoc.element.async.auto)
1.  [function <span class="apidocSignatureSpan">async.</span>autoInject (tasks, callback)](#apidoc.element.async.autoInject)
1.  [function <span class="apidocSignatureSpan">async.</span>cargo (worker, payload)](#apidoc.element.async.cargo)
1.  [function <span class="apidocSignatureSpan">async.</span>compose ()](#apidoc.element.async.compose)
1.  [function <span class="apidocSignatureSpan">async.</span>concat (obj, iteratee, callback)](#apidoc.element.async.concat)
1.  [function <span class="apidocSignatureSpan">async.</span>concatSeries (obj, iteratee, callback)](#apidoc.element.async.concatSeries)
1.  [function <span class="apidocSignatureSpan">async.</span>constant ()](#apidoc.element.async.constant)
1.  [function <span class="apidocSignatureSpan">async.</span>detect (obj, iteratee, callback)](#apidoc.element.async.detect)
1.  [function <span class="apidocSignatureSpan">async.</span>detectLimit (obj, limit, iteratee, callback)](#apidoc.element.async.detectLimit)
1.  [function <span class="apidocSignatureSpan">async.</span>detectSeries (iterable, iteratee, callback)](#apidoc.element.async.detectSeries)
1.  [function <span class="apidocSignatureSpan">async.</span>dir ()](#apidoc.element.async.dir)
1.  [function <span class="apidocSignatureSpan">async.</span>doDuring (fn, test, callback)](#apidoc.element.async.doDuring)
1.  [function <span class="apidocSignatureSpan">async.</span>doUntil (fn, test, callback)](#apidoc.element.async.doUntil)
1.  [function <span class="apidocSignatureSpan">async.</span>doWhilst (iteratee, test, callback)](#apidoc.element.async.doWhilst)
1.  [function <span class="apidocSignatureSpan">async.</span>during (test, fn, callback)](#apidoc.element.async.during)
1.  [function <span class="apidocSignatureSpan">async.</span>each (coll, iteratee, callback)](#apidoc.element.async.each)
1.  [function <span class="apidocSignatureSpan">async.</span>eachLimit (coll, limit, iteratee, callback)](#apidoc.element.async.eachLimit)
1.  [function <span class="apidocSignatureSpan">async.</span>eachOf (coll, iteratee, callback)](#apidoc.element.async.eachOf)
1.  [function <span class="apidocSignatureSpan">async.</span>eachOfLimit (coll, limit, iteratee, callback)](#apidoc.element.async.eachOfLimit)
1.  [function <span class="apidocSignatureSpan">async.</span>eachOfSeries (iterable, iteratee, callback)](#apidoc.element.async.eachOfSeries)
1.  [function <span class="apidocSignatureSpan">async.</span>eachSeries (iterable, iteratee, callback)](#apidoc.element.async.eachSeries)
1.  [function <span class="apidocSignatureSpan">async.</span>ensureAsync (fn)](#apidoc.element.async.ensureAsync)
1.  [function <span class="apidocSignatureSpan">async.</span>every (obj, iteratee, callback)](#apidoc.element.async.every)
1.  [function <span class="apidocSignatureSpan">async.</span>everyLimit (obj, limit, iteratee, callback)](#apidoc.element.async.everyLimit)
1.  [function <span class="apidocSignatureSpan">async.</span>everySeries (iterable, iteratee, callback)](#apidoc.element.async.everySeries)
1.  [function <span class="apidocSignatureSpan">async.</span>filter (obj, iteratee, callback)](#apidoc.element.async.filter)
1.  [function <span class="apidocSignatureSpan">async.</span>filterLimit (obj, limit, iteratee, callback)](#apidoc.element.async.filterLimit)
1.  [function <span class="apidocSignatureSpan">async.</span>filterSeries (iterable, iteratee, callback)](#apidoc.element.async.filterSeries)
1.  [function <span class="apidocSignatureSpan">async.</span>find (obj, iteratee, callback)](#apidoc.element.async.find)
1.  [function <span class="apidocSignatureSpan">async.</span>findLimit (obj, limit, iteratee, callback)](#apidoc.element.async.findLimit)
1.  [function <span class="apidocSignatureSpan">async.</span>findSeries (iterable, iteratee, callback)](#apidoc.element.async.findSeries)
1.  [function <span class="apidocSignatureSpan">async.</span>foldl (coll, memo, iteratee, callback)](#apidoc.element.async.foldl)
1.  [function <span class="apidocSignatureSpan">async.</span>foldr (array, memo, iteratee, callback)](#apidoc.element.async.foldr)
1.  [function <span class="apidocSignatureSpan">async.</span>forEach (coll, iteratee, callback)](#apidoc.element.async.forEach)
1.  [function <span class="apidocSignatureSpan">async.</span>forEachLimit (coll, limit, iteratee, callback)](#apidoc.element.async.forEachLimit)
1.  [function <span class="apidocSignatureSpan">async.</span>forEachOf (coll, iteratee, callback)](#apidoc.element.async.forEachOf)
1.  [function <span class="apidocSignatureSpan">async.</span>forEachOfLimit (coll, limit, iteratee, callback)](#apidoc.element.async.forEachOfLimit)
1.  [function <span class="apidocSignatureSpan">async.</span>forEachOfSeries (iterable, iteratee, callback)](#apidoc.element.async.forEachOfSeries)
1.  [function <span class="apidocSignatureSpan">async.</span>forEachSeries (iterable, iteratee, callback)](#apidoc.element.async.forEachSeries)
1.  [function <span class="apidocSignatureSpan">async.</span>forever (fn, errback)](#apidoc.element.async.forever)
1.  [function <span class="apidocSignatureSpan">async.</span>inject (coll, memo, iteratee, callback)](#apidoc.element.async.inject)
1.  [function <span class="apidocSignatureSpan">async.</span>log ()](#apidoc.element.async.log)
1.  [function <span class="apidocSignatureSpan">async.</span>map (obj, iteratee, callback)](#apidoc.element.async.map)
1.  [function <span class="apidocSignatureSpan">async.</span>mapLimit (obj, limit, iteratee, callback)](#apidoc.element.async.mapLimit)
1.  [function <span class="apidocSignatureSpan">async.</span>mapSeries (iterable, iteratee, callback)](#apidoc.element.async.mapSeries)
1.  [function <span class="apidocSignatureSpan">async.</span>mapValues (iterable, iteratee, callback)](#apidoc.element.async.mapValues)
1.  [function <span class="apidocSignatureSpan">async.</span>mapValuesLimit (obj, limit, iteratee, callback)](#apidoc.element.async.mapValuesLimit)
1.  [function <span class="apidocSignatureSpan">async.</span>mapValuesSeries (iterable, iteratee, callback)](#apidoc.element.async.mapValuesSeries)
1.  [function <span class="apidocSignatureSpan">async.</span>memoize (fn, hasher)](#apidoc.element.async.memoize)
1.  [function <span class="apidocSignatureSpan">async.</span>nextTick ()](#apidoc.element.async.nextTick)
1.  [function <span class="apidocSignatureSpan">async.</span>parallel (tasks, callback)](#apidoc.element.async.parallel)
1.  [function <span class="apidocSignatureSpan">async.</span>parallelLimit (tasks, limit, callback)](#apidoc.element.async.parallelLimit)
1.  [function <span class="apidocSignatureSpan">async.</span>priorityQueue (worker, concurrency)](#apidoc.element.async.priorityQueue)
1.  [function <span class="apidocSignatureSpan">async.</span>queue (worker, concurrency)](#apidoc.element.async.queue)
1.  [function <span class="apidocSignatureSpan">async.</span>race (tasks, callback)](#apidoc.element.async.race)
1.  [function <span class="apidocSignatureSpan">async.</span>reduce (coll, memo, iteratee, callback)](#apidoc.element.async.reduce)
1.  [function <span class="apidocSignatureSpan">async.</span>reduceRight (array, memo, iteratee, callback)](#apidoc.element.async.reduceRight)
1.  [function <span class="apidocSignatureSpan">async.</span>reflect (fn)](#apidoc.element.async.reflect)
1.  [function <span class="apidocSignatureSpan">async.</span>reflectAll (tasks)](#apidoc.element.async.reflectAll)
1.  [function <span class="apidocSignatureSpan">async.</span>reject (obj, iteratee, callback)](#apidoc.element.async.reject)
1.  [function <span class="apidocSignatureSpan">async.</span>rejectLimit (obj, limit, iteratee, callback)](#apidoc.element.async.rejectLimit)
1.  [function <span class="apidocSignatureSpan">async.</span>rejectSeries (iterable, iteratee, callback)](#apidoc.element.async.rejectSeries)
1.  [function <span class="apidocSignatureSpan">async.</span>retry (opts, task, callback)](#apidoc.element.async.retry)
1.  [function <span class="apidocSignatureSpan">async.</span>retryable (opts, task)](#apidoc.element.async.retryable)
1.  [function <span class="apidocSignatureSpan">async.</span>select (obj, iteratee, callback)](#apidoc.element.async.select)
1.  [function <span class="apidocSignatureSpan">async.</span>selectLimit (obj, limit, iteratee, callback)](#apidoc.element.async.selectLimit)
1.  [function <span class="apidocSignatureSpan">async.</span>selectSeries (iterable, iteratee, callback)](#apidoc.element.async.selectSeries)
1.  [function <span class="apidocSignatureSpan">async.</span>seq ()](#apidoc.element.async.seq)
1.  [function <span class="apidocSignatureSpan">async.</span>series (tasks, callback)](#apidoc.element.async.series)
1.  [function <span class="apidocSignatureSpan">async.</span>setImmediate ()](#apidoc.element.async.setImmediate)
1.  [function <span class="apidocSignatureSpan">async.</span>some (obj, iteratee, callback)](#apidoc.element.async.some)
1.  [function <span class="apidocSignatureSpan">async.</span>someLimit (obj, limit, iteratee, callback)](#apidoc.element.async.someLimit)
1.  [function <span class="apidocSignatureSpan">async.</span>someSeries (iterable, iteratee, callback)](#apidoc.element.async.someSeries)
1.  [function <span class="apidocSignatureSpan">async.</span>sortBy (coll, iteratee, callback)](#apidoc.element.async.sortBy)
1.  [function <span class="apidocSignatureSpan">async.</span>timeout (asyncFn, milliseconds, info)](#apidoc.element.async.timeout)
1.  [function <span class="apidocSignatureSpan">async.</span>times (iterable, iteratee, callback)](#apidoc.element.async.times)
1.  [function <span class="apidocSignatureSpan">async.</span>timesLimit (count, limit, iteratee, callback)](#apidoc.element.async.timesLimit)
1.  [function <span class="apidocSignatureSpan">async.</span>timesSeries (iterable, iteratee, callback)](#apidoc.element.async.timesSeries)
1.  [function <span class="apidocSignatureSpan">async.</span>transform (coll, accumulator, iteratee, callback)](#apidoc.element.async.transform)
1.  [function <span class="apidocSignatureSpan">async.</span>unmemoize (fn)](#apidoc.element.async.unmemoize)
1.  [function <span class="apidocSignatureSpan">async.</span>until (test, fn, callback)](#apidoc.element.async.until)
1.  [function <span class="apidocSignatureSpan">async.</span>waterfall (tasks, callback)](#apidoc.element.async.waterfall)
1.  [function <span class="apidocSignatureSpan">async.</span>whilst (test, iteratee, callback)](#apidoc.element.async.whilst)
1.  [function <span class="apidocSignatureSpan">async.</span>wrapSync (func)](#apidoc.element.async.wrapSync)
1.  object <span class="apidocSignatureSpan">async.</span>default

#### [module async.default](#apidoc.module.async.default)
1.  [function <span class="apidocSignatureSpan">async.default.</span>all (obj, iteratee, callback)](#apidoc.element.async.default.all)
1.  [function <span class="apidocSignatureSpan">async.default.</span>any (obj, iteratee, callback)](#apidoc.element.async.default.any)
1.  [function <span class="apidocSignatureSpan">async.default.</span>apply ()](#apidoc.element.async.default.apply)
1.  [function <span class="apidocSignatureSpan">async.default.</span>applyEach ()](#apidoc.element.async.default.applyEach)
1.  [function <span class="apidocSignatureSpan">async.default.</span>applyEachSeries ()](#apidoc.element.async.default.applyEachSeries)
1.  [function <span class="apidocSignatureSpan">async.default.</span>asyncify (func)](#apidoc.element.async.default.asyncify)
1.  [function <span class="apidocSignatureSpan">async.default.</span>auto (tasks, concurrency, callback)](#apidoc.element.async.default.auto)
1.  [function <span class="apidocSignatureSpan">async.default.</span>autoInject (tasks, callback)](#apidoc.element.async.default.autoInject)
1.  [function <span class="apidocSignatureSpan">async.default.</span>cargo (worker, payload)](#apidoc.element.async.default.cargo)
1.  [function <span class="apidocSignatureSpan">async.default.</span>compose ()](#apidoc.element.async.default.compose)
1.  [function <span class="apidocSignatureSpan">async.default.</span>concat (obj, iteratee, callback)](#apidoc.element.async.default.concat)
1.  [function <span class="apidocSignatureSpan">async.default.</span>concatSeries (obj, iteratee, callback)](#apidoc.element.async.default.concatSeries)
1.  [function <span class="apidocSignatureSpan">async.default.</span>constant ()](#apidoc.element.async.default.constant)
1.  [function <span class="apidocSignatureSpan">async.default.</span>detect (obj, iteratee, callback)](#apidoc.element.async.default.detect)
1.  [function <span class="apidocSignatureSpan">async.default.</span>detectLimit (obj, limit, iteratee, callback)](#apidoc.element.async.default.detectLimit)
1.  [function <span class="apidocSignatureSpan">async.default.</span>detectSeries (iterable, iteratee, callback)](#apidoc.element.async.default.detectSeries)
1.  [function <span class="apidocSignatureSpan">async.default.</span>dir ()](#apidoc.element.async.default.dir)
1.  [function <span class="apidocSignatureSpan">async.default.</span>doDuring (fn, test, callback)](#apidoc.element.async.default.doDuring)
1.  [function <span class="apidocSignatureSpan">async.default.</span>doUntil (fn, test, callback)](#apidoc.element.async.default.doUntil)
1.  [function <span class="apidocSignatureSpan">async.default.</span>doWhilst (iteratee, test, callback)](#apidoc.element.async.default.doWhilst)
1.  [function <span class="apidocSignatureSpan">async.default.</span>during (test, fn, callback)](#apidoc.element.async.default.during)
1.  [function <span class="apidocSignatureSpan">async.default.</span>each (coll, iteratee, callback)](#apidoc.element.async.default.each)
1.  [function <span class="apidocSignatureSpan">async.default.</span>eachLimit (coll, limit, iteratee, callback)](#apidoc.element.async.default.eachLimit)
1.  [function <span class="apidocSignatureSpan">async.default.</span>eachOf (coll, iteratee, callback)](#apidoc.element.async.default.eachOf)
1.  [function <span class="apidocSignatureSpan">async.default.</span>eachOfLimit (coll, limit, iteratee, callback)](#apidoc.element.async.default.eachOfLimit)
1.  [function <span class="apidocSignatureSpan">async.default.</span>eachOfSeries (iterable, iteratee, callback)](#apidoc.element.async.default.eachOfSeries)
1.  [function <span class="apidocSignatureSpan">async.default.</span>eachSeries (iterable, iteratee, callback)](#apidoc.element.async.default.eachSeries)
1.  [function <span class="apidocSignatureSpan">async.default.</span>ensureAsync (fn)](#apidoc.element.async.default.ensureAsync)
1.  [function <span class="apidocSignatureSpan">async.default.</span>every (obj, iteratee, callback)](#apidoc.element.async.default.every)
1.  [function <span class="apidocSignatureSpan">async.default.</span>everyLimit (obj, limit, iteratee, callback)](#apidoc.element.async.default.everyLimit)
1.  [function <span class="apidocSignatureSpan">async.default.</span>everySeries (iterable, iteratee, callback)](#apidoc.element.async.default.everySeries)
1.  [function <span class="apidocSignatureSpan">async.default.</span>filter (obj, iteratee, callback)](#apidoc.element.async.default.filter)
1.  [function <span class="apidocSignatureSpan">async.default.</span>filterLimit (obj, limit, iteratee, callback)](#apidoc.element.async.default.filterLimit)
1.  [function <span class="apidocSignatureSpan">async.default.</span>filterSeries (iterable, iteratee, callback)](#apidoc.element.async.default.filterSeries)
1.  [function <span class="apidocSignatureSpan">async.default.</span>foldl (coll, memo, iteratee, callback)](#apidoc.element.async.default.foldl)
1.  [function <span class="apidocSignatureSpan">async.default.</span>foldr (array, memo, iteratee, callback)](#apidoc.element.async.default.foldr)
1.  [function <span class="apidocSignatureSpan">async.default.</span>forEach (coll, iteratee, callback)](#apidoc.element.async.default.forEach)
1.  [function <span class="apidocSignatureSpan">async.default.</span>forEachLimit (coll, limit, iteratee, callback)](#apidoc.element.async.default.forEachLimit)
1.  [function <span class="apidocSignatureSpan">async.default.</span>forEachOf (coll, iteratee, callback)](#apidoc.element.async.default.forEachOf)
1.  [function <span class="apidocSignatureSpan">async.default.</span>forEachOfLimit (coll, limit, iteratee, callback)](#apidoc.element.async.default.forEachOfLimit)
1.  [function <span class="apidocSignatureSpan">async.default.</span>forEachOfSeries (iterable, iteratee, callback)](#apidoc.element.async.default.forEachOfSeries)
1.  [function <span class="apidocSignatureSpan">async.default.</span>forEachSeries (iterable, iteratee, callback)](#apidoc.element.async.default.forEachSeries)
1.  [function <span class="apidocSignatureSpan">async.default.</span>forever (fn, errback)](#apidoc.element.async.default.forever)
1.  [function <span class="apidocSignatureSpan">async.default.</span>inject (coll, memo, iteratee, callback)](#apidoc.element.async.default.inject)
1.  [function <span class="apidocSignatureSpan">async.default.</span>log ()](#apidoc.element.async.default.log)
1.  [function <span class="apidocSignatureSpan">async.default.</span>map (obj, iteratee, callback)](#apidoc.element.async.default.map)
1.  [function <span class="apidocSignatureSpan">async.default.</span>mapLimit (obj, limit, iteratee, callback)](#apidoc.element.async.default.mapLimit)
1.  [function <span class="apidocSignatureSpan">async.default.</span>mapSeries (iterable, iteratee, callback)](#apidoc.element.async.default.mapSeries)
1.  [function <span class="apidocSignatureSpan">async.default.</span>mapValues (iterable, iteratee, callback)](#apidoc.element.async.default.mapValues)
1.  [function <span class="apidocSignatureSpan">async.default.</span>mapValuesLimit (obj, limit, iteratee, callback)](#apidoc.element.async.default.mapValuesLimit)
1.  [function <span class="apidocSignatureSpan">async.default.</span>mapValuesSeries (iterable, iteratee, callback)](#apidoc.element.async.default.mapValuesSeries)
1.  [function <span class="apidocSignatureSpan">async.default.</span>memoize (fn, hasher)](#apidoc.element.async.default.memoize)
1.  [function <span class="apidocSignatureSpan">async.default.</span>nextTick ()](#apidoc.element.async.default.nextTick)
1.  [function <span class="apidocSignatureSpan">async.default.</span>parallel (tasks, callback)](#apidoc.element.async.default.parallel)
1.  [function <span class="apidocSignatureSpan">async.default.</span>parallelLimit (tasks, limit, callback)](#apidoc.element.async.default.parallelLimit)
1.  [function <span class="apidocSignatureSpan">async.default.</span>priorityQueue (worker, concurrency)](#apidoc.element.async.default.priorityQueue)
1.  [function <span class="apidocSignatureSpan">async.default.</span>queue (worker, concurrency)](#apidoc.element.async.default.queue)
1.  [function <span class="apidocSignatureSpan">async.default.</span>race (tasks, callback)](#apidoc.element.async.default.race)
1.  [function <span class="apidocSignatureSpan">async.default.</span>reduce (coll, memo, iteratee, callback)](#apidoc.element.async.default.reduce)
1.  [function <span class="apidocSignatureSpan">async.default.</span>reduceRight (array, memo, iteratee, callback)](#apidoc.element.async.default.reduceRight)
1.  [function <span class="apidocSignatureSpan">async.default.</span>reflect (fn)](#apidoc.element.async.default.reflect)
1.  [function <span class="apidocSignatureSpan">async.default.</span>reflectAll (tasks)](#apidoc.element.async.default.reflectAll)
1.  [function <span class="apidocSignatureSpan">async.default.</span>reject (obj, iteratee, callback)](#apidoc.element.async.default.reject)
1.  [function <span class="apidocSignatureSpan">async.default.</span>rejectLimit (obj, limit, iteratee, callback)](#apidoc.element.async.default.rejectLimit)
1.  [function <span class="apidocSignatureSpan">async.default.</span>rejectSeries (iterable, iteratee, callback)](#apidoc.element.async.default.rejectSeries)
1.  [function <span class="apidocSignatureSpan">async.default.</span>retry (opts, task, callback)](#apidoc.element.async.default.retry)
1.  [function <span class="apidocSignatureSpan">async.default.</span>retryable (opts, task)](#apidoc.element.async.default.retryable)
1.  [function <span class="apidocSignatureSpan">async.default.</span>select (obj, iteratee, callback)](#apidoc.element.async.default.select)
1.  [function <span class="apidocSignatureSpan">async.default.</span>selectLimit (obj, limit, iteratee, callback)](#apidoc.element.async.default.selectLimit)
1.  [function <span class="apidocSignatureSpan">async.default.</span>selectSeries (iterable, iteratee, callback)](#apidoc.element.async.default.selectSeries)
1.  [function <span class="apidocSignatureSpan">async.default.</span>seq ()](#apidoc.element.async.default.seq)
1.  [function <span class="apidocSignatureSpan">async.default.</span>series (tasks, callback)](#apidoc.element.async.default.series)
1.  [function <span class="apidocSignatureSpan">async.default.</span>setImmediate ()](#apidoc.element.async.default.setImmediate)
1.  [function <span class="apidocSignatureSpan">async.default.</span>some (obj, iteratee, callback)](#apidoc.element.async.default.some)
1.  [function <span class="apidocSignatureSpan">async.default.</span>someLimit (obj, limit, iteratee, callback)](#apidoc.element.async.default.someLimit)
1.  [function <span class="apidocSignatureSpan">async.default.</span>someSeries (iterable, iteratee, callback)](#apidoc.element.async.default.someSeries)
1.  [function <span class="apidocSignatureSpan">async.default.</span>sortBy (coll, iteratee, callback)](#apidoc.element.async.default.sortBy)
1.  [function <span class="apidocSignatureSpan">async.default.</span>timeout (asyncFn, milliseconds, info)](#apidoc.element.async.default.timeout)
1.  [function <span class="apidocSignatureSpan">async.default.</span>times (iterable, iteratee, callback)](#apidoc.element.async.default.times)
1.  [function <span class="apidocSignatureSpan">async.default.</span>timesLimit (count, limit, iteratee, callback)](#apidoc.element.async.default.timesLimit)
1.  [function <span class="apidocSignatureSpan">async.default.</span>timesSeries (iterable, iteratee, callback)](#apidoc.element.async.default.timesSeries)
1.  [function <span class="apidocSignatureSpan">async.default.</span>transform (coll, accumulator, iteratee, callback)](#apidoc.element.async.default.transform)
1.  [function <span class="apidocSignatureSpan">async.default.</span>unmemoize (fn)](#apidoc.element.async.default.unmemoize)
1.  [function <span class="apidocSignatureSpan">async.default.</span>until (test, fn, callback)](#apidoc.element.async.default.until)
1.  [function <span class="apidocSignatureSpan">async.default.</span>waterfall (tasks, callback)](#apidoc.element.async.default.waterfall)
1.  [function <span class="apidocSignatureSpan">async.default.</span>whilst (test, iteratee, callback)](#apidoc.element.async.default.whilst)
1.  [function <span class="apidocSignatureSpan">async.default.</span>wrapSync (func)](#apidoc.element.async.default.wrapSync)



# <a name="apidoc.module.async"></a>[module async](#apidoc.module.async)

#### <a name="apidoc.element.async.all"></a>[function <span class="apidocSignatureSpan">async.</span>all (obj, iteratee, callback)](#apidoc.element.async.all)
- description and source-code
```javascript
all = function (obj, iteratee, callback) {
    return fn(eachOf, obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.allLimit"></a>[function <span class="apidocSignatureSpan">async.</span>allLimit (obj, limit, iteratee, callback)](#apidoc.element.async.allLimit)
- description and source-code
```javascript
allLimit = function (obj, limit, iteratee, callback) {
    return fn(_eachOfLimit(limit), obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.allSeries"></a>[function <span class="apidocSignatureSpan">async.</span>allSeries (iterable, iteratee, callback)](#apidoc.element.async.allSeries)
- description and source-code
```javascript
allSeries = function (iterable, iteratee, callback) {
    return fn(iterable, limit, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.any"></a>[function <span class="apidocSignatureSpan">async.</span>any (obj, iteratee, callback)](#apidoc.element.async.any)
- description and source-code
```javascript
any = function (obj, iteratee, callback) {
    return fn(eachOf, obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.anyLimit"></a>[function <span class="apidocSignatureSpan">async.</span>anyLimit (obj, limit, iteratee, callback)](#apidoc.element.async.anyLimit)
- description and source-code
```javascript
anyLimit = function (obj, limit, iteratee, callback) {
    return fn(_eachOfLimit(limit), obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.anySeries"></a>[function <span class="apidocSignatureSpan">async.</span>anySeries (iterable, iteratee, callback)](#apidoc.element.async.anySeries)
- description and source-code
```javascript
anySeries = function (iterable, iteratee, callback) {
    return fn(iterable, limit, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.apply"></a>[function <span class="apidocSignatureSpan">async.</span>apply ()](#apidoc.element.async.apply)
- description and source-code
```javascript
apply = function () {
  var args = arguments,
      index = -1,
      length = nativeMax(args.length - start, 0),
      array = Array(length);

  while (++index < length) {
    array[index] = args[start + index];
  }
  index = -1;
  var otherArgs = Array(start + 1);
  while (++index < start) {
    otherArgs[index] = args[index];
  }
  otherArgs[start] = transform(array);
  return apply(func, this, otherArgs);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.applyEach"></a>[function <span class="apidocSignatureSpan">async.</span>applyEach ()](#apidoc.element.async.applyEach)
- description and source-code
```javascript
applyEach = function () {
  var args = arguments,
      index = -1,
      length = nativeMax(args.length - start, 0),
      array = Array(length);

  while (++index < length) {
    array[index] = args[start + index];
  }
  index = -1;
  var otherArgs = Array(start + 1);
  while (++index < start) {
    otherArgs[index] = args[index];
  }
  otherArgs[start] = transform(array);
  return apply(func, this, otherArgs);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.applyEachSeries"></a>[function <span class="apidocSignatureSpan">async.</span>applyEachSeries ()](#apidoc.element.async.applyEachSeries)
- description and source-code
```javascript
applyEachSeries = function () {
  var args = arguments,
      index = -1,
      length = nativeMax(args.length - start, 0),
      array = Array(length);

  while (++index < length) {
    array[index] = args[start + index];
  }
  index = -1;
  var otherArgs = Array(start + 1);
  while (++index < start) {
    otherArgs[index] = args[index];
  }
  otherArgs[start] = transform(array);
  return apply(func, this, otherArgs);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.asyncify"></a>[function <span class="apidocSignatureSpan">async.</span>asyncify (func)](#apidoc.element.async.asyncify)
- description and source-code
```javascript
function asyncify(func) {
    return initialParams(function (args, callback) {
        var result;
        try {
            result = func.apply(this, args);
        } catch (e) {
            return callback(e);
        }
        // if result is Promise object
        if (isObject(result) && typeof result.then === 'function') {
            result.then(function (value) {
                callback(null, value);
            }, function (err) {
                callback(err.message ? err : new Error(err));
            });
        } else {
            callback(null, result);
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.auto"></a>[function <span class="apidocSignatureSpan">async.</span>auto (tasks, concurrency, callback)](#apidoc.element.async.auto)
- description and source-code
```javascript
auto = function (tasks, concurrency, callback) {
    if (typeof concurrency === 'function') {
        // concurrency is optional, shift the args.
        callback = concurrency;
        concurrency = null;
    }
    callback = once(callback || noop);
    var keys$$1 = keys(tasks);
    var numTasks = keys$$1.length;
    if (!numTasks) {
        return callback(null);
    }
    if (!concurrency) {
        concurrency = numTasks;
    }

    var results = {};
    var runningTasks = 0;
    var hasError = false;

    var listeners = Object.create(null);

    var readyTasks = [];

    // for cycle detection:
    var readyToCheck = []; // tasks that have been identified as reachable
    // without the possibility of returning to an ancestor task
    var uncheckedDependencies = {};

    baseForOwn(tasks, function (task, key) {
        if (!isArray(task)) {
            // no dependencies
            enqueueTask(key, [task]);
            readyToCheck.push(key);
            return;
        }

        var dependencies = task.slice(0, task.length - 1);
        var remainingDependencies = dependencies.length;
        if (remainingDependencies === 0) {
            enqueueTask(key, task);
            readyToCheck.push(key);
            return;
        }
        uncheckedDependencies[key] = remainingDependencies;

        arrayEach(dependencies, function (dependencyName) {
            if (!tasks[dependencyName]) {
                throw new Error('async.auto task '' + key + '' has a non-existent dependency '' + dependencyName + '' in ' + dependencies
.join(', '));
            }
            addListener(dependencyName, function () {
                remainingDependencies--;
                if (remainingDependencies === 0) {
                    enqueueTask(key, task);
                }
            });
        });
    });

    checkForDeadlocks();
    processQueue();

    function enqueueTask(key, task) {
        readyTasks.push(function () {
            runTask(key, task);
        });
    }

    function processQueue() {
        if (readyTasks.length === 0 && runningTasks === 0) {
            return callback(null, results);
        }
        while (readyTasks.length && runningTasks < concurrency) {
            var run = readyTasks.shift();
            run();
        }
    }

    function addListener(taskName, fn) {
        var taskListeners = listeners[taskName];
        if (!taskListeners) {
            taskListeners = listeners[taskName] = [];
        }

        taskListeners.push(fn);
    }

    function taskComplete(taskName) {
        var taskListeners = listeners[taskName] || [];
        arrayEach(taskListeners, function (fn) {
            fn();
        });
        processQueue();
    }

    function runTask(key, task) {
        if (hasError) return;

        var taskCallback = onlyOnce(rest(function (err, args) {
            runningTasks--;
            if (args.length <= 1) {
                args = args[0];
            }
            if (err) {
                var safeResults = {};
                baseForOwn(results, function (val, rkey) {
                    safeResults[rkey] = val;
                });
                safeResults[key] = args;
                hasError = true;
                listeners = Object.create(null);

                callback(err, safeResults);
            } else {
                results[key] = args;
                taskComplete(key);
            }
        }));

        runningTasks++;
        var taskFn = task[task.length - 1];
        if (task.length > 1) {
            taskFn(results, taskCallback);
        } else {
            taskFn(taskCallback);
        }
    }

    function checkForDeadlocks() {
        // Kahn's algorithm
        // https://en.wikipedia.org/wiki/Topological_sorting#Kahn.27s_algorithm
        // http://connalle.blogspot.com/2013/10/topological-sortingkahn-algorithm.html
        var currentTask;
        var counter = 0;
        while (readyToCheck.length) {
            currentTask = readyToCheck.pop();
            counter++;
            arrayEach(getDependents(currentTask), function (dependent) { ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.autoInject"></a>[function <span class="apidocSignatureSpan">async.</span>autoInject (tasks, callback)](#apidoc.element.async.autoInject)
- description and source-code
```javascript
function autoInject(tasks, callback) {
    var newTasks = {};

    baseForOwn(tasks, function (taskFn, key) {
        var params;

        if (isArray(taskFn)) {
            params = taskFn.slice(0, -1);
            taskFn = taskFn[taskFn.length - 1];

            newTasks[key] = params.concat(params.length > 0 ? newTask : taskFn);
        } else if (taskFn.length === 1) {
            // no dependencies, use the function as-is
            newTasks[key] = taskFn;
        } else {
            params = parseParams(taskFn);
            if (taskFn.length === 0 && params.length === 0) {
                throw new Error("autoInject task functions require explicit parameters.");
            }

            params.pop();

            newTasks[key] = params.concat(newTask);
        }

        function newTask(results, taskCb) {
            var newArgs = arrayMap(params, function (name) {
                return results[name];
            });
            newArgs.push(taskCb);
            taskFn.apply(null, newArgs);
        }
    });

    auto(newTasks, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.cargo"></a>[function <span class="apidocSignatureSpan">async.</span>cargo (worker, payload)](#apidoc.element.async.cargo)
- description and source-code
```javascript
function cargo(worker, payload) {
  return queue(worker, 1, payload);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.compose"></a>[function <span class="apidocSignatureSpan">async.</span>compose ()](#apidoc.element.async.compose)
- description and source-code
```javascript
compose = function () {
  var args = arguments,
      index = -1,
      length = nativeMax(args.length - start, 0),
      array = Array(length);

  while (++index < length) {
    array[index] = args[start + index];
  }
  index = -1;
  var otherArgs = Array(start + 1);
  while (++index < start) {
    otherArgs[index] = args[index];
  }
  otherArgs[start] = transform(array);
  return apply(func, this, otherArgs);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.concat"></a>[function <span class="apidocSignatureSpan">async.</span>concat (obj, iteratee, callback)](#apidoc.element.async.concat)
- description and source-code
```javascript
concat = function (obj, iteratee, callback) {
    return fn(eachOf, obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.concatSeries"></a>[function <span class="apidocSignatureSpan">async.</span>concatSeries (obj, iteratee, callback)](#apidoc.element.async.concatSeries)
- description and source-code
```javascript
concatSeries = function (obj, iteratee, callback) {
    return fn(eachOfSeries, obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.constant"></a>[function <span class="apidocSignatureSpan">async.</span>constant ()](#apidoc.element.async.constant)
- description and source-code
```javascript
constant = function () {
  var args = arguments,
      index = -1,
      length = nativeMax(args.length - start, 0),
      array = Array(length);

  while (++index < length) {
    array[index] = args[start + index];
  }
  index = -1;
  var otherArgs = Array(start + 1);
  while (++index < start) {
    otherArgs[index] = args[index];
  }
  otherArgs[start] = transform(array);
  return apply(func, this, otherArgs);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.detect"></a>[function <span class="apidocSignatureSpan">async.</span>detect (obj, iteratee, callback)](#apidoc.element.async.detect)
- description and source-code
```javascript
detect = function (obj, iteratee, callback) {
    return fn(eachOf, obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.detectLimit"></a>[function <span class="apidocSignatureSpan">async.</span>detectLimit (obj, limit, iteratee, callback)](#apidoc.element.async.detectLimit)
- description and source-code
```javascript
detectLimit = function (obj, limit, iteratee, callback) {
    return fn(_eachOfLimit(limit), obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.detectSeries"></a>[function <span class="apidocSignatureSpan">async.</span>detectSeries (iterable, iteratee, callback)](#apidoc.element.async.detectSeries)
- description and source-code
```javascript
detectSeries = function (iterable, iteratee, callback) {
    return fn(iterable, limit, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.dir"></a>[function <span class="apidocSignatureSpan">async.</span>dir ()](#apidoc.element.async.dir)
- description and source-code
```javascript
dir = function () {
  var args = arguments,
      index = -1,
      length = nativeMax(args.length - start, 0),
      array = Array(length);

  while (++index < length) {
    array[index] = args[start + index];
  }
  index = -1;
  var otherArgs = Array(start + 1);
  while (++index < start) {
    otherArgs[index] = args[index];
  }
  otherArgs[start] = transform(array);
  return apply(func, this, otherArgs);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.doDuring"></a>[function <span class="apidocSignatureSpan">async.</span>doDuring (fn, test, callback)](#apidoc.element.async.doDuring)
- description and source-code
```javascript
function doDuring(fn, test, callback) {
    callback = onlyOnce(callback || noop);

    var next = rest(function (err, args) {
        if (err) return callback(err);
        args.push(check);
        test.apply(this, args);
    });

    function check(err, truth) {
        if (err) return callback(err);
        if (!truth) return callback(null);
        fn(next);
    }

    check(null, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.doUntil"></a>[function <span class="apidocSignatureSpan">async.</span>doUntil (fn, test, callback)](#apidoc.element.async.doUntil)
- description and source-code
```javascript
function doUntil(fn, test, callback) {
    doWhilst(fn, function () {
        return !test.apply(this, arguments);
    }, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.doWhilst"></a>[function <span class="apidocSignatureSpan">async.</span>doWhilst (iteratee, test, callback)](#apidoc.element.async.doWhilst)
- description and source-code
```javascript
function doWhilst(iteratee, test, callback) {
    callback = onlyOnce(callback || noop);
    var next = rest(function (err, args) {
        if (err) return callback(err);
        if (test.apply(this, args)) return iteratee(next);
        callback.apply(null, [null].concat(args));
    });
    iteratee(next);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.during"></a>[function <span class="apidocSignatureSpan">async.</span>during (test, fn, callback)](#apidoc.element.async.during)
- description and source-code
```javascript
function during(test, fn, callback) {
    callback = onlyOnce(callback || noop);

    function next(err) {
        if (err) return callback(err);
        test(check);
    }

    function check(err, truth) {
        if (err) return callback(err);
        if (!truth) return callback(null);
        fn(next);
    }

    test(check);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.each"></a>[function <span class="apidocSignatureSpan">async.</span>each (coll, iteratee, callback)](#apidoc.element.async.each)
- description and source-code
```javascript
function eachLimit(coll, iteratee, callback) {
  eachOf(coll, _withoutIndex(iteratee), callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.eachLimit"></a>[function <span class="apidocSignatureSpan">async.</span>eachLimit (coll, limit, iteratee, callback)](#apidoc.element.async.eachLimit)
- description and source-code
```javascript
function eachLimit$1(coll, limit, iteratee, callback) {
  _eachOfLimit(limit)(coll, _withoutIndex(iteratee), callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.eachOf"></a>[function <span class="apidocSignatureSpan">async.</span>eachOf (coll, iteratee, callback)](#apidoc.element.async.eachOf)
- description and source-code
```javascript
eachOf = function (coll, iteratee, callback) {
    var eachOfImplementation = isArrayLike(coll) ? eachOfArrayLike : eachOfGeneric;
    eachOfImplementation(coll, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.eachOfLimit"></a>[function <span class="apidocSignatureSpan">async.</span>eachOfLimit (coll, limit, iteratee, callback)](#apidoc.element.async.eachOfLimit)
- description and source-code
```javascript
function eachOfLimit(coll, limit, iteratee, callback) {
  _eachOfLimit(limit)(coll, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.eachOfSeries"></a>[function <span class="apidocSignatureSpan">async.</span>eachOfSeries (iterable, iteratee, callback)](#apidoc.element.async.eachOfSeries)
- description and source-code
```javascript
eachOfSeries = function (iterable, iteratee, callback) {
    return fn(iterable, limit, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.eachSeries"></a>[function <span class="apidocSignatureSpan">async.</span>eachSeries (iterable, iteratee, callback)](#apidoc.element.async.eachSeries)
- description and source-code
```javascript
eachSeries = function (iterable, iteratee, callback) {
    return fn(iterable, limit, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.ensureAsync"></a>[function <span class="apidocSignatureSpan">async.</span>ensureAsync (fn)](#apidoc.element.async.ensureAsync)
- description and source-code
```javascript
function ensureAsync(fn) {
    return initialParams(function (args, callback) {
        var sync = true;
        args.push(function () {
            var innerArgs = arguments;
            if (sync) {
                setImmediate$1(function () {
                    callback.apply(null, innerArgs);
                });
            } else {
                callback.apply(null, innerArgs);
            }
        });
        fn.apply(this, args);
        sync = false;
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.every"></a>[function <span class="apidocSignatureSpan">async.</span>every (obj, iteratee, callback)](#apidoc.element.async.every)
- description and source-code
```javascript
every = function (obj, iteratee, callback) {
    return fn(eachOf, obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.everyLimit"></a>[function <span class="apidocSignatureSpan">async.</span>everyLimit (obj, limit, iteratee, callback)](#apidoc.element.async.everyLimit)
- description and source-code
```javascript
everyLimit = function (obj, limit, iteratee, callback) {
    return fn(_eachOfLimit(limit), obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.everySeries"></a>[function <span class="apidocSignatureSpan">async.</span>everySeries (iterable, iteratee, callback)](#apidoc.element.async.everySeries)
- description and source-code
```javascript
everySeries = function (iterable, iteratee, callback) {
    return fn(iterable, limit, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.filter"></a>[function <span class="apidocSignatureSpan">async.</span>filter (obj, iteratee, callback)](#apidoc.element.async.filter)
- description and source-code
```javascript
filter = function (obj, iteratee, callback) {
    return fn(eachOf, obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.filterLimit"></a>[function <span class="apidocSignatureSpan">async.</span>filterLimit (obj, limit, iteratee, callback)](#apidoc.element.async.filterLimit)
- description and source-code
```javascript
filterLimit = function (obj, limit, iteratee, callback) {
    return fn(_eachOfLimit(limit), obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.filterSeries"></a>[function <span class="apidocSignatureSpan">async.</span>filterSeries (iterable, iteratee, callback)](#apidoc.element.async.filterSeries)
- description and source-code
```javascript
filterSeries = function (iterable, iteratee, callback) {
    return fn(iterable, limit, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.find"></a>[function <span class="apidocSignatureSpan">async.</span>find (obj, iteratee, callback)](#apidoc.element.async.find)
- description and source-code
```javascript
find = function (obj, iteratee, callback) {
    return fn(eachOf, obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.findLimit"></a>[function <span class="apidocSignatureSpan">async.</span>findLimit (obj, limit, iteratee, callback)](#apidoc.element.async.findLimit)
- description and source-code
```javascript
findLimit = function (obj, limit, iteratee, callback) {
    return fn(_eachOfLimit(limit), obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.findSeries"></a>[function <span class="apidocSignatureSpan">async.</span>findSeries (iterable, iteratee, callback)](#apidoc.element.async.findSeries)
- description and source-code
```javascript
findSeries = function (iterable, iteratee, callback) {
    return fn(iterable, limit, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.foldl"></a>[function <span class="apidocSignatureSpan">async.</span>foldl (coll, memo, iteratee, callback)](#apidoc.element.async.foldl)
- description and source-code
```javascript
function reduce(coll, memo, iteratee, callback) {
    callback = once(callback || noop);
    eachOfSeries(coll, function (x, i, callback) {
        iteratee(memo, x, function (err, v) {
            memo = v;
            callback(err);
        });
    }, function (err) {
        callback(err, memo);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.foldr"></a>[function <span class="apidocSignatureSpan">async.</span>foldr (array, memo, iteratee, callback)](#apidoc.element.async.foldr)
- description and source-code
```javascript
function reduceRight(array, memo, iteratee, callback) {
  var reversed = slice.call(array).reverse();
  reduce(reversed, memo, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.forEach"></a>[function <span class="apidocSignatureSpan">async.</span>forEach (coll, iteratee, callback)](#apidoc.element.async.forEach)
- description and source-code
```javascript
function eachLimit(coll, iteratee, callback) {
  eachOf(coll, _withoutIndex(iteratee), callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.forEachLimit"></a>[function <span class="apidocSignatureSpan">async.</span>forEachLimit (coll, limit, iteratee, callback)](#apidoc.element.async.forEachLimit)
- description and source-code
```javascript
function eachLimit$1(coll, limit, iteratee, callback) {
  _eachOfLimit(limit)(coll, _withoutIndex(iteratee), callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.forEachOf"></a>[function <span class="apidocSignatureSpan">async.</span>forEachOf (coll, iteratee, callback)](#apidoc.element.async.forEachOf)
- description and source-code
```javascript
forEachOf = function (coll, iteratee, callback) {
    var eachOfImplementation = isArrayLike(coll) ? eachOfArrayLike : eachOfGeneric;
    eachOfImplementation(coll, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.forEachOfLimit"></a>[function <span class="apidocSignatureSpan">async.</span>forEachOfLimit (coll, limit, iteratee, callback)](#apidoc.element.async.forEachOfLimit)
- description and source-code
```javascript
function eachOfLimit(coll, limit, iteratee, callback) {
  _eachOfLimit(limit)(coll, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.forEachOfSeries"></a>[function <span class="apidocSignatureSpan">async.</span>forEachOfSeries (iterable, iteratee, callback)](#apidoc.element.async.forEachOfSeries)
- description and source-code
```javascript
forEachOfSeries = function (iterable, iteratee, callback) {
    return fn(iterable, limit, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.forEachSeries"></a>[function <span class="apidocSignatureSpan">async.</span>forEachSeries (iterable, iteratee, callback)](#apidoc.element.async.forEachSeries)
- description and source-code
```javascript
forEachSeries = function (iterable, iteratee, callback) {
    return fn(iterable, limit, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.forever"></a>[function <span class="apidocSignatureSpan">async.</span>forever (fn, errback)](#apidoc.element.async.forever)
- description and source-code
```javascript
function forever(fn, errback) {
    var done = onlyOnce(errback || noop);
    var task = ensureAsync(fn);

    function next(err) {
        if (err) return done(err);
        task(next);
    }
    next();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.inject"></a>[function <span class="apidocSignatureSpan">async.</span>inject (coll, memo, iteratee, callback)](#apidoc.element.async.inject)
- description and source-code
```javascript
function reduce(coll, memo, iteratee, callback) {
    callback = once(callback || noop);
    eachOfSeries(coll, function (x, i, callback) {
        iteratee(memo, x, function (err, v) {
            memo = v;
            callback(err);
        });
    }, function (err) {
        callback(err, memo);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.log"></a>[function <span class="apidocSignatureSpan">async.</span>log ()](#apidoc.element.async.log)
- description and source-code
```javascript
log = function () {
  var args = arguments,
      index = -1,
      length = nativeMax(args.length - start, 0),
      array = Array(length);

  while (++index < length) {
    array[index] = args[start + index];
  }
  index = -1;
  var otherArgs = Array(start + 1);
  while (++index < start) {
    otherArgs[index] = args[index];
  }
  otherArgs[start] = transform(array);
  return apply(func, this, otherArgs);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.map"></a>[function <span class="apidocSignatureSpan">async.</span>map (obj, iteratee, callback)](#apidoc.element.async.map)
- description and source-code
```javascript
map = function (obj, iteratee, callback) {
    return fn(eachOf, obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.mapLimit"></a>[function <span class="apidocSignatureSpan">async.</span>mapLimit (obj, limit, iteratee, callback)](#apidoc.element.async.mapLimit)
- description and source-code
```javascript
mapLimit = function (obj, limit, iteratee, callback) {
    return fn(_eachOfLimit(limit), obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.mapSeries"></a>[function <span class="apidocSignatureSpan">async.</span>mapSeries (iterable, iteratee, callback)](#apidoc.element.async.mapSeries)
- description and source-code
```javascript
mapSeries = function (iterable, iteratee, callback) {
    return fn(iterable, limit, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.mapValues"></a>[function <span class="apidocSignatureSpan">async.</span>mapValues (iterable, iteratee, callback)](#apidoc.element.async.mapValues)
- description and source-code
```javascript
mapValues = function (iterable, iteratee, callback) {
    return fn(iterable, limit, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.mapValuesLimit"></a>[function <span class="apidocSignatureSpan">async.</span>mapValuesLimit (obj, limit, iteratee, callback)](#apidoc.element.async.mapValuesLimit)
- description and source-code
```javascript
function mapValuesLimit(obj, limit, iteratee, callback) {
    callback = once(callback || noop);
    var newObj = {};
    eachOfLimit(obj, limit, function (val, key, next) {
        iteratee(val, key, function (err, result) {
            if (err) return next(err);
            newObj[key] = result;
            next();
        });
    }, function (err) {
        callback(err, newObj);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.mapValuesSeries"></a>[function <span class="apidocSignatureSpan">async.</span>mapValuesSeries (iterable, iteratee, callback)](#apidoc.element.async.mapValuesSeries)
- description and source-code
```javascript
mapValuesSeries = function (iterable, iteratee, callback) {
    return fn(iterable, limit, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.memoize"></a>[function <span class="apidocSignatureSpan">async.</span>memoize (fn, hasher)](#apidoc.element.async.memoize)
- description and source-code
```javascript
function memoize(fn, hasher) {
    var memo = Object.create(null);
    var queues = Object.create(null);
    hasher = hasher || identity;
    var memoized = initialParams(function memoized(args, callback) {
        var key = hasher.apply(null, args);
        if (has(memo, key)) {
            setImmediate$1(function () {
                callback.apply(null, memo[key]);
            });
        } else if (has(queues, key)) {
            queues[key].push(callback);
        } else {
            queues[key] = [callback];
            fn.apply(null, args.concat(rest(function (args) {
                memo[key] = args;
                var q = queues[key];
                delete queues[key];
                for (var i = 0, l = q.length; i < l; i++) {
                    q[i].apply(null, args);
                }
            })));
        }
    });
    memoized.memo = memo;
    memoized.unmemoized = fn;
    return memoized;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.nextTick"></a>[function <span class="apidocSignatureSpan">async.</span>nextTick ()](#apidoc.element.async.nextTick)
- description and source-code
```javascript
nextTick = function () {
  var args = arguments,
      index = -1,
      length = nativeMax(args.length - start, 0),
      array = Array(length);

  while (++index < length) {
    array[index] = args[start + index];
  }
  index = -1;
  var otherArgs = Array(start + 1);
  while (++index < start) {
    otherArgs[index] = args[index];
  }
  otherArgs[start] = transform(array);
  return apply(func, this, otherArgs);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.parallel"></a>[function <span class="apidocSignatureSpan">async.</span>parallel (tasks, callback)](#apidoc.element.async.parallel)
- description and source-code
```javascript
function parallelLimit(tasks, callback) {
  _parallel(eachOf, tasks, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.parallelLimit"></a>[function <span class="apidocSignatureSpan">async.</span>parallelLimit (tasks, limit, callback)](#apidoc.element.async.parallelLimit)
- description and source-code
```javascript
function parallelLimit$1(tasks, limit, callback) {
  _parallel(_eachOfLimit(limit), tasks, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.priorityQueue"></a>[function <span class="apidocSignatureSpan">async.</span>priorityQueue (worker, concurrency)](#apidoc.element.async.priorityQueue)
- description and source-code
```javascript
priorityQueue = function (worker, concurrency) {
    // Start with a normal queue
    var q = queue$1(worker, concurrency);

    // Override push to accept second parameter representing priority
    q.push = function (data, priority, callback) {
        if (callback == null) callback = noop;
        if (typeof callback !== 'function') {
            throw new Error('task callback must be a function');
        }
        q.started = true;
        if (!isArray(data)) {
            data = [data];
        }
        if (data.length === 0) {
            // call drain immediately if there are no tasks
            return setImmediate$1(function () {
                q.drain();
            });
        }

        priority = priority || 0;
        var nextNode = q._tasks.head;
        while (nextNode && priority >= nextNode.priority) {
            nextNode = nextNode.next;
        }

        for (var i = 0, l = data.length; i < l; i++) {
            var item = {
                data: data[i],
                priority: priority,
                callback: callback
            };

            if (nextNode) {
                q._tasks.insertBefore(nextNode, item);
            } else {
                q._tasks.push(item);
            }
        }
        setImmediate$1(q.process);
    };

    // Remove unshift function
    delete q.unshift;

    return q;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.queue"></a>[function <span class="apidocSignatureSpan">async.</span>queue (worker, concurrency)](#apidoc.element.async.queue)
- description and source-code
```javascript
queue = function (worker, concurrency) {
  return queue(function (items, cb) {
    worker(items[0], cb);
  }, concurrency, 1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.race"></a>[function <span class="apidocSignatureSpan">async.</span>race (tasks, callback)](#apidoc.element.async.race)
- description and source-code
```javascript
function race(tasks, callback) {
    callback = once(callback || noop);
    if (!isArray(tasks)) return callback(new TypeError('First argument to race must be an array of functions'));
    if (!tasks.length) return callback();
    for (var i = 0, l = tasks.length; i < l; i++) {
        tasks[i](callback);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.reduce"></a>[function <span class="apidocSignatureSpan">async.</span>reduce (coll, memo, iteratee, callback)](#apidoc.element.async.reduce)
- description and source-code
```javascript
function reduce(coll, memo, iteratee, callback) {
    callback = once(callback || noop);
    eachOfSeries(coll, function (x, i, callback) {
        iteratee(memo, x, function (err, v) {
            memo = v;
            callback(err);
        });
    }, function (err) {
        callback(err, memo);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.reduceRight"></a>[function <span class="apidocSignatureSpan">async.</span>reduceRight (array, memo, iteratee, callback)](#apidoc.element.async.reduceRight)
- description and source-code
```javascript
function reduceRight(array, memo, iteratee, callback) {
  var reversed = slice.call(array).reverse();
  reduce(reversed, memo, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.reflect"></a>[function <span class="apidocSignatureSpan">async.</span>reflect (fn)](#apidoc.element.async.reflect)
- description and source-code
```javascript
function reflect(fn) {
    return initialParams(function reflectOn(args, reflectCallback) {
        args.push(rest(function callback(err, cbArgs) {
            if (err) {
                reflectCallback(null, {
                    error: err
                });
            } else {
                var value = null;
                if (cbArgs.length === 1) {
                    value = cbArgs[0];
                } else if (cbArgs.length > 1) {
                    value = cbArgs;
                }
                reflectCallback(null, {
                    value: value
                });
            }
        }));

        return fn.apply(this, args);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.reflectAll"></a>[function <span class="apidocSignatureSpan">async.</span>reflectAll (tasks)](#apidoc.element.async.reflectAll)
- description and source-code
```javascript
function reflectAll(tasks) {
    var results;
    if (isArray(tasks)) {
        results = arrayMap(tasks, reflect);
    } else {
        results = {};
        baseForOwn(tasks, function (task, key) {
            results[key] = reflect.call(this, task);
        });
    }
    return results;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.reject"></a>[function <span class="apidocSignatureSpan">async.</span>reject (obj, iteratee, callback)](#apidoc.element.async.reject)
- description and source-code
```javascript
reject = function (obj, iteratee, callback) {
    return fn(eachOf, obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.rejectLimit"></a>[function <span class="apidocSignatureSpan">async.</span>rejectLimit (obj, limit, iteratee, callback)](#apidoc.element.async.rejectLimit)
- description and source-code
```javascript
rejectLimit = function (obj, limit, iteratee, callback) {
    return fn(_eachOfLimit(limit), obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.rejectSeries"></a>[function <span class="apidocSignatureSpan">async.</span>rejectSeries (iterable, iteratee, callback)](#apidoc.element.async.rejectSeries)
- description and source-code
```javascript
rejectSeries = function (iterable, iteratee, callback) {
    return fn(iterable, limit, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.retry"></a>[function <span class="apidocSignatureSpan">async.</span>retry (opts, task, callback)](#apidoc.element.async.retry)
- description and source-code
```javascript
function retry(opts, task, callback) {
    var DEFAULT_TIMES = 5;
    var DEFAULT_INTERVAL = 0;

    var options = {
        times: DEFAULT_TIMES,
        intervalFunc: constant$1(DEFAULT_INTERVAL)
    };

    function parseTimes(acc, t) {
        if (typeof t === 'object') {
            acc.times = +t.times || DEFAULT_TIMES;

            acc.intervalFunc = typeof t.interval === 'function' ? t.interval : constant$1(+t.interval || DEFAULT_INTERVAL);

            acc.errorFilter = t.errorFilter;
        } else if (typeof t === 'number' || typeof t === 'string') {
            acc.times = +t || DEFAULT_TIMES;
        } else {
            throw new Error("Invalid arguments for async.retry");
        }
    }

    if (arguments.length < 3 && typeof opts === 'function') {
        callback = task || noop;
        task = opts;
    } else {
        parseTimes(options, opts);
        callback = callback || noop;
    }

    if (typeof task !== 'function') {
        throw new Error("Invalid arguments for async.retry");
    }

    var attempt = 1;
    function retryAttempt() {
        task(function (err) {
            if (err && attempt++ < options.times && (typeof options.errorFilter != 'function' || options.errorFilter(err))) {
                setTimeout(retryAttempt, options.intervalFunc(attempt));
            } else {
                callback.apply(null, arguments);
            }
        });
    }

    retryAttempt();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.retryable"></a>[function <span class="apidocSignatureSpan">async.</span>retryable (opts, task)](#apidoc.element.async.retryable)
- description and source-code
```javascript
retryable = function (opts, task) {
    if (!task) {
        task = opts;
        opts = null;
    }
    return initialParams(function (args, callback) {
        function taskFn(cb) {
            task.apply(null, args.concat(cb));
        }

        if (opts) retry(opts, taskFn, callback);else retry(taskFn, callback);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.select"></a>[function <span class="apidocSignatureSpan">async.</span>select (obj, iteratee, callback)](#apidoc.element.async.select)
- description and source-code
```javascript
select = function (obj, iteratee, callback) {
    return fn(eachOf, obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.selectLimit"></a>[function <span class="apidocSignatureSpan">async.</span>selectLimit (obj, limit, iteratee, callback)](#apidoc.element.async.selectLimit)
- description and source-code
```javascript
selectLimit = function (obj, limit, iteratee, callback) {
    return fn(_eachOfLimit(limit), obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.selectSeries"></a>[function <span class="apidocSignatureSpan">async.</span>selectSeries (iterable, iteratee, callback)](#apidoc.element.async.selectSeries)
- description and source-code
```javascript
selectSeries = function (iterable, iteratee, callback) {
    return fn(iterable, limit, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.seq"></a>[function <span class="apidocSignatureSpan">async.</span>seq ()](#apidoc.element.async.seq)
- description and source-code
```javascript
seq = function () {
  var args = arguments,
      index = -1,
      length = nativeMax(args.length - start, 0),
      array = Array(length);

  while (++index < length) {
    array[index] = args[start + index];
  }
  index = -1;
  var otherArgs = Array(start + 1);
  while (++index < start) {
    otherArgs[index] = args[index];
  }
  otherArgs[start] = transform(array);
  return apply(func, this, otherArgs);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.series"></a>[function <span class="apidocSignatureSpan">async.</span>series (tasks, callback)](#apidoc.element.async.series)
- description and source-code
```javascript
function series(tasks, callback) {
  _parallel(eachOfSeries, tasks, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.setImmediate"></a>[function <span class="apidocSignatureSpan">async.</span>setImmediate ()](#apidoc.element.async.setImmediate)
- description and source-code
```javascript
setImmediate = function () {
  var args = arguments,
      index = -1,
      length = nativeMax(args.length - start, 0),
      array = Array(length);

  while (++index < length) {
    array[index] = args[start + index];
  }
  index = -1;
  var otherArgs = Array(start + 1);
  while (++index < start) {
    otherArgs[index] = args[index];
  }
  otherArgs[start] = transform(array);
  return apply(func, this, otherArgs);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.some"></a>[function <span class="apidocSignatureSpan">async.</span>some (obj, iteratee, callback)](#apidoc.element.async.some)
- description and source-code
```javascript
some = function (obj, iteratee, callback) {
    return fn(eachOf, obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.someLimit"></a>[function <span class="apidocSignatureSpan">async.</span>someLimit (obj, limit, iteratee, callback)](#apidoc.element.async.someLimit)
- description and source-code
```javascript
someLimit = function (obj, limit, iteratee, callback) {
    return fn(_eachOfLimit(limit), obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.someSeries"></a>[function <span class="apidocSignatureSpan">async.</span>someSeries (iterable, iteratee, callback)](#apidoc.element.async.someSeries)
- description and source-code
```javascript
someSeries = function (iterable, iteratee, callback) {
    return fn(iterable, limit, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.sortBy"></a>[function <span class="apidocSignatureSpan">async.</span>sortBy (coll, iteratee, callback)](#apidoc.element.async.sortBy)
- description and source-code
```javascript
function sortBy(coll, iteratee, callback) {
    map(coll, function (x, callback) {
        iteratee(x, function (err, criteria) {
            if (err) return callback(err);
            callback(null, { value: x, criteria: criteria });
        });
    }, function (err, results) {
        if (err) return callback(err);
        callback(null, arrayMap(results.sort(comparator), baseProperty('value')));
    });

    function comparator(left, right) {
        var a = left.criteria,
            b = right.criteria;
        return a < b ? -1 : a > b ? 1 : 0;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.timeout"></a>[function <span class="apidocSignatureSpan">async.</span>timeout (asyncFn, milliseconds, info)](#apidoc.element.async.timeout)
- description and source-code
```javascript
function timeout(asyncFn, milliseconds, info) {
    var originalCallback, timer;
    var timedOut = false;

    function injectedCallback() {
        if (!timedOut) {
            originalCallback.apply(null, arguments);
            clearTimeout(timer);
        }
    }

    function timeoutCallback() {
        var name = asyncFn.name || 'anonymous';
        var error = new Error('Callback function "' + name + '" timed out.');
        error.code = 'ETIMEDOUT';
        if (info) {
            error.info = info;
        }
        timedOut = true;
        originalCallback(error);
    }

    return initialParams(function (args, origCallback) {
        originalCallback = origCallback;
        // setup timer and call original function
        timer = setTimeout(timeoutCallback, milliseconds);
        asyncFn.apply(null, args.concat(injectedCallback));
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.times"></a>[function <span class="apidocSignatureSpan">async.</span>times (iterable, iteratee, callback)](#apidoc.element.async.times)
- description and source-code
```javascript
times = function (iterable, iteratee, callback) {
    return fn(iterable, limit, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.timesLimit"></a>[function <span class="apidocSignatureSpan">async.</span>timesLimit (count, limit, iteratee, callback)](#apidoc.element.async.timesLimit)
- description and source-code
```javascript
function timeLimit(count, limit, iteratee, callback) {
  mapLimit(baseRange(0, count, 1), limit, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.timesSeries"></a>[function <span class="apidocSignatureSpan">async.</span>timesSeries (iterable, iteratee, callback)](#apidoc.element.async.timesSeries)
- description and source-code
```javascript
timesSeries = function (iterable, iteratee, callback) {
    return fn(iterable, limit, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.transform"></a>[function <span class="apidocSignatureSpan">async.</span>transform (coll, accumulator, iteratee, callback)](#apidoc.element.async.transform)
- description and source-code
```javascript
function transform(coll, accumulator, iteratee, callback) {
    if (arguments.length === 3) {
        callback = iteratee;
        iteratee = accumulator;
        accumulator = isArray(coll) ? [] : {};
    }
    callback = once(callback || noop);

    eachOf(coll, function (v, k, cb) {
        iteratee(accumulator, v, k, cb);
    }, function (err) {
        callback(err, accumulator);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.unmemoize"></a>[function <span class="apidocSignatureSpan">async.</span>unmemoize (fn)](#apidoc.element.async.unmemoize)
- description and source-code
```javascript
function unmemoize(fn) {
    return function () {
        return (fn.unmemoized || fn).apply(null, arguments);
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.until"></a>[function <span class="apidocSignatureSpan">async.</span>until (test, fn, callback)](#apidoc.element.async.until)
- description and source-code
```javascript
function until(test, fn, callback) {
    whilst(function () {
        return !test.apply(this, arguments);
    }, fn, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.waterfall"></a>[function <span class="apidocSignatureSpan">async.</span>waterfall (tasks, callback)](#apidoc.element.async.waterfall)
- description and source-code
```javascript
waterfall = function (tasks, callback) {
    callback = once(callback || noop);
    if (!isArray(tasks)) return callback(new Error('First argument to waterfall must be an array of functions'));
    if (!tasks.length) return callback();
    var taskIndex = 0;

    function nextTask(args) {
        if (taskIndex === tasks.length) {
            return callback.apply(null, [null].concat(args));
        }

        var taskCallback = onlyOnce(rest(function (err, args) {
            if (err) {
                return callback.apply(null, [err].concat(args));
            }
            nextTask(args);
        }));

        args.push(taskCallback);

        var task = tasks[taskIndex++];
        task.apply(null, args);
    }

    nextTask([]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.whilst"></a>[function <span class="apidocSignatureSpan">async.</span>whilst (test, iteratee, callback)](#apidoc.element.async.whilst)
- description and source-code
```javascript
function whilst(test, iteratee, callback) {
    callback = onlyOnce(callback || noop);
    if (!test()) return callback(null);
    var next = rest(function (err, args) {
        if (err) return callback(err);
        if (test()) return iteratee(next);
        callback.apply(null, [null].concat(args));
    });
    iteratee(next);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.wrapSync"></a>[function <span class="apidocSignatureSpan">async.</span>wrapSync (func)](#apidoc.element.async.wrapSync)
- description and source-code
```javascript
function asyncify(func) {
    return initialParams(function (args, callback) {
        var result;
        try {
            result = func.apply(this, args);
        } catch (e) {
            return callback(e);
        }
        // if result is Promise object
        if (isObject(result) && typeof result.then === 'function') {
            result.then(function (value) {
                callback(null, value);
            }, function (err) {
                callback(err.message ? err : new Error(err));
            });
        } else {
            callback(null, result);
        }
    });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.async.default"></a>[module async.default](#apidoc.module.async.default)

#### <a name="apidoc.element.async.default.all"></a>[function <span class="apidocSignatureSpan">async.default.</span>all (obj, iteratee, callback)](#apidoc.element.async.default.all)
- description and source-code
```javascript
all = function (obj, iteratee, callback) {
    return fn(eachOf, obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.any"></a>[function <span class="apidocSignatureSpan">async.default.</span>any (obj, iteratee, callback)](#apidoc.element.async.default.any)
- description and source-code
```javascript
any = function (obj, iteratee, callback) {
    return fn(eachOf, obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.apply"></a>[function <span class="apidocSignatureSpan">async.default.</span>apply ()](#apidoc.element.async.default.apply)
- description and source-code
```javascript
apply = function () {
  var args = arguments,
      index = -1,
      length = nativeMax(args.length - start, 0),
      array = Array(length);

  while (++index < length) {
    array[index] = args[start + index];
  }
  index = -1;
  var otherArgs = Array(start + 1);
  while (++index < start) {
    otherArgs[index] = args[index];
  }
  otherArgs[start] = transform(array);
  return apply(func, this, otherArgs);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.applyEach"></a>[function <span class="apidocSignatureSpan">async.default.</span>applyEach ()](#apidoc.element.async.default.applyEach)
- description and source-code
```javascript
applyEach = function () {
  var args = arguments,
      index = -1,
      length = nativeMax(args.length - start, 0),
      array = Array(length);

  while (++index < length) {
    array[index] = args[start + index];
  }
  index = -1;
  var otherArgs = Array(start + 1);
  while (++index < start) {
    otherArgs[index] = args[index];
  }
  otherArgs[start] = transform(array);
  return apply(func, this, otherArgs);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.applyEachSeries"></a>[function <span class="apidocSignatureSpan">async.default.</span>applyEachSeries ()](#apidoc.element.async.default.applyEachSeries)
- description and source-code
```javascript
applyEachSeries = function () {
  var args = arguments,
      index = -1,
      length = nativeMax(args.length - start, 0),
      array = Array(length);

  while (++index < length) {
    array[index] = args[start + index];
  }
  index = -1;
  var otherArgs = Array(start + 1);
  while (++index < start) {
    otherArgs[index] = args[index];
  }
  otherArgs[start] = transform(array);
  return apply(func, this, otherArgs);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.asyncify"></a>[function <span class="apidocSignatureSpan">async.default.</span>asyncify (func)](#apidoc.element.async.default.asyncify)
- description and source-code
```javascript
function asyncify(func) {
    return initialParams(function (args, callback) {
        var result;
        try {
            result = func.apply(this, args);
        } catch (e) {
            return callback(e);
        }
        // if result is Promise object
        if (isObject(result) && typeof result.then === 'function') {
            result.then(function (value) {
                callback(null, value);
            }, function (err) {
                callback(err.message ? err : new Error(err));
            });
        } else {
            callback(null, result);
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.auto"></a>[function <span class="apidocSignatureSpan">async.default.</span>auto (tasks, concurrency, callback)](#apidoc.element.async.default.auto)
- description and source-code
```javascript
auto = function (tasks, concurrency, callback) {
    if (typeof concurrency === 'function') {
        // concurrency is optional, shift the args.
        callback = concurrency;
        concurrency = null;
    }
    callback = once(callback || noop);
    var keys$$1 = keys(tasks);
    var numTasks = keys$$1.length;
    if (!numTasks) {
        return callback(null);
    }
    if (!concurrency) {
        concurrency = numTasks;
    }

    var results = {};
    var runningTasks = 0;
    var hasError = false;

    var listeners = Object.create(null);

    var readyTasks = [];

    // for cycle detection:
    var readyToCheck = []; // tasks that have been identified as reachable
    // without the possibility of returning to an ancestor task
    var uncheckedDependencies = {};

    baseForOwn(tasks, function (task, key) {
        if (!isArray(task)) {
            // no dependencies
            enqueueTask(key, [task]);
            readyToCheck.push(key);
            return;
        }

        var dependencies = task.slice(0, task.length - 1);
        var remainingDependencies = dependencies.length;
        if (remainingDependencies === 0) {
            enqueueTask(key, task);
            readyToCheck.push(key);
            return;
        }
        uncheckedDependencies[key] = remainingDependencies;

        arrayEach(dependencies, function (dependencyName) {
            if (!tasks[dependencyName]) {
                throw new Error('async.auto task '' + key + '' has a non-existent dependency '' + dependencyName + '' in ' + dependencies
.join(', '));
            }
            addListener(dependencyName, function () {
                remainingDependencies--;
                if (remainingDependencies === 0) {
                    enqueueTask(key, task);
                }
            });
        });
    });

    checkForDeadlocks();
    processQueue();

    function enqueueTask(key, task) {
        readyTasks.push(function () {
            runTask(key, task);
        });
    }

    function processQueue() {
        if (readyTasks.length === 0 && runningTasks === 0) {
            return callback(null, results);
        }
        while (readyTasks.length && runningTasks < concurrency) {
            var run = readyTasks.shift();
            run();
        }
    }

    function addListener(taskName, fn) {
        var taskListeners = listeners[taskName];
        if (!taskListeners) {
            taskListeners = listeners[taskName] = [];
        }

        taskListeners.push(fn);
    }

    function taskComplete(taskName) {
        var taskListeners = listeners[taskName] || [];
        arrayEach(taskListeners, function (fn) {
            fn();
        });
        processQueue();
    }

    function runTask(key, task) {
        if (hasError) return;

        var taskCallback = onlyOnce(rest(function (err, args) {
            runningTasks--;
            if (args.length <= 1) {
                args = args[0];
            }
            if (err) {
                var safeResults = {};
                baseForOwn(results, function (val, rkey) {
                    safeResults[rkey] = val;
                });
                safeResults[key] = args;
                hasError = true;
                listeners = Object.create(null);

                callback(err, safeResults);
            } else {
                results[key] = args;
                taskComplete(key);
            }
        }));

        runningTasks++;
        var taskFn = task[task.length - 1];
        if (task.length > 1) {
            taskFn(results, taskCallback);
        } else {
            taskFn(taskCallback);
        }
    }

    function checkForDeadlocks() {
        // Kahn's algorithm
        // https://en.wikipedia.org/wiki/Topological_sorting#Kahn.27s_algorithm
        // http://connalle.blogspot.com/2013/10/topological-sortingkahn-algorithm.html
        var currentTask;
        var counter = 0;
        while (readyToCheck.length) {
            currentTask = readyToCheck.pop();
            counter++;
            arrayEach(getDependents(currentTask), function (dependent) { ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.autoInject"></a>[function <span class="apidocSignatureSpan">async.default.</span>autoInject (tasks, callback)](#apidoc.element.async.default.autoInject)
- description and source-code
```javascript
function autoInject(tasks, callback) {
    var newTasks = {};

    baseForOwn(tasks, function (taskFn, key) {
        var params;

        if (isArray(taskFn)) {
            params = taskFn.slice(0, -1);
            taskFn = taskFn[taskFn.length - 1];

            newTasks[key] = params.concat(params.length > 0 ? newTask : taskFn);
        } else if (taskFn.length === 1) {
            // no dependencies, use the function as-is
            newTasks[key] = taskFn;
        } else {
            params = parseParams(taskFn);
            if (taskFn.length === 0 && params.length === 0) {
                throw new Error("autoInject task functions require explicit parameters.");
            }

            params.pop();

            newTasks[key] = params.concat(newTask);
        }

        function newTask(results, taskCb) {
            var newArgs = arrayMap(params, function (name) {
                return results[name];
            });
            newArgs.push(taskCb);
            taskFn.apply(null, newArgs);
        }
    });

    auto(newTasks, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.cargo"></a>[function <span class="apidocSignatureSpan">async.default.</span>cargo (worker, payload)](#apidoc.element.async.default.cargo)
- description and source-code
```javascript
function cargo(worker, payload) {
  return queue(worker, 1, payload);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.compose"></a>[function <span class="apidocSignatureSpan">async.default.</span>compose ()](#apidoc.element.async.default.compose)
- description and source-code
```javascript
compose = function () {
  var args = arguments,
      index = -1,
      length = nativeMax(args.length - start, 0),
      array = Array(length);

  while (++index < length) {
    array[index] = args[start + index];
  }
  index = -1;
  var otherArgs = Array(start + 1);
  while (++index < start) {
    otherArgs[index] = args[index];
  }
  otherArgs[start] = transform(array);
  return apply(func, this, otherArgs);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.concat"></a>[function <span class="apidocSignatureSpan">async.default.</span>concat (obj, iteratee, callback)](#apidoc.element.async.default.concat)
- description and source-code
```javascript
concat = function (obj, iteratee, callback) {
    return fn(eachOf, obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.concatSeries"></a>[function <span class="apidocSignatureSpan">async.default.</span>concatSeries (obj, iteratee, callback)](#apidoc.element.async.default.concatSeries)
- description and source-code
```javascript
concatSeries = function (obj, iteratee, callback) {
    return fn(eachOfSeries, obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.constant"></a>[function <span class="apidocSignatureSpan">async.default.</span>constant ()](#apidoc.element.async.default.constant)
- description and source-code
```javascript
constant = function () {
  var args = arguments,
      index = -1,
      length = nativeMax(args.length - start, 0),
      array = Array(length);

  while (++index < length) {
    array[index] = args[start + index];
  }
  index = -1;
  var otherArgs = Array(start + 1);
  while (++index < start) {
    otherArgs[index] = args[index];
  }
  otherArgs[start] = transform(array);
  return apply(func, this, otherArgs);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.detect"></a>[function <span class="apidocSignatureSpan">async.default.</span>detect (obj, iteratee, callback)](#apidoc.element.async.default.detect)
- description and source-code
```javascript
detect = function (obj, iteratee, callback) {
    return fn(eachOf, obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.detectLimit"></a>[function <span class="apidocSignatureSpan">async.default.</span>detectLimit (obj, limit, iteratee, callback)](#apidoc.element.async.default.detectLimit)
- description and source-code
```javascript
detectLimit = function (obj, limit, iteratee, callback) {
    return fn(_eachOfLimit(limit), obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.detectSeries"></a>[function <span class="apidocSignatureSpan">async.default.</span>detectSeries (iterable, iteratee, callback)](#apidoc.element.async.default.detectSeries)
- description and source-code
```javascript
detectSeries = function (iterable, iteratee, callback) {
    return fn(iterable, limit, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.dir"></a>[function <span class="apidocSignatureSpan">async.default.</span>dir ()](#apidoc.element.async.default.dir)
- description and source-code
```javascript
dir = function () {
  var args = arguments,
      index = -1,
      length = nativeMax(args.length - start, 0),
      array = Array(length);

  while (++index < length) {
    array[index] = args[start + index];
  }
  index = -1;
  var otherArgs = Array(start + 1);
  while (++index < start) {
    otherArgs[index] = args[index];
  }
  otherArgs[start] = transform(array);
  return apply(func, this, otherArgs);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.doDuring"></a>[function <span class="apidocSignatureSpan">async.default.</span>doDuring (fn, test, callback)](#apidoc.element.async.default.doDuring)
- description and source-code
```javascript
function doDuring(fn, test, callback) {
    callback = onlyOnce(callback || noop);

    var next = rest(function (err, args) {
        if (err) return callback(err);
        args.push(check);
        test.apply(this, args);
    });

    function check(err, truth) {
        if (err) return callback(err);
        if (!truth) return callback(null);
        fn(next);
    }

    check(null, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.doUntil"></a>[function <span class="apidocSignatureSpan">async.default.</span>doUntil (fn, test, callback)](#apidoc.element.async.default.doUntil)
- description and source-code
```javascript
function doUntil(fn, test, callback) {
    doWhilst(fn, function () {
        return !test.apply(this, arguments);
    }, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.doWhilst"></a>[function <span class="apidocSignatureSpan">async.default.</span>doWhilst (iteratee, test, callback)](#apidoc.element.async.default.doWhilst)
- description and source-code
```javascript
function doWhilst(iteratee, test, callback) {
    callback = onlyOnce(callback || noop);
    var next = rest(function (err, args) {
        if (err) return callback(err);
        if (test.apply(this, args)) return iteratee(next);
        callback.apply(null, [null].concat(args));
    });
    iteratee(next);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.during"></a>[function <span class="apidocSignatureSpan">async.default.</span>during (test, fn, callback)](#apidoc.element.async.default.during)
- description and source-code
```javascript
function during(test, fn, callback) {
    callback = onlyOnce(callback || noop);

    function next(err) {
        if (err) return callback(err);
        test(check);
    }

    function check(err, truth) {
        if (err) return callback(err);
        if (!truth) return callback(null);
        fn(next);
    }

    test(check);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.each"></a>[function <span class="apidocSignatureSpan">async.default.</span>each (coll, iteratee, callback)](#apidoc.element.async.default.each)
- description and source-code
```javascript
function eachLimit(coll, iteratee, callback) {
  eachOf(coll, _withoutIndex(iteratee), callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.eachLimit"></a>[function <span class="apidocSignatureSpan">async.default.</span>eachLimit (coll, limit, iteratee, callback)](#apidoc.element.async.default.eachLimit)
- description and source-code
```javascript
function eachLimit$1(coll, limit, iteratee, callback) {
  _eachOfLimit(limit)(coll, _withoutIndex(iteratee), callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.eachOf"></a>[function <span class="apidocSignatureSpan">async.default.</span>eachOf (coll, iteratee, callback)](#apidoc.element.async.default.eachOf)
- description and source-code
```javascript
eachOf = function (coll, iteratee, callback) {
    var eachOfImplementation = isArrayLike(coll) ? eachOfArrayLike : eachOfGeneric;
    eachOfImplementation(coll, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.eachOfLimit"></a>[function <span class="apidocSignatureSpan">async.default.</span>eachOfLimit (coll, limit, iteratee, callback)](#apidoc.element.async.default.eachOfLimit)
- description and source-code
```javascript
function eachOfLimit(coll, limit, iteratee, callback) {
  _eachOfLimit(limit)(coll, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.eachOfSeries"></a>[function <span class="apidocSignatureSpan">async.default.</span>eachOfSeries (iterable, iteratee, callback)](#apidoc.element.async.default.eachOfSeries)
- description and source-code
```javascript
eachOfSeries = function (iterable, iteratee, callback) {
    return fn(iterable, limit, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.eachSeries"></a>[function <span class="apidocSignatureSpan">async.default.</span>eachSeries (iterable, iteratee, callback)](#apidoc.element.async.default.eachSeries)
- description and source-code
```javascript
eachSeries = function (iterable, iteratee, callback) {
    return fn(iterable, limit, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.ensureAsync"></a>[function <span class="apidocSignatureSpan">async.default.</span>ensureAsync (fn)](#apidoc.element.async.default.ensureAsync)
- description and source-code
```javascript
function ensureAsync(fn) {
    return initialParams(function (args, callback) {
        var sync = true;
        args.push(function () {
            var innerArgs = arguments;
            if (sync) {
                setImmediate$1(function () {
                    callback.apply(null, innerArgs);
                });
            } else {
                callback.apply(null, innerArgs);
            }
        });
        fn.apply(this, args);
        sync = false;
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.every"></a>[function <span class="apidocSignatureSpan">async.default.</span>every (obj, iteratee, callback)](#apidoc.element.async.default.every)
- description and source-code
```javascript
every = function (obj, iteratee, callback) {
    return fn(eachOf, obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.everyLimit"></a>[function <span class="apidocSignatureSpan">async.default.</span>everyLimit (obj, limit, iteratee, callback)](#apidoc.element.async.default.everyLimit)
- description and source-code
```javascript
everyLimit = function (obj, limit, iteratee, callback) {
    return fn(_eachOfLimit(limit), obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.everySeries"></a>[function <span class="apidocSignatureSpan">async.default.</span>everySeries (iterable, iteratee, callback)](#apidoc.element.async.default.everySeries)
- description and source-code
```javascript
everySeries = function (iterable, iteratee, callback) {
    return fn(iterable, limit, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.filter"></a>[function <span class="apidocSignatureSpan">async.default.</span>filter (obj, iteratee, callback)](#apidoc.element.async.default.filter)
- description and source-code
```javascript
filter = function (obj, iteratee, callback) {
    return fn(eachOf, obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.filterLimit"></a>[function <span class="apidocSignatureSpan">async.default.</span>filterLimit (obj, limit, iteratee, callback)](#apidoc.element.async.default.filterLimit)
- description and source-code
```javascript
filterLimit = function (obj, limit, iteratee, callback) {
    return fn(_eachOfLimit(limit), obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.filterSeries"></a>[function <span class="apidocSignatureSpan">async.default.</span>filterSeries (iterable, iteratee, callback)](#apidoc.element.async.default.filterSeries)
- description and source-code
```javascript
filterSeries = function (iterable, iteratee, callback) {
    return fn(iterable, limit, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.foldl"></a>[function <span class="apidocSignatureSpan">async.default.</span>foldl (coll, memo, iteratee, callback)](#apidoc.element.async.default.foldl)
- description and source-code
```javascript
function reduce(coll, memo, iteratee, callback) {
    callback = once(callback || noop);
    eachOfSeries(coll, function (x, i, callback) {
        iteratee(memo, x, function (err, v) {
            memo = v;
            callback(err);
        });
    }, function (err) {
        callback(err, memo);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.foldr"></a>[function <span class="apidocSignatureSpan">async.default.</span>foldr (array, memo, iteratee, callback)](#apidoc.element.async.default.foldr)
- description and source-code
```javascript
function reduceRight(array, memo, iteratee, callback) {
  var reversed = slice.call(array).reverse();
  reduce(reversed, memo, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.forEach"></a>[function <span class="apidocSignatureSpan">async.default.</span>forEach (coll, iteratee, callback)](#apidoc.element.async.default.forEach)
- description and source-code
```javascript
function eachLimit(coll, iteratee, callback) {
  eachOf(coll, _withoutIndex(iteratee), callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.forEachLimit"></a>[function <span class="apidocSignatureSpan">async.default.</span>forEachLimit (coll, limit, iteratee, callback)](#apidoc.element.async.default.forEachLimit)
- description and source-code
```javascript
function eachLimit$1(coll, limit, iteratee, callback) {
  _eachOfLimit(limit)(coll, _withoutIndex(iteratee), callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.forEachOf"></a>[function <span class="apidocSignatureSpan">async.default.</span>forEachOf (coll, iteratee, callback)](#apidoc.element.async.default.forEachOf)
- description and source-code
```javascript
forEachOf = function (coll, iteratee, callback) {
    var eachOfImplementation = isArrayLike(coll) ? eachOfArrayLike : eachOfGeneric;
    eachOfImplementation(coll, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.forEachOfLimit"></a>[function <span class="apidocSignatureSpan">async.default.</span>forEachOfLimit (coll, limit, iteratee, callback)](#apidoc.element.async.default.forEachOfLimit)
- description and source-code
```javascript
function eachOfLimit(coll, limit, iteratee, callback) {
  _eachOfLimit(limit)(coll, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.forEachOfSeries"></a>[function <span class="apidocSignatureSpan">async.default.</span>forEachOfSeries (iterable, iteratee, callback)](#apidoc.element.async.default.forEachOfSeries)
- description and source-code
```javascript
forEachOfSeries = function (iterable, iteratee, callback) {
    return fn(iterable, limit, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.forEachSeries"></a>[function <span class="apidocSignatureSpan">async.default.</span>forEachSeries (iterable, iteratee, callback)](#apidoc.element.async.default.forEachSeries)
- description and source-code
```javascript
forEachSeries = function (iterable, iteratee, callback) {
    return fn(iterable, limit, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.forever"></a>[function <span class="apidocSignatureSpan">async.default.</span>forever (fn, errback)](#apidoc.element.async.default.forever)
- description and source-code
```javascript
function forever(fn, errback) {
    var done = onlyOnce(errback || noop);
    var task = ensureAsync(fn);

    function next(err) {
        if (err) return done(err);
        task(next);
    }
    next();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.inject"></a>[function <span class="apidocSignatureSpan">async.default.</span>inject (coll, memo, iteratee, callback)](#apidoc.element.async.default.inject)
- description and source-code
```javascript
function reduce(coll, memo, iteratee, callback) {
    callback = once(callback || noop);
    eachOfSeries(coll, function (x, i, callback) {
        iteratee(memo, x, function (err, v) {
            memo = v;
            callback(err);
        });
    }, function (err) {
        callback(err, memo);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.log"></a>[function <span class="apidocSignatureSpan">async.default.</span>log ()](#apidoc.element.async.default.log)
- description and source-code
```javascript
log = function () {
  var args = arguments,
      index = -1,
      length = nativeMax(args.length - start, 0),
      array = Array(length);

  while (++index < length) {
    array[index] = args[start + index];
  }
  index = -1;
  var otherArgs = Array(start + 1);
  while (++index < start) {
    otherArgs[index] = args[index];
  }
  otherArgs[start] = transform(array);
  return apply(func, this, otherArgs);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.map"></a>[function <span class="apidocSignatureSpan">async.default.</span>map (obj, iteratee, callback)](#apidoc.element.async.default.map)
- description and source-code
```javascript
map = function (obj, iteratee, callback) {
    return fn(eachOf, obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.mapLimit"></a>[function <span class="apidocSignatureSpan">async.default.</span>mapLimit (obj, limit, iteratee, callback)](#apidoc.element.async.default.mapLimit)
- description and source-code
```javascript
mapLimit = function (obj, limit, iteratee, callback) {
    return fn(_eachOfLimit(limit), obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.mapSeries"></a>[function <span class="apidocSignatureSpan">async.default.</span>mapSeries (iterable, iteratee, callback)](#apidoc.element.async.default.mapSeries)
- description and source-code
```javascript
mapSeries = function (iterable, iteratee, callback) {
    return fn(iterable, limit, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.mapValues"></a>[function <span class="apidocSignatureSpan">async.default.</span>mapValues (iterable, iteratee, callback)](#apidoc.element.async.default.mapValues)
- description and source-code
```javascript
mapValues = function (iterable, iteratee, callback) {
    return fn(iterable, limit, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.mapValuesLimit"></a>[function <span class="apidocSignatureSpan">async.default.</span>mapValuesLimit (obj, limit, iteratee, callback)](#apidoc.element.async.default.mapValuesLimit)
- description and source-code
```javascript
function mapValuesLimit(obj, limit, iteratee, callback) {
    callback = once(callback || noop);
    var newObj = {};
    eachOfLimit(obj, limit, function (val, key, next) {
        iteratee(val, key, function (err, result) {
            if (err) return next(err);
            newObj[key] = result;
            next();
        });
    }, function (err) {
        callback(err, newObj);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.mapValuesSeries"></a>[function <span class="apidocSignatureSpan">async.default.</span>mapValuesSeries (iterable, iteratee, callback)](#apidoc.element.async.default.mapValuesSeries)
- description and source-code
```javascript
mapValuesSeries = function (iterable, iteratee, callback) {
    return fn(iterable, limit, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.memoize"></a>[function <span class="apidocSignatureSpan">async.default.</span>memoize (fn, hasher)](#apidoc.element.async.default.memoize)
- description and source-code
```javascript
function memoize(fn, hasher) {
    var memo = Object.create(null);
    var queues = Object.create(null);
    hasher = hasher || identity;
    var memoized = initialParams(function memoized(args, callback) {
        var key = hasher.apply(null, args);
        if (has(memo, key)) {
            setImmediate$1(function () {
                callback.apply(null, memo[key]);
            });
        } else if (has(queues, key)) {
            queues[key].push(callback);
        } else {
            queues[key] = [callback];
            fn.apply(null, args.concat(rest(function (args) {
                memo[key] = args;
                var q = queues[key];
                delete queues[key];
                for (var i = 0, l = q.length; i < l; i++) {
                    q[i].apply(null, args);
                }
            })));
        }
    });
    memoized.memo = memo;
    memoized.unmemoized = fn;
    return memoized;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.nextTick"></a>[function <span class="apidocSignatureSpan">async.default.</span>nextTick ()](#apidoc.element.async.default.nextTick)
- description and source-code
```javascript
nextTick = function () {
  var args = arguments,
      index = -1,
      length = nativeMax(args.length - start, 0),
      array = Array(length);

  while (++index < length) {
    array[index] = args[start + index];
  }
  index = -1;
  var otherArgs = Array(start + 1);
  while (++index < start) {
    otherArgs[index] = args[index];
  }
  otherArgs[start] = transform(array);
  return apply(func, this, otherArgs);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.parallel"></a>[function <span class="apidocSignatureSpan">async.default.</span>parallel (tasks, callback)](#apidoc.element.async.default.parallel)
- description and source-code
```javascript
function parallelLimit(tasks, callback) {
  _parallel(eachOf, tasks, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.parallelLimit"></a>[function <span class="apidocSignatureSpan">async.default.</span>parallelLimit (tasks, limit, callback)](#apidoc.element.async.default.parallelLimit)
- description and source-code
```javascript
function parallelLimit$1(tasks, limit, callback) {
  _parallel(_eachOfLimit(limit), tasks, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.priorityQueue"></a>[function <span class="apidocSignatureSpan">async.default.</span>priorityQueue (worker, concurrency)](#apidoc.element.async.default.priorityQueue)
- description and source-code
```javascript
priorityQueue = function (worker, concurrency) {
    // Start with a normal queue
    var q = queue$1(worker, concurrency);

    // Override push to accept second parameter representing priority
    q.push = function (data, priority, callback) {
        if (callback == null) callback = noop;
        if (typeof callback !== 'function') {
            throw new Error('task callback must be a function');
        }
        q.started = true;
        if (!isArray(data)) {
            data = [data];
        }
        if (data.length === 0) {
            // call drain immediately if there are no tasks
            return setImmediate$1(function () {
                q.drain();
            });
        }

        priority = priority || 0;
        var nextNode = q._tasks.head;
        while (nextNode && priority >= nextNode.priority) {
            nextNode = nextNode.next;
        }

        for (var i = 0, l = data.length; i < l; i++) {
            var item = {
                data: data[i],
                priority: priority,
                callback: callback
            };

            if (nextNode) {
                q._tasks.insertBefore(nextNode, item);
            } else {
                q._tasks.push(item);
            }
        }
        setImmediate$1(q.process);
    };

    // Remove unshift function
    delete q.unshift;

    return q;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.queue"></a>[function <span class="apidocSignatureSpan">async.default.</span>queue (worker, concurrency)](#apidoc.element.async.default.queue)
- description and source-code
```javascript
queue = function (worker, concurrency) {
  return queue(function (items, cb) {
    worker(items[0], cb);
  }, concurrency, 1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.race"></a>[function <span class="apidocSignatureSpan">async.default.</span>race (tasks, callback)](#apidoc.element.async.default.race)
- description and source-code
```javascript
function race(tasks, callback) {
    callback = once(callback || noop);
    if (!isArray(tasks)) return callback(new TypeError('First argument to race must be an array of functions'));
    if (!tasks.length) return callback();
    for (var i = 0, l = tasks.length; i < l; i++) {
        tasks[i](callback);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.reduce"></a>[function <span class="apidocSignatureSpan">async.default.</span>reduce (coll, memo, iteratee, callback)](#apidoc.element.async.default.reduce)
- description and source-code
```javascript
function reduce(coll, memo, iteratee, callback) {
    callback = once(callback || noop);
    eachOfSeries(coll, function (x, i, callback) {
        iteratee(memo, x, function (err, v) {
            memo = v;
            callback(err);
        });
    }, function (err) {
        callback(err, memo);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.reduceRight"></a>[function <span class="apidocSignatureSpan">async.default.</span>reduceRight (array, memo, iteratee, callback)](#apidoc.element.async.default.reduceRight)
- description and source-code
```javascript
function reduceRight(array, memo, iteratee, callback) {
  var reversed = slice.call(array).reverse();
  reduce(reversed, memo, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.reflect"></a>[function <span class="apidocSignatureSpan">async.default.</span>reflect (fn)](#apidoc.element.async.default.reflect)
- description and source-code
```javascript
function reflect(fn) {
    return initialParams(function reflectOn(args, reflectCallback) {
        args.push(rest(function callback(err, cbArgs) {
            if (err) {
                reflectCallback(null, {
                    error: err
                });
            } else {
                var value = null;
                if (cbArgs.length === 1) {
                    value = cbArgs[0];
                } else if (cbArgs.length > 1) {
                    value = cbArgs;
                }
                reflectCallback(null, {
                    value: value
                });
            }
        }));

        return fn.apply(this, args);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.reflectAll"></a>[function <span class="apidocSignatureSpan">async.default.</span>reflectAll (tasks)](#apidoc.element.async.default.reflectAll)
- description and source-code
```javascript
function reflectAll(tasks) {
    var results;
    if (isArray(tasks)) {
        results = arrayMap(tasks, reflect);
    } else {
        results = {};
        baseForOwn(tasks, function (task, key) {
            results[key] = reflect.call(this, task);
        });
    }
    return results;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.reject"></a>[function <span class="apidocSignatureSpan">async.default.</span>reject (obj, iteratee, callback)](#apidoc.element.async.default.reject)
- description and source-code
```javascript
reject = function (obj, iteratee, callback) {
    return fn(eachOf, obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.rejectLimit"></a>[function <span class="apidocSignatureSpan">async.default.</span>rejectLimit (obj, limit, iteratee, callback)](#apidoc.element.async.default.rejectLimit)
- description and source-code
```javascript
rejectLimit = function (obj, limit, iteratee, callback) {
    return fn(_eachOfLimit(limit), obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.rejectSeries"></a>[function <span class="apidocSignatureSpan">async.default.</span>rejectSeries (iterable, iteratee, callback)](#apidoc.element.async.default.rejectSeries)
- description and source-code
```javascript
rejectSeries = function (iterable, iteratee, callback) {
    return fn(iterable, limit, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.retry"></a>[function <span class="apidocSignatureSpan">async.default.</span>retry (opts, task, callback)](#apidoc.element.async.default.retry)
- description and source-code
```javascript
function retry(opts, task, callback) {
    var DEFAULT_TIMES = 5;
    var DEFAULT_INTERVAL = 0;

    var options = {
        times: DEFAULT_TIMES,
        intervalFunc: constant$1(DEFAULT_INTERVAL)
    };

    function parseTimes(acc, t) {
        if (typeof t === 'object') {
            acc.times = +t.times || DEFAULT_TIMES;

            acc.intervalFunc = typeof t.interval === 'function' ? t.interval : constant$1(+t.interval || DEFAULT_INTERVAL);

            acc.errorFilter = t.errorFilter;
        } else if (typeof t === 'number' || typeof t === 'string') {
            acc.times = +t || DEFAULT_TIMES;
        } else {
            throw new Error("Invalid arguments for async.retry");
        }
    }

    if (arguments.length < 3 && typeof opts === 'function') {
        callback = task || noop;
        task = opts;
    } else {
        parseTimes(options, opts);
        callback = callback || noop;
    }

    if (typeof task !== 'function') {
        throw new Error("Invalid arguments for async.retry");
    }

    var attempt = 1;
    function retryAttempt() {
        task(function (err) {
            if (err && attempt++ < options.times && (typeof options.errorFilter != 'function' || options.errorFilter(err))) {
                setTimeout(retryAttempt, options.intervalFunc(attempt));
            } else {
                callback.apply(null, arguments);
            }
        });
    }

    retryAttempt();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.retryable"></a>[function <span class="apidocSignatureSpan">async.default.</span>retryable (opts, task)](#apidoc.element.async.default.retryable)
- description and source-code
```javascript
retryable = function (opts, task) {
    if (!task) {
        task = opts;
        opts = null;
    }
    return initialParams(function (args, callback) {
        function taskFn(cb) {
            task.apply(null, args.concat(cb));
        }

        if (opts) retry(opts, taskFn, callback);else retry(taskFn, callback);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.select"></a>[function <span class="apidocSignatureSpan">async.default.</span>select (obj, iteratee, callback)](#apidoc.element.async.default.select)
- description and source-code
```javascript
select = function (obj, iteratee, callback) {
    return fn(eachOf, obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.selectLimit"></a>[function <span class="apidocSignatureSpan">async.default.</span>selectLimit (obj, limit, iteratee, callback)](#apidoc.element.async.default.selectLimit)
- description and source-code
```javascript
selectLimit = function (obj, limit, iteratee, callback) {
    return fn(_eachOfLimit(limit), obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.selectSeries"></a>[function <span class="apidocSignatureSpan">async.default.</span>selectSeries (iterable, iteratee, callback)](#apidoc.element.async.default.selectSeries)
- description and source-code
```javascript
selectSeries = function (iterable, iteratee, callback) {
    return fn(iterable, limit, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.seq"></a>[function <span class="apidocSignatureSpan">async.default.</span>seq ()](#apidoc.element.async.default.seq)
- description and source-code
```javascript
seq = function () {
  var args = arguments,
      index = -1,
      length = nativeMax(args.length - start, 0),
      array = Array(length);

  while (++index < length) {
    array[index] = args[start + index];
  }
  index = -1;
  var otherArgs = Array(start + 1);
  while (++index < start) {
    otherArgs[index] = args[index];
  }
  otherArgs[start] = transform(array);
  return apply(func, this, otherArgs);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.series"></a>[function <span class="apidocSignatureSpan">async.default.</span>series (tasks, callback)](#apidoc.element.async.default.series)
- description and source-code
```javascript
function series(tasks, callback) {
  _parallel(eachOfSeries, tasks, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.setImmediate"></a>[function <span class="apidocSignatureSpan">async.default.</span>setImmediate ()](#apidoc.element.async.default.setImmediate)
- description and source-code
```javascript
setImmediate = function () {
  var args = arguments,
      index = -1,
      length = nativeMax(args.length - start, 0),
      array = Array(length);

  while (++index < length) {
    array[index] = args[start + index];
  }
  index = -1;
  var otherArgs = Array(start + 1);
  while (++index < start) {
    otherArgs[index] = args[index];
  }
  otherArgs[start] = transform(array);
  return apply(func, this, otherArgs);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.some"></a>[function <span class="apidocSignatureSpan">async.default.</span>some (obj, iteratee, callback)](#apidoc.element.async.default.some)
- description and source-code
```javascript
some = function (obj, iteratee, callback) {
    return fn(eachOf, obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.someLimit"></a>[function <span class="apidocSignatureSpan">async.default.</span>someLimit (obj, limit, iteratee, callback)](#apidoc.element.async.default.someLimit)
- description and source-code
```javascript
someLimit = function (obj, limit, iteratee, callback) {
    return fn(_eachOfLimit(limit), obj, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.someSeries"></a>[function <span class="apidocSignatureSpan">async.default.</span>someSeries (iterable, iteratee, callback)](#apidoc.element.async.default.someSeries)
- description and source-code
```javascript
someSeries = function (iterable, iteratee, callback) {
    return fn(iterable, limit, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.sortBy"></a>[function <span class="apidocSignatureSpan">async.default.</span>sortBy (coll, iteratee, callback)](#apidoc.element.async.default.sortBy)
- description and source-code
```javascript
function sortBy(coll, iteratee, callback) {
    map(coll, function (x, callback) {
        iteratee(x, function (err, criteria) {
            if (err) return callback(err);
            callback(null, { value: x, criteria: criteria });
        });
    }, function (err, results) {
        if (err) return callback(err);
        callback(null, arrayMap(results.sort(comparator), baseProperty('value')));
    });

    function comparator(left, right) {
        var a = left.criteria,
            b = right.criteria;
        return a < b ? -1 : a > b ? 1 : 0;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.timeout"></a>[function <span class="apidocSignatureSpan">async.default.</span>timeout (asyncFn, milliseconds, info)](#apidoc.element.async.default.timeout)
- description and source-code
```javascript
function timeout(asyncFn, milliseconds, info) {
    var originalCallback, timer;
    var timedOut = false;

    function injectedCallback() {
        if (!timedOut) {
            originalCallback.apply(null, arguments);
            clearTimeout(timer);
        }
    }

    function timeoutCallback() {
        var name = asyncFn.name || 'anonymous';
        var error = new Error('Callback function "' + name + '" timed out.');
        error.code = 'ETIMEDOUT';
        if (info) {
            error.info = info;
        }
        timedOut = true;
        originalCallback(error);
    }

    return initialParams(function (args, origCallback) {
        originalCallback = origCallback;
        // setup timer and call original function
        timer = setTimeout(timeoutCallback, milliseconds);
        asyncFn.apply(null, args.concat(injectedCallback));
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.times"></a>[function <span class="apidocSignatureSpan">async.default.</span>times (iterable, iteratee, callback)](#apidoc.element.async.default.times)
- description and source-code
```javascript
times = function (iterable, iteratee, callback) {
    return fn(iterable, limit, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.timesLimit"></a>[function <span class="apidocSignatureSpan">async.default.</span>timesLimit (count, limit, iteratee, callback)](#apidoc.element.async.default.timesLimit)
- description and source-code
```javascript
function timeLimit(count, limit, iteratee, callback) {
  mapLimit(baseRange(0, count, 1), limit, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.timesSeries"></a>[function <span class="apidocSignatureSpan">async.default.</span>timesSeries (iterable, iteratee, callback)](#apidoc.element.async.default.timesSeries)
- description and source-code
```javascript
timesSeries = function (iterable, iteratee, callback) {
    return fn(iterable, limit, iteratee, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.transform"></a>[function <span class="apidocSignatureSpan">async.default.</span>transform (coll, accumulator, iteratee, callback)](#apidoc.element.async.default.transform)
- description and source-code
```javascript
function transform(coll, accumulator, iteratee, callback) {
    if (arguments.length === 3) {
        callback = iteratee;
        iteratee = accumulator;
        accumulator = isArray(coll) ? [] : {};
    }
    callback = once(callback || noop);

    eachOf(coll, function (v, k, cb) {
        iteratee(accumulator, v, k, cb);
    }, function (err) {
        callback(err, accumulator);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.unmemoize"></a>[function <span class="apidocSignatureSpan">async.default.</span>unmemoize (fn)](#apidoc.element.async.default.unmemoize)
- description and source-code
```javascript
function unmemoize(fn) {
    return function () {
        return (fn.unmemoized || fn).apply(null, arguments);
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.until"></a>[function <span class="apidocSignatureSpan">async.default.</span>until (test, fn, callback)](#apidoc.element.async.default.until)
- description and source-code
```javascript
function until(test, fn, callback) {
    whilst(function () {
        return !test.apply(this, arguments);
    }, fn, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.waterfall"></a>[function <span class="apidocSignatureSpan">async.default.</span>waterfall (tasks, callback)](#apidoc.element.async.default.waterfall)
- description and source-code
```javascript
waterfall = function (tasks, callback) {
    callback = once(callback || noop);
    if (!isArray(tasks)) return callback(new Error('First argument to waterfall must be an array of functions'));
    if (!tasks.length) return callback();
    var taskIndex = 0;

    function nextTask(args) {
        if (taskIndex === tasks.length) {
            return callback.apply(null, [null].concat(args));
        }

        var taskCallback = onlyOnce(rest(function (err, args) {
            if (err) {
                return callback.apply(null, [err].concat(args));
            }
            nextTask(args);
        }));

        args.push(taskCallback);

        var task = tasks[taskIndex++];
        task.apply(null, args);
    }

    nextTask([]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.whilst"></a>[function <span class="apidocSignatureSpan">async.default.</span>whilst (test, iteratee, callback)](#apidoc.element.async.default.whilst)
- description and source-code
```javascript
function whilst(test, iteratee, callback) {
    callback = onlyOnce(callback || noop);
    if (!test()) return callback(null);
    var next = rest(function (err, args) {
        if (err) return callback(err);
        if (test()) return iteratee(next);
        callback.apply(null, [null].concat(args));
    });
    iteratee(next);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.async.default.wrapSync"></a>[function <span class="apidocSignatureSpan">async.default.</span>wrapSync (func)](#apidoc.element.async.default.wrapSync)
- description and source-code
```javascript
function asyncify(func) {
    return initialParams(function (args, callback) {
        var result;
        try {
            result = func.apply(this, args);
        } catch (e) {
            return callback(e);
        }
        // if result is Promise object
        if (isObject(result) && typeof result.then === 'function') {
            result.then(function (value) {
                callback(null, value);
            }, function (err) {
                callback(err.message ? err : new Error(err));
            });
        } else {
            callback(null, result);
        }
    });
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
