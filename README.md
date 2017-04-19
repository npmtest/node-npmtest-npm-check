# npmtest-npm-check

#### basic test coverage for  [npm-check (v5.4.0)](https://github.com/dylang/npm-check)  [![npm package](https://img.shields.io/npm/v/npmtest-npm-check.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-npm-check) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-npm-check.svg)](https://travis-ci.org/npmtest/node-npmtest-npm-check)

#### Check for outdated, incorrect, and unused dependencies.

[![NPM](https://nodei.co/npm/npm-check.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/npm-check)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-npm-check/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-npm-check/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-npm-check/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-npm-check/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-npm-check/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-npm-check/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-npm-check/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-npm-check/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-npm-check/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-npm-check/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-npm-check/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-npm-check/build/test-report.html](https://npmtest.github.io/node-npmtest-npm-check/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-npm-check/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-npm-check/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-npm-check/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-npm-check/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-npm-check/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-npm-check/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-npm-check/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-npm-check/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Dylan Greene"
    },
    "bin": {
        "npm-check": "bin/cli.js"
    },
    "bugs": {
        "url": "https://github.com/dylang/npm-check/issues"
    },
    "dependencies": {
        "babel-runtime": "^6.6.1",
        "callsite-record": "^3.0.0",
        "chalk": "^1.1.3",
        "co": "^4.6.0",
        "depcheck": "^0.6.3",
        "execa": "^0.2.2",
        "giturl": "^1.0.0",
        "global-modules": "^0.2.0",
        "globby": "^4.0.0",
        "inquirer": "^0.12.0",
        "is-ci": "^1.0.8",
        "lodash": "^4.7.0",
        "meow": "^3.7.0",
        "merge-options": "0.0.64",
        "minimatch": "^3.0.2",
        "node-emoji": "^1.0.3",
        "ora": "^0.2.1",
        "package-json": "^2.0.1",
        "path-exists": "^2.1.0",
        "pkg-dir": "^1.0.0",
        "semver": "^5.0.1",
        "semver-diff": "^2.0.0",
        "text-table": "^0.2.0",
        "throat": "^2.0.2",
        "update-notifier": "^0.6.3"
    },
    "description": "Check for outdated, incorrect, and unused dependencies.",
    "devDependencies": {
        "babel-cli": "^6.6.5",
        "babel-plugin-transform-runtime": "^6.6.0",
        "babel-preset-es2015": "^6.6.0",
        "grunt": "^0.4.0",
        "grunt-cli": "^1.2.0",
        "grunt-release": "^0.13.0",
        "grunt-templates-dylang": "^1.0.9",
        "load-grunt-tasks": "^3.3.0",
        "xo": "^0.13.0"
    },
    "directories": {},
    "dist": {
        "shasum": "21f537e474616458beaccd6ecfc9f73f246ee7bd",
        "tarball": "https://registry.npmjs.org/npm-check/-/npm-check-5.4.0.tgz"
    },
    "engines": {
        "node": ">=0.11.0"
    },
    "files": [
        "bin",
        "lib",
        "lib-es5"
    ],
    "gitHead": "ee416b8a20742e81cd848aaace1ce328e070f8f2",
    "homepage": "https://github.com/dylang/npm-check",
    "keywords": [
        "npm",
        "outdated",
        "dependencies",
        "unused",
        "changelog",
        "check",
        "updates",
        "api",
        "interactive",
        "cli",
        "safe",
        "updating",
        "updater",
        "installer",
        "devDependencies"
    ],
    "license": "MIT",
    "main": "lib",
    "maintainers": [
        {
            "name": "dylang"
        },
        {
            "name": "linusu"
        }
    ],
    "name": "npm-check",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/dylang/npm-check.git"
    },
    "scripts": {
        "lint": "xo ./lib/*.js",
        "prepublish": "npm run transpile",
        "readme": "grunt readme",
        "repos": "grunt repos # required for grunt readme to run",
        "test": "xo ./lib/*.js && ./bin/cli.js || echo Exit Status: $?.",
        "transpile": "babel lib --out-dir lib-es5",
        "watch": "babel lib --out-dir lib-es5 --watch"
    },
    "version": "5.4.0",
    "xo": {
        "space": 4,
        "rules": {
            "no-warning-comments": [
                0
            ],
            "global-require": [
                0
            ]
        }
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
