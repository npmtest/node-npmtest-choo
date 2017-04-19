# npmtest-choo

#### test coverage for  [choo (v5.1.5)](https://github.com/yoshuawuyts/choo#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-choo.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-choo) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-choo.svg)](https://travis-ci.org/npmtest/node-npmtest-choo)

#### A 4kb framework for creating sturdy frontend applications

[![NPM](https://nodei.co/npm/choo.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/choo)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-choo/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-choo/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-choo/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-choo/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-choo/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-choo/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-choo/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-choo/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-choo/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-choo/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-choo/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-choo/build/test-report.html](https://npmtest.github.io/node-npmtest-choo/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-choo/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-choo/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-choo/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-choo/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-choo/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-choo/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-choo/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-choo/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "bugs": {
        "url": "https://github.com/yoshuawuyts/choo/issues"
    },
    "dependencies": {
        "bel": "^4.5.1",
        "document-ready": "^2.0.1",
        "nanobus": "^3.0.0",
        "nanohistory": "^1.0.0",
        "nanohref": "^1.0.0",
        "nanomorph": "^4.0.0",
        "nanomount": "^1.0.0",
        "nanoraf": "^3.0.0",
        "nanorouter": "^2.0.0"
    },
    "description": "A 4kb framework for creating sturdy frontend applications",
    "devDependencies": {
        "browserify": "^14.3.0",
        "bundle-collapser": "^1.2.1",
        "dependency-check": "^2.8.0",
        "discify": "^1.6.0",
        "node-zopfli": "^2.0.2",
        "pretty-bytes-cli": "^2.0.0",
        "spok": "^0.8.1",
        "standard": "^10.0.0",
        "tape": "^4.6.3",
        "uglifyify": "^3.0.4",
        "uglifyjs": "^2.4.10",
        "unassertify": "^2.0.4"
    },
    "directories": {},
    "dist": {
        "shasum": "c3c0886c4ecfb40eb7e2b5d43ba18060c9f8011a",
        "tarball": "https://registry.npmjs.org/choo/-/choo-5.1.5.tgz"
    },
    "gitHead": "2cdf2dcdf0dc5ec47f06f30f0dfd3eff89e64751",
    "homepage": "https://github.com/yoshuawuyts/choo#readme",
    "keywords": [
        "client",
        "frontend",
        "framework",
        "minimal",
        "composable",
        "tiny"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "ahdinosaur"
        },
        {
            "name": "maxogden"
        },
        {
            "name": "sethvincent"
        },
        {
            "name": "timwis"
        },
        {
            "name": "toddself"
        },
        {
            "name": "yoshuawuyts"
        }
    ],
    "name": "choo",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/yoshuawuyts/choo.git"
    },
    "scripts": {
        "build": "mkdir -p dist/ && browserify index -p bundle-collapser/plugin > dist/bundle.js && browserify index -g unassertify -g uglifyify -p bundle-collapser/plugin | uglifyjs > dist/bundle.min.js && zopfli -i 100 dist/bundle.min.js && wc -c < dist/bundle.min.js.gz | pretty-bytes",
        "deps": "dependency-check --entry ./html.js . && dependency-check . --extra --no-dev --entry ./html.js",
        "inspect": "browserify --full-paths index -g unassertify -g uglifyify | discify --open",
        "prepublish": "npm run build",
        "start": "bankai start example --optimize",
        "test": "standard && npm run deps && node test.js"
    },
    "version": "5.1.5"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
