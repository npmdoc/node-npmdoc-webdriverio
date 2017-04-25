# npmdoc-webdriverio

#### basic api documentation for  [webdriverio (v4.7.1)](http://webdriver.io)  [![npm package](https://img.shields.io/npm/v/npmdoc-webdriverio.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-webdriverio) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-webdriverio.svg)](https://travis-ci.org/npmdoc/node-npmdoc-webdriverio)

#### A nodejs bindings implementation for selenium 2.0/webdriver

[![NPM](https://nodei.co/npm/webdriverio.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/webdriverio)

- [https://npmdoc.github.io/node-npmdoc-webdriverio/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-webdriverio/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-webdriverio/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-webdriverio/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-webdriverio/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-webdriverio/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Camilo Tapia"
    },
    "bin": {
        "wdio": "bin/wdio"
    },
    "bugs": {
        "url": "https://github.com/webdriverio/webdriverio/issues"
    },
    "dependencies": {
        "archiver": "~1.3.0",
        "babel-runtime": "~6.23.0",
        "css-parse": "~2.0.0",
        "css-value": "~0.0.1",
        "deepmerge": "~1.3.2",
        "ejs": "~2.5.6",
        "gaze": "~1.1.2",
        "glob": "~7.1.1",
        "inquirer": "~3.0.6",
        "json-stringify-safe": "~5.0.1",
        "mkdirp": "~0.5.1",
        "npm-install-package": "~2.1.0",
        "optimist": "~0.6.1",
        "q": "~1.5.0",
        "request": "~2.81.0",
        "rgb2hex": "~0.1.0",
        "safe-buffer": "~5.0.1",
        "supports-color": "~3.2.3",
        "url": "~0.11.0",
        "validator": "~7.0.0",
        "wdio-dot-reporter": "~0.0.8",
        "wgxpath": "~1.0.0"
    },
    "description": "A nodejs bindings implementation for selenium 2.0/webdriver",
    "devDependencies": {
        "babel-cli": "^6.24.1",
        "babel-core": "^6.24.1",
        "babel-eslint": "^7.2.1",
        "babel-plugin-add-module-exports": "^0.2.1",
        "babel-plugin-transform-runtime": "^6.23.0",
        "babel-preset-env": "^1.3.3",
        "babel-preset-stage-0": "^6.24.1",
        "babel-register": "^6.24.1",
        "chai": "^3.5.0",
        "chai-as-promised": "^6.0.0",
        "chai-string": "^1.3.0",
        "chai-things": "^0.2.0",
        "codeclimate-test-reporter": "^0.4.1",
        "cordova": "^6.5.0",
        "coveralls": "^2.13.0",
        "eslint": "^3.19.0",
        "eslint-config-standard": "^10.2.1",
        "eslint-plugin-chai-expect": "^1.1.1",
        "eslint-plugin-import": "^2.2.0",
        "eslint-plugin-mocha": "^4.9.0",
        "eslint-plugin-node": "^4.2.2",
        "eslint-plugin-promise": "^3.5.0",
        "eslint-plugin-standard": "^3.0.1",
        "isparta": "^4.0.0",
        "istanbul": "^0.4.5",
        "mocha": "^3.2.0",
        "mock-require": "^2.0.2",
        "nock": "^9.0.13",
        "node-static": "^0.7.9",
        "np": "2.13.2",
        "npm-run-all": "^4.0.2",
        "sauce-connect-launcher": "^1.2.1",
        "saucelabs": "^1.4.0",
        "sinon": "^2.1.0",
        "snyk": "^1.28.0",
        "wdio-mocha-framework": "^0.5.9"
    },
    "directories": {},
    "dist": {
        "shasum": "2248d1c6a2e05a89c840d4d62e9e550997a43854",
        "tarball": "https://registry.npmjs.org/webdriverio/-/webdriverio-4.7.1.tgz"
    },
    "engines": {
        "node": ">= 0.12.0"
    },
    "gitHead": "a611b804cb39a6fe134091acf895f72794d11429",
    "homepage": "http://webdriver.io",
    "keywords": [
        "webdriverio",
        "webdriver",
        "selenium",
        "appium",
        "saucelabs",
        "sauce",
        "labs",
        "mocha",
        "nodeUnit",
        "buster",
        "phantomjs",
        "chai",
        "vows",
        "jasmine",
        "assert",
        "cucumber",
        "testingbot"
    ],
    "license": "MIT",
    "main": "./build/index.js",
    "maintainers": [
        {
            "name": "christian-bromann"
        },
        {
            "name": "georgecrawfordft"
        }
    ],
    "name": "webdriverio",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/webdriverio/webdriverio.git"
    },
    "scripts": {
        "build": "run-s clean compile copy",
        "clean": "run-p clean:*",
        "clean:android": "rm -fr test/site/platforms/android",
        "clean:build": "rm -fr build",
        "clean:cordova": "rm -fr test/site/platforms test/site/plugins",
        "clean:coverage": "rm -fr coverage",
        "clean:ios": "rm -fr test/site/platforms/ios",
        "compile": "run-p compile:*",
        "compile:index": "mkdir -p build && babel index.js --out-file build/index.js",
        "compile:lib": "babel lib/ -d build/lib",
        "copy": "run-p copy:*",
        "copy:ejstemplate": "cp lib/helpers/wdio.conf.ejs build/lib/helpers/wdio.conf.ejs",
        "copy:packagejson": "cp package.json build",
        "cordova": "npm-run-all cordova:add_platforms --parallel cordova:compile:*",
        "cordova:add_platforms": "cd ./test/site && cordova platform add ios android && cd ../../",
        "cordova:compile:android": "cd ./test/site && cordova build android && cd ../../",
        "cordova:compile:ios": "cd ./test/site && cordova build ios && cd ../../",
        "eslint": "eslint ./lib test/",
        "prepublish": "npm prune",
        "release": "np patch",
        "release:major": "np major",
        "release:minor": "np minor",
        "release:patch": "np patch",
        "test": "run-s eslint test:unit",
        "test:android": "mocha test/setup.js test/spec/mobile/*.js test/spec/mobile/android/*.js",
        "test:ci": "run-s eslint build test:$_ENV",
        "test:cover": "babel-node ./node_modules/.bin/isparta cover --include 'lib/*.js' _mocha",
        "test:desktop": "mocha test/setup.js test/spec/*.js test/spec/desktop/*.js",
        "test:functional": "mocha test/setup.js test/spec/functional/**/*.js",
        "test:ios": "mocha test/setup.js test/spec/mobile/*.js test/spec/mobile/ios/*.js",
        "test:multibrowser": "mocha test/setup.js test/spec/multibrowser/**/*.js",
        "test:snyk": "snyk auth $SNYK_AUTH_TOKEN && snyk test",
        "test:unit": "mocha test/setup-unit.js test/spec/unit/*.js",
        "test:wdio": "mocha test/setup-unit.js test/spec/wdio/*.js",
        "watch": "npm run compile:lib -- --watch"
    },
    "tags": [
        "webdriver",
        "selenium",
        "test",
        "automation",
        "browser",
        "javascript",
        "node"
    ],
    "version": "4.7.1"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
