# api documentation for  [deep-diff (v0.3.4)](https://github.com/flitbit/diff#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-deep-diff.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-deep-diff) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-deep-diff.svg)](https://travis-ci.org/npmdoc/node-npmdoc-deep-diff)
#### Javascript utility for calculating deep difference, capturing changes, and applying changes across objects; for nodejs and the browser.

[![NPM](https://nodei.co/npm/deep-diff.png?downloads=true)](https://www.npmjs.com/package/deep-diff)

[![apidoc](https://npmdoc.github.io/node-npmdoc-deep-diff/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-deep-diff_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-deep-diff/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-deep-diff/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-deep-diff/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Phillip Clark",
        "email": "phillip@flitbit.com"
    },
    "bugs": {
        "url": "https://github.com/flitbit/diff/issues"
    },
    "contributors": [
        {
            "name": "Dan Drinkard",
            "email": "dan.drinkard@gmail.com"
        },
        {
            "name": "Daniel Spangler",
            "email": "daniel.spangler@gmail.com"
        },
        {
            "name": "Denning",
            "email": "denningj@amazon.com"
        },
        {
            "name": "Elad Efrat",
            "email": "elad@iNNU.ORG"
        },
        {
            "name": "Mats Bryntse",
            "email": "mats.dev@bryntum.com"
        },
        {
            "name": "Nicholas Calugar",
            "email": "njcalugar@gmail.com"
        },
        {
            "name": "Paul Pflugradt",
            "email": "paulpflugradt@googlemail.com"
        },
        {
            "name": "Serkan Serttop",
            "email": "serkanserttop@yahoo.com"
        },
        {
            "name": "Simen Bekkhus",
            "email": "sbekkhus91@gmail.com"
        },
        {
            "name": "Tom Ashworth",
            "email": "tashworth@twitter.com"
        },
        {
            "name": "Tom MacWright",
            "email": "tmcw@users.noreply.github.com"
        },
        {
            "name": "Yandell",
            "email": "hyandell@amazon.com"
        },
        {
            "name": "ZauberNerd",
            "email": "zaubernerd@zaubernerd.de"
        },
        {
            "name": "caasi Huang",
            "email": "caasi.igd@gmail.com"
        },
        {
            "name": "icesoar",
            "email": "icesoar@hotmail.com"
        },
        {
            "name": "orlando",
            "email": "operri@opentable.com"
        },
        {
            "name": "ravishivt",
            "email": "javishi@gmail.com"
        },
        {
            "name": "wooorm",
            "email": "tituswormer@gmail.com"
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
        "uglifyjs": "^2.4.10"
    },
    "directories": {
        "examples": "./examples",
        "releases": "./releases",
        "test": "./test"
    },
    "dist": {
        "shasum": "aac5c39952236abe5f037a2349060ba01b00ae48",
        "tarball": "https://registry.npmjs.org/deep-diff/-/deep-diff-0.3.4.tgz"
    },
    "files": [
        "index.js",
        "releases/"
    ],
    "gitHead": "e271e69f4c6dbccf657cf30355d307b46659de67",
    "homepage": "https://github.com/flitbit/diff#readme",
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
            "name": "flitbit",
            "email": "phillip@flitbit.com"
        }
    ],
    "name": "deep-diff",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/flitbit/diff.git"
    },
    "scripts": {
        "pretest": "jscs index.js test/ && jshint index.js test/",
        "release": "uglifyjs index.js -o releases/deep-diff-$npm_package_version.min.js  -r '$,require,exports,module,window,global' -m  --comments '/^!/'",
        "test": "mocha"
    },
    "version": "0.3.4"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module deep-diff](#apidoc.module.deep-diff)
1.  [function <span class="apidocSignatureSpan">deep-diff.</span>applyChange (target, source, change)](#apidoc.element.deep-diff.applyChange)
1.  [function <span class="apidocSignatureSpan">deep-diff.</span>applyDiff (target, source, filter)](#apidoc.element.deep-diff.applyDiff)
1.  [function <span class="apidocSignatureSpan">deep-diff.</span>diff (lhs, rhs, prefilter, accum)](#apidoc.element.deep-diff.diff)
1.  [function <span class="apidocSignatureSpan">deep-diff.</span>isConflict ()](#apidoc.element.deep-diff.isConflict)
1.  [function <span class="apidocSignatureSpan">deep-diff.</span>noConflict ()](#apidoc.element.deep-diff.noConflict)
1.  [function <span class="apidocSignatureSpan">deep-diff.</span>observableDiff (lhs, rhs, changes, prefilter, path, key, stack)](#apidoc.element.deep-diff.observableDiff)
1.  [function <span class="apidocSignatureSpan">deep-diff.</span>revertChange (target, source, change)](#apidoc.element.deep-diff.revertChange)



# <a name="apidoc.module.deep-diff"></a>[module deep-diff](#apidoc.module.deep-diff)

#### <a name="apidoc.element.deep-diff.applyChange"></a>[function <span class="apidocSignatureSpan">deep-diff.</span>applyChange (target, source, change)](#apidoc.element.deep-diff.applyChange)
- description and source-code
```javascript
function applyChange(target, source, change) {
  if (target && source && change && change.kind) {
    var it = target,
        i = -1,
        last = change.path ? change.path.length - 1 : 0;
    while (++i < last) {
      if (typeof it[change.path[i]] === 'undefined') {
        it[change.path[i]] = (typeof change.path[i] === 'number') ? [] : {};
      }
      it = it[change.path[i]];
    }
    switch (change.kind) {
      case 'A':
        applyArrayChange(change.path ? it[change.path[i]] : it, change.index, change.item);
        break;
      case 'D':
        delete it[change.path[i]];
        break;
      case 'E':
      case 'N':
        it[change.path[i]] = change.rhs;
        break;
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.deep-diff.applyDiff"></a>[function <span class="apidocSignatureSpan">deep-diff.</span>applyDiff (target, source, filter)](#apidoc.element.deep-diff.applyDiff)
- description and source-code
```javascript
function applyDiff(target, source, filter) {
  if (target && source) {
    var onChange = function(change) {
      if (!filter || filter(target, source, change)) {
        applyChange(target, source, change);
      }
    };
    deepDiff(target, source, onChange);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.deep-diff.diff"></a>[function <span class="apidocSignatureSpan">deep-diff.</span>diff (lhs, rhs, prefilter, accum)](#apidoc.element.deep-diff.diff)
- description and source-code
```javascript
function accumulateDiff(lhs, rhs, prefilter, accum) {
  accum = accum || [];
  deepDiff(lhs, rhs,
    function(diff) {
      if (diff) {
        accum.push(diff);
      }
    },
    prefilter);
  return (accum.length) ? accum : undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.deep-diff.isConflict"></a>[function <span class="apidocSignatureSpan">deep-diff.</span>isConflict ()](#apidoc.element.deep-diff.isConflict)
- description and source-code
```javascript
isConflict = function () {
  return 'undefined' !== typeof conflict;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.deep-diff.noConflict"></a>[function <span class="apidocSignatureSpan">deep-diff.</span>noConflict ()](#apidoc.element.deep-diff.noConflict)
- description and source-code
```javascript
noConflict = function () {
  if (conflictResolution) {
    conflictResolution.forEach(function(it) {
      it();
    });
    conflictResolution = null;
  }
  return accumulateDiff;
}
```
- example usage
```shell
...
'''

**browser**
'''html
<script src="deep-diff-0.3.1.min.js"></script>
'''
> Minified, browser release of the current version of the module is under the 'releases' folder.
> In a browser, 'deep-diff' defines a global variable 'DeepDiff'. If there is a conflict in the global namesapce you can restore
 the conflicting definition and assign 'deep-diff' to another variable like this: 'var deep = DeepDiff.noConflict();'.

## Simple Examples

In order to describe differences, change revolves around an 'origin' object. For consistency, the 'origin' object is always the
operand on the 'left-hand-side' of operations. The 'comparand', which may contain changes, is always on the 'right-hand-side' of
 operations.

''' javascript
var diff = require('deep-diff').diff;
...
```

#### <a name="apidoc.element.deep-diff.observableDiff"></a>[function <span class="apidocSignatureSpan">deep-diff.</span>observableDiff (lhs, rhs, changes, prefilter, path, key, stack)](#apidoc.element.deep-diff.observableDiff)
- description and source-code
```javascript
function deepDiff(lhs, rhs, changes, prefilter, path, key, stack) {
  path = path || [];
  var currentPath = path.slice(0);
  if (typeof key !== 'undefined') {
    if (prefilter) {
      if (typeof(prefilter) === 'function' && prefilter(currentPath, key)) { return; }
      else if (typeof(prefilter) === 'object') {
        if (prefilter.prefilter && prefilter.prefilter(currentPath, key)) { return; }
        if (prefilter.normalize) {
          var alt = prefilter.normalize(currentPath, key, lhs, rhs);
          if (alt) {
            lhs = alt[0];
            rhs = alt[1];
          }
        }
      }
    }
    currentPath.push(key);
  }

  // Use string comparison for regexes
  if (realTypeOf(lhs) === 'regexp' && realTypeOf(rhs) === 'regexp') {
    lhs = lhs.toString();
    rhs = rhs.toString();
  }

  var ltype = typeof lhs;
  var rtype = typeof rhs;
  if (ltype === 'undefined') {
    if (rtype !== 'undefined') {
      changes(new DiffNew(currentPath, rhs));
    }
  } else if (rtype === 'undefined') {
    changes(new DiffDeleted(currentPath, lhs));
  } else if (realTypeOf(lhs) !== realTypeOf(rhs)) {
    changes(new DiffEdit(currentPath, lhs, rhs));
  } else if (Object.prototype.toString.call(lhs) === '[object Date]' && Object.prototype.toString.call(rhs) === '[object Date]' && ((
lhs - rhs) !== 0)) {
    changes(new DiffEdit(currentPath, lhs, rhs));
  } else if (ltype === 'object' && lhs !== null && rhs !== null) {
    stack = stack || [];
    if (stack.indexOf(lhs) < 0) {
      stack.push(lhs);
      if (Array.isArray(lhs)) {
        var i, len = lhs.length;
        for (i = 0; i < lhs.length; i++) {
          if (i >= rhs.length) {
            changes(new DiffArray(currentPath, i, new DiffDeleted(undefined, lhs[i])));
          } else {
            deepDiff(lhs[i], rhs[i], changes, prefilter, currentPath, i, stack);
          }
        }
        while (i < rhs.length) {
          changes(new DiffArray(currentPath, i, new DiffNew(undefined, rhs[i++])));
        }
      } else {
        var akeys = Object.keys(lhs);
        var pkeys = Object.keys(rhs);
        akeys.forEach(function(k, i) {
          var other = pkeys.indexOf(k);
          if (other >= 0) {
            deepDiff(lhs[k], rhs[k], changes, prefilter, currentPath, k, stack);
            pkeys = arrayRemove(pkeys, other);
          } else {
            deepDiff(lhs[k], undefined, changes, prefilter, currentPath, k, stack);
          }
        });
        pkeys.forEach(function(k) {
          deepDiff(undefined, rhs[k], changes, prefilter, currentPath, k, stack);
        });
      }
      stack.length = stack.length - 1;
    }
  } else if (lhs !== rhs) {
    if (!(ltype === 'number' && isNaN(lhs) && isNaN(rhs))) {
      changes(new DiffEdit(currentPath, lhs, rhs));
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.deep-diff.revertChange"></a>[function <span class="apidocSignatureSpan">deep-diff.</span>revertChange (target, source, change)](#apidoc.element.deep-diff.revertChange)
- description and source-code
```javascript
function revertChange(target, source, change) {
  if (target && source && change && change.kind) {
    var it = target,
        i, u;
    u = change.path.length - 1;
    for (i = 0; i < u; i++) {
      if (typeof it[change.path[i]] === 'undefined') {
        it[change.path[i]] = {};
      }
      it = it[change.path[i]];
    }
    switch (change.kind) {
      case 'A':
        // Array was modified...
        // it will be an array...
        revertArrayChange(it[change.path[i]], change.index, change.item);
        break;
      case 'D':
        // Item was deleted...
        it[change.path[i]] = change.lhs;
        break;
      case 'E':
        // Item was edited...
        it[change.path[i]] = change.lhs;
        break;
      case 'N':
        // Item is new...
        delete it[change.path[i]];
        break;
    }
  }
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
