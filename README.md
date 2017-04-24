# npmdoc-send

#### api documentation for  [send (v0.15.1)](https://github.com/pillarjs/send#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-send.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-send) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-send.svg)](https://travis-ci.org/npmdoc/node-npmdoc-send)

#### Better streaming static file server with Range and conditional-GET support

[![NPM](https://nodei.co/npm/send.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/send)

- [https://npmdoc.github.io/node-npmdoc-send/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-send/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-send/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-send/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-send/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-send/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "TJ Holowaychuk"
    },
    "bugs": {
        "url": "https://github.com/pillarjs/send/issues"
    },
    "contributors": [
        {
            "name": "Douglas Christopher Wilson"
        },
        {
            "name": "James Wyatt Cready"
        },
        {
            "name": "Jesús Leganés Combarro"
        }
    ],
    "dependencies": {
        "debug": "2.6.1",
        "depd": "~1.1.0",
        "destroy": "~1.0.4",
        "encodeurl": "~1.0.1",
        "escape-html": "~1.0.3",
        "etag": "~1.8.0",
        "fresh": "0.5.0",
        "http-errors": "~1.6.1",
        "mime": "1.3.4",
        "ms": "0.7.2",
        "on-finished": "~2.3.0",
        "range-parser": "~1.2.0",
        "statuses": "~1.3.1"
    },
    "description": "Better streaming static file server with Range and conditional-GET support",
    "devDependencies": {
        "after": "0.8.2",
        "eslint": "3.17.0",
        "eslint-config-standard": "7.0.0",
        "eslint-plugin-markdown": "1.0.0-beta.4",
        "eslint-plugin-promise": "3.5.0",
        "eslint-plugin-standard": "2.1.1",
        "istanbul": "0.4.5",
        "mocha": "2.5.3",
        "supertest": "1.1.0"
    },
    "directories": {},
    "dist": {
        "shasum": "8a02354c26e6f5cca700065f5f0cdeba90ec7b5f",
        "tarball": "https://registry.npmjs.org/send/-/send-0.15.1.tgz"
    },
    "engines": {
        "node": ">= 0.8.0"
    },
    "files": [
        "HISTORY.md",
        "LICENSE",
        "README.md",
        "index.js"
    ],
    "gitHead": "ea1748a3b3e00dbcbb0629cf368ced575c6ab7d6",
    "homepage": "https://github.com/pillarjs/send#readme",
    "keywords": [
        "static",
        "file",
        "server"
    ],
    "license": "MIT",
    "maintainers": [
        {
            "name": "dougwilson"
        }
    ],
    "name": "send",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/pillarjs/send.git"
    },
    "scripts": {
        "lint": "eslint --plugin markdown --ext js,md .",
        "test": "mocha --check-leaks --reporter spec --bail",
        "test-ci": "istanbul cover node_modules/mocha/bin/_mocha --report lcovonly -- --check-leaks --reporter spec",
        "test-cov": "istanbul cover node_modules/mocha/bin/_mocha -- --check-leaks --reporter dot"
    },
    "version": "0.15.1",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
