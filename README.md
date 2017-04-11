# test coverage for  [webpack-merge (v4.1.0)](https://github.com/survivejs/webpack-merge)  [![npm package](https://img.shields.io/npm/v/npmtest-webpack-merge.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-webpack-merge) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-webpack-merge.svg)](https://travis-ci.org/npmtest/node-npmtest-webpack-merge)
#### Variant of merge that's useful for webpack configuration

[![NPM](https://nodei.co/npm/webpack-merge.png?downloads=true)](https://www.npmjs.com/package/webpack-merge)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-webpack-merge/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-webpack-merge/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-webpack-merge/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-webpack-merge/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-webpack-merge/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-webpack-merge/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-webpack-merge/tree/gh-pages/build)|

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-webpack-merge/build/screenCapture.buildCustomOrg.browser.coverage.html.png)](https://npmtest.github.io/node-npmtest-webpack-merge/build/coverage.html/index.html)

[![test-report](https://npmtest.github.io/node-npmtest-webpack-merge/build/screenCapture.buildCustomOrg.browser.%252Fhome%252Ftravis%252Fbuild%252Fnpmtest%252Fnode-npmtest-webpack-merge%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-webpack-merge/build/test-report.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-webpack-merge/build/screenCapture.buildApidoc.browser.%252Fhome%252Ftravis%252Fbuild%252Fnpmdoc%252Fnode-npmdoc-webpack-merge%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-webpack-merge/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-webpack-merge/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-webpack-merge/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Juho Vepsalainen",
        "email": "bebraw@gmail.com"
    },
    "bugs": {
        "url": "https://github.com/survivejs/webpack-merge/issues"
    },
    "dependencies": {
        "lodash": "^4.17.4"
    },
    "description": "Variant of merge that's useful for webpack configuration",
    "devDependencies": {
        "babel-cli": "^6.18.0",
        "babel-plugin-lodash": "^3.2.11",
        "babel-preset-es2015": "^6.18.0",
        "copy-webpack-plugin": "^4.0.1",
        "eslint": "^3.13.1",
        "eslint-config-airbnb": "^14.0.0",
        "eslint-plugin-import": "^2.2.0",
        "eslint-plugin-jsx-a11y": "^3.0.2",
        "eslint-plugin-react": "^6.9.0",
        "git-prepush-hook": "^1.0.1",
        "istanbul": "^0.4.5",
        "mocha": "^3.2.0",
        "npm-watch": "^0.1.7",
        "webpack": "^1.14.0"
    },
    "directories": {},
    "dist": {
        "shasum": "6ad72223b3e0b837e531e4597c199f909361511e",
        "tarball": "https://registry.npmjs.org/webpack-merge/-/webpack-merge-4.1.0.tgz"
    },
    "files": [
        "lib"
    ],
    "gitHead": "d9559b9d28deecd1d7887aeef67a41180b66eb78",
    "homepage": "https://github.com/survivejs/webpack-merge",
    "keywords": [
        "webpack",
        "merge"
    ],
    "license": "MIT",
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "bebraw",
            "email": "bebraw@gmail.com"
        }
    ],
    "name": "webpack-merge",
    "optionalDependencies": {},
    "pre-push": [
        "test:lint",
        "build",
        "test"
    ],
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/survivejs/webpack-merge.git"
    },
    "scripts": {
        "build": "babel src -d lib",
        "preversion": "npm run test:lint && npm run build && npm test && git commit --allow-empty -am \"Update lib\"",
        "test": "mocha tests/test-*",
        "test:coverage": "istanbul cover node_modules/.bin/_mocha tests/test-*",
        "test:lint": "eslint src/ tests/ --cache",
        "watch": "npm-watch"
    },
    "version": "4.1.0",
    "watch": {
        "build": {
            "patterns": [
                "src/**/*.js"
            ]
        },
        "test": {
            "patterns": [
                "src/**/*.js",
                "tests/**/*.js"
            ]
        },
        "test:lint": {
            "patterns": [
                "src/**/*.js",
                "tests/**/*.js"
            ]
        }
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
