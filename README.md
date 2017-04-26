# npmtest-runjs

#### basic test coverage for  [runjs (v3.2.1)](https://github.com/pawelgalazka/runjs#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-runjs.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-runjs) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-runjs.svg)](https://travis-ci.org/npmtest/node-npmtest-runjs)

#### Minimalistic building tool

[![NPM](https://nodei.co/npm/runjs.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/runjs)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-runjs/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-runjs/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-runjs/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-runjs/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-runjs/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-runjs/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-runjs/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-runjs/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-runjs/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-runjs/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-runjs/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-runjs/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-runjs/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-runjs/build/test-report.html](https://npmtest.github.io/node-npmtest-runjs/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-runjs/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-runjs/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-runjs/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-runjs/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-runjs/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-runjs/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-runjs/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-runjs/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Pawel Galazka"
    },
    "babel": {
        "presets": [
            "es2015"
        ]
    },
    "bin": {
        "run": "bin/run.js"
    },
    "bugs": {
        "url": "https://github.com/pawelgalazka/runjs/issues"
    },
    "dependencies": {
        "chalk": "1.1.3",
        "get-parameter-names": "0.3.0",
        "lodash.template": "4.4.0"
    },
    "description": "Minimalistic building tool",
    "devDependencies": {
        "babel-cli": "6.16.0",
        "babel-core": "6.16.0",
        "babel-eslint": "7.0.0",
        "babel-jest": "16.0.0",
        "babel-preset-es2015": "6.16.0",
        "babel-register": "6.16.3",
        "eslint": "3.6.1",
        "eslint-config-standard": "6.2.0",
        "eslint-plugin-promise": "2.0.1",
        "eslint-plugin-standard": "2.0.1",
        "jest": "16.0.2"
    },
    "directories": {},
    "dist": {
        "shasum": "c84d9cbaaf7a6e7958888bac45101fc809506d28",
        "tarball": "https://registry.npmjs.org/runjs/-/runjs-3.2.1.tgz"
    },
    "engines": {
        "node": ">=4.8.0"
    },
    "eslintConfig": {
        "extends": [
            "eslint-config-standard"
        ],
        "parser": "babel-eslint"
    },
    "gitHead": "cf44efc4372fb8651bfb893e977d4cfa591ef131",
    "homepage": "https://github.com/pawelgalazka/runjs#readme",
    "keywords": [
        "build",
        "system",
        "make",
        "tool"
    ],
    "license": "MIT",
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "pawelgalazka"
        }
    ],
    "name": "runjs",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/pawelgalazka/runjs.git"
    },
    "scripts": {
        "build": "babel src/ --out-dir lib/",
        "clean": "rm -rf node_modules && rm -rf test/sandbox/node_modules",
        "lint": "eslint src/ bin/ test/*.test.js",
        "test": "npm run test:fast && npm run test:e2e",
        "test:e2e": "bash ./test/e2e.test.sh",
        "test:fast": "npm run lint && npm run build && jest"
    },
    "version": "3.2.1"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
