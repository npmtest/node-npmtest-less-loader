# npmtest-less-loader

#### basic test coverage for  [less-loader (v4.0.3)](https://github.com/webpack-contrib/less-loader#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-less-loader.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-less-loader) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-less-loader.svg)](https://travis-ci.org/npmtest/node-npmtest-less-loader)

#### Less loader for webpack. Compiles Less to CSS.

[![NPM](https://nodei.co/npm/less-loader.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/less-loader)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-less-loader/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-less-loader/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-less-loader/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-less-loader/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-less-loader/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-less-loader/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-less-loader/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-less-loader/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-less-loader/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-less-loader/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-less-loader/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-less-loader/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-less-loader/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-less-loader/build/test-report.html](https://npmtest.github.io/node-npmtest-less-loader/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-less-loader/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-less-loader/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-less-loader/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-less-loader/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-less-loader/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-less-loader/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-less-loader/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-less-loader/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Johannes Ewald @jhnns"
    },
    "bugs": {
        "url": "https://github.com/webpack-contrib/less-loader/issues"
    },
    "dependencies": {
        "clone": "^2.1.1",
        "loader-utils": "^1.1.0",
        "pify": "^2.3.0"
    },
    "description": "Less loader for webpack. Compiles Less to CSS.",
    "devDependencies": {
        "babel-cli": "^6.24.0",
        "babel-jest": "^19.0.0",
        "babel-plugin-transform-object-rest-spread": "^6.23.0",
        "babel-polyfill": "^6.23.0",
        "babel-preset-env": "^1.2.2",
        "cross-env": "^3.2.4",
        "del-cli": "^0.2.1",
        "eslint": "^3.18.0",
        "eslint-config-webpack": "^1.2.1",
        "eslint-plugin-import": "^2.2.0",
        "inspect-loader": "^1.0.0",
        "jest": "^19.0.2",
        "less": "^2.3.1",
        "lint-staged": "^3.4.0",
        "nodemon": "^1.11.0",
        "nsp": "^2.6.3",
        "pre-commit": "^1.2.2",
        "standard-version": "^4.0.0",
        "webpack": "^2.3.2",
        "webpack-defaults": "^0.4.5"
    },
    "directories": {},
    "dist": {
        "shasum": "d1e6462ca2f090c11248455e14b8dda4616d0521",
        "tarball": "https://registry.npmjs.org/less-loader/-/less-loader-4.0.3.tgz"
    },
    "engines": {
        "node": ">=4.3 <5.0.0 || >=5.10"
    },
    "files": [
        "README.md",
        "LICENSE",
        "dist"
    ],
    "gitHead": "e8b7d48a43ebbe82a818efa33efdb6fcf36c4a61",
    "homepage": "https://github.com/webpack-contrib/less-loader#readme",
    "license": "MIT",
    "lint-staged": {
        "*.js": [
            "eslint --fix",
            "git add"
        ]
    },
    "main": "dist/index.js",
    "maintainers": [
        {
            "name": "bebraw"
        },
        {
            "name": "d3viant0ne"
        },
        {
            "name": "ericclemmons"
        },
        {
            "name": "jhnns"
        },
        {
            "name": "sokra"
        },
        {
            "name": "thelarkinn"
        }
    ],
    "name": "less-loader",
    "optionalDependencies": {},
    "peerDependencies": {
        "less": "^2.3.1",
        "webpack": "^2.2.0"
    },
    "pre-commit": "lint-staged",
    "repository": {
        "type": "git",
        "url": "git://github.com/webpack-contrib/less-loader.git"
    },
    "scripts": {
        "appveyor:test": "npm test",
        "build": "cross-env NODE_ENV=production babel -s true src -d dist --ignore 'src/**/*.test.js'",
        "clean:dist": "del-cli dist",
        "create-spec": "babel-node test/helpers/createSpec.js",
        "lint": "eslint --cache src test",
        "lint-staged": "lint-staged",
        "posttest": "npm run lint",
        "prebuild": "yarn run clean:dist",
        "prepublish": "yarn run build",
        "pretest": "npm run create-spec",
        "release": "yarn run standard-version",
        "security": "nsp check",
        "serve:dev": "nodemon $2 --exec babel-node",
        "start": "yarn run serve:dev src",
        "test": "jest",
        "test:coverage": "jest --collectCoverageFrom='src/**/*.js' --coverage",
        "test:watch": "jest --watch",
        "travis:coverage": "yarn run test:coverage",
        "travis:lint": "yarn run lint && yarn run security",
        "travis:test": "yarn run test",
        "webpack-defaults": "webpack-defaults"
    },
    "version": "4.0.3",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
