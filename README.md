# npmdoc-deep-diff

#### basic api documentation for  [deep-diff (v0.3.6)](https://github.com/flitbit/diff#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-deep-diff.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-deep-diff) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-deep-diff.svg)](https://travis-ci.org/npmdoc/node-npmdoc-deep-diff)

#### Javascript utility for calculating deep difference, capturing changes, and applying changes across objects; for nodejs and the browser.

[![NPM](https://nodei.co/npm/deep-diff.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/deep-diff)

- [https://npmdoc.github.io/node-npmdoc-deep-diff/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-deep-diff/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-deep-diff/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-deep-diff/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-deep-diff/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-deep-diff/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Phillip Clark"
    },
    "bugs": {
        "url": "https://github.com/flitbit/diff/issues"
    },
    "contributors": [
        {
            "name": "Simen Bekkhus"
        },
        {
            "name": "Paul Pflugradt"
        },
        {
            "name": "wooorm"
        },
        {
            "name": "Nicholas Calugar"
        },
        {
            "name": "Yandell"
        },
        {
            "name": "Thiago Santos"
        },
        {
            "name": "Steve Mao"
        },
        {
            "name": "Mats Bryntse"
        },
        {
            "name": "Phillip Clark"
        },
        {
            "name": "ZauberNerd"
        },
        {
            "name": "ravishivt"
        },
        {
            "name": "Daniel Spangler"
        },
        {
            "name": "Thomas de Barochez"
        },
        {
            "name": "Morton Fox"
        },
        {
            "name": "Amila Welihinda"
        },
        {
            "name": "Will Biddy"
        },
        {
            "name": "icesoar"
        },
        {
            "name": "Serkan Serttop"
        },
        {
            "name": "orlando"
        },
        {
            "name": "Tom MacWright"
        },
        {
            "name": "Denning"
        },
        {
            "name": "Dan Drinkard"
        },
        {
            "name": "Elad Efrat"
        },
        {
            "name": "caasi Huang"
        },
        {
            "name": "Tom Ashworth"
        }
    ],
    "dependencies": {},
    "description": "Javascript utility for calculating deep difference, capturing changes, and applying changes across objects; for nodejs and the browser.",
    "devDependencies": {
        "deep-equal": "~1.0.0",
        "expect.js": "^0.3.1",
        "jscs": "^1.12.0",
        "jshint": "^2.6.3",
        "mocha": "^2.2.1",
        "rollup": "^0.41.6",
        "uglifyjs": "^2.4.10"
    },
    "directories": {
        "examples": "./examples",
        "releases": "./releases",
        "test": "./test"
    },
    "dist": {
        "shasum": "9134a91ded42ea25b9ebe192c93ac6f4ec2e6c9a",
        "tarball": "https://registry.npmjs.org/deep-diff/-/deep-diff-0.3.6.tgz"
    },
    "files": [
        "index.js",
        "index.es.js",
        "releases/"
    ],
    "gitHead": "f7df1a4eba06c8ce492f9bd7e3aeba7e18b8db82",
    "homepage": "https://github.com/flitbit/diff#readme",
    "jsnext:main": "/index.es.js",
    "keywords": [
        "diff",
        "difference",
        "compare",
        "change-tracking"
    ],
    "license": "MIT",
    "main": "./index.js",
    "maintainers": [
        {
            "name": "flitbit"
        }
    ],
    "module": "./index.es.js",
    "name": "deep-diff",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/flitbit/diff.git"
    },
    "scripts": {
        "build": "rollup index.es.js -f umd -o index.js -n DeepDiff",
        "pretest": "jscs index.es.js test/ -e && jshint index.es.js test/",
        "release": "uglifyjs index.js -o releases/deep-diff-$npm_package_version.min.js  -r '$,require,exports,module,window,global' -m  --comments '/^!/'",
        "test": "mocha"
    },
    "version": "0.3.6",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
