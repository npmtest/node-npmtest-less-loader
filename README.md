# npmtest-less-loader

#### basic test coverage for  less-loader (v4.0.3)  [![npm package](https://img.shields.io/npm/v/npmtest-less-loader.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-less-loader) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-less-loader.svg)](https://travis-ci.org/npmtest/node-npmtest-less-loader)

#### Less loader for webpack. Compiles Less to CSS.

[![NPM](https://nodei.co/npm/less-loader.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/less-loader)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-less-loader/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-less-loader/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-less-loader/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-less-loader/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-less-loader/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-less-loader/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-less-loader/tree/gh-pages/build)|

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
    "name": "less-loader",
    "version": "4.0.3",
    "author": "Johannes Ewald @jhnns",
    "description": "Less loader for webpack. Compiles Less to CSS.",
    "main": "dist/index.js",
    "scripts": {
        "create-spec": "babel-node test/helpers/createSpec.js",
        "pretest": "npm run create-spec",
        "test": "jest",
        "posttest": "npm run lint",
        "travis:test": "yarn run test",
        "appveyor:test": "npm test",
        "lint": "eslint --cache src test",
        "webpack-defaults": "webpack-defaults",
        "start": "yarn run serve:dev src",
        "build": "cross-env NODE_ENV=production babel -s true src -d dist --ignore 'src/**/*.test.js'",
        "clean:dist": "del-cli dist",
        "lint-staged": "lint-staged",
        "prebuild": "yarn run clean:dist",
        "prepublish": "yarn run build",
        "release": "yarn run standard-version",
        "security": "nsp check",
        "serve:dev": "nodemon $2 --exec babel-node",
        "test:watch": "jest --watch",
        "test:coverage": "jest --collectCoverageFrom='src/**/*.js' --coverage",
        "travis:coverage": "yarn run test:coverage",
        "travis:lint": "yarn run lint && yarn run security"
    },
    "engines": {
        "node": ">=4.3 <5.0.0 || >=5.10"
    },
    "dependencies": {
        "clone": "^2.1.1",
        "loader-utils": "^1.1.0",
        "pify": "^2.3.0"
    },
    "peerDependencies": {
        "less": "^2.3.1",
        "webpack": "^2.2.0"
    },
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
    "repository": {
        "type": "git",
        "url": "git://github.com/webpack-contrib/less-loader.git"
    },
    "license": "MIT",
    "files": [
        "README.md",
        "LICENSE",
        "dist"
    ],
    "pre-commit": "lint-staged",
    "lint-staged": {
        "*.js": [
            "eslint --fix",
            "git add"
        ]
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
