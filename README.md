# api documentation for  [send (v0.15.1)](https://github.com/pillarjs/send#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-send.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-send) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-send.svg)](https://travis-ci.org/npmdoc/node-npmdoc-send)
#### Better streaming static file server with Range and conditional-GET support

[![NPM](https://nodei.co/npm/send.png?downloads=true)](https://www.npmjs.com/package/send)

[![apidoc](https://npmdoc.github.io/node-npmdoc-send/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-send_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-send/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-send/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-send/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "TJ Holowaychuk",
        "email": "tj@vision-media.ca"
    },
    "bugs": {
        "url": "https://github.com/pillarjs/send/issues"
    },
    "contributors": [
        {
            "name": "Douglas Christopher Wilson",
            "email": "doug@somethingdoug.com"
        },
        {
            "name": "James Wyatt Cready",
            "email": "jcready@gmail.com"
        },
        {
            "name": "Jesús Leganés Combarro",
            "email": "piranna@gmail.com"
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
            "name": "dougwilson",
            "email": "doug@somethingdoug.com"
        }
    ],
    "name": "send",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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
    "version": "0.15.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module send](#apidoc.module.send)
1.  [function <span class="apidocSignatureSpan">send.</span>mime.Mime ()](#apidoc.element.send.mime.Mime)
1.  object <span class="apidocSignatureSpan">send.</span>mime
1.  object <span class="apidocSignatureSpan">send.</span>mime.Mime.prototype
1.  object <span class="apidocSignatureSpan">send.</span>mime.charsets

#### [module send.mime](#apidoc.module.send.mime)
1.  [function <span class="apidocSignatureSpan">send.mime.</span>Mime ()](#apidoc.element.send.mime.Mime)
1.  object <span class="apidocSignatureSpan">send.mime.</span>charsets
1.  object <span class="apidocSignatureSpan">send.mime.</span>extensions
1.  object <span class="apidocSignatureSpan">send.mime.</span>types
1.  string <span class="apidocSignatureSpan">send.mime.</span>default_type

#### [module send.mime.Mime](#apidoc.module.send.mime.Mime)
1.  [function <span class="apidocSignatureSpan">send.mime.</span>Mime ()](#apidoc.element.send.mime.Mime.Mime)

#### [module send.mime.Mime.prototype](#apidoc.module.send.mime.Mime.prototype)
1.  [function <span class="apidocSignatureSpan">send.mime.Mime.prototype.</span>define (map)](#apidoc.element.send.mime.Mime.prototype.define)
1.  [function <span class="apidocSignatureSpan">send.mime.Mime.prototype.</span>extension (mimeType)](#apidoc.element.send.mime.Mime.prototype.extension)
1.  [function <span class="apidocSignatureSpan">send.mime.Mime.prototype.</span>load (file)](#apidoc.element.send.mime.Mime.prototype.load)
1.  [function <span class="apidocSignatureSpan">send.mime.Mime.prototype.</span>lookup (path, fallback)](#apidoc.element.send.mime.Mime.prototype.lookup)

#### [module send.mime.charsets](#apidoc.module.send.mime.charsets)
1.  [function <span class="apidocSignatureSpan">send.mime.charsets.</span>lookup (mimeType, fallback)](#apidoc.element.send.mime.charsets.lookup)



# <a name="apidoc.module.send"></a>[module send](#apidoc.module.send)

#### <a name="apidoc.element.send.mime.Mime"></a>[function <span class="apidocSignatureSpan">send.</span>mime.Mime ()](#apidoc.element.send.mime.Mime)
- description and source-code
```javascript
function Mime() {
  // Map of extension -> mime type
  this.types = Object.create(null);

  // Map of mime type -> extension
  this.extensions = Object.create(null);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.send.mime"></a>[module send.mime](#apidoc.module.send.mime)

#### <a name="apidoc.element.send.mime.Mime"></a>[function <span class="apidocSignatureSpan">send.mime.</span>Mime ()](#apidoc.element.send.mime.Mime)
- description and source-code
```javascript
function Mime() {
  // Map of extension -> mime type
  this.types = Object.create(null);

  // Map of mime type -> extension
  this.extensions = Object.create(null);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.send.mime.Mime"></a>[module send.mime.Mime](#apidoc.module.send.mime.Mime)

#### <a name="apidoc.element.send.mime.Mime.Mime"></a>[function <span class="apidocSignatureSpan">send.mime.</span>Mime ()](#apidoc.element.send.mime.Mime.Mime)
- description and source-code
```javascript
function Mime() {
  // Map of extension -> mime type
  this.types = Object.create(null);

  // Map of mime type -> extension
  this.extensions = Object.create(null);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.send.mime.Mime.prototype"></a>[module send.mime.Mime.prototype](#apidoc.module.send.mime.Mime.prototype)

#### <a name="apidoc.element.send.mime.Mime.prototype.define"></a>[function <span class="apidocSignatureSpan">send.mime.Mime.prototype.</span>define (map)](#apidoc.element.send.mime.Mime.prototype.define)
- description and source-code
```javascript
define = function (map) {
  for (var type in map) {
    var exts = map[type];
    for (var i = 0; i < exts.length; i++) {
      if (process.env.DEBUG_MIME && this.types[exts]) {
        console.warn(this._loading.replace(/.*\//, ''), 'changes "' + exts[i] + '" extension type from ' +
          this.types[exts] + ' to ' + type);
      }

      this.types[exts[i]] = type;
    }

    // Default extension is the first one we encounter
    if (!this.extensions[type]) {
      this.extensions[type] = exts[0];
    }
  }
}
```
- example usage
```shell
...
var parseUrl = require('parseurl')
var send = require('send')

// Default unknown types to text/plain
send.mime.default_type = 'text/plain'

// Add a custom type
send.mime.define({
  'application/x-my-type': ['x-mt', 'x-mtt']
})

var server = http.createServer(function onRequest (req, res) {
  send(req, parseUrl(req).pathname).pipe(res)
})
...
```

#### <a name="apidoc.element.send.mime.Mime.prototype.extension"></a>[function <span class="apidocSignatureSpan">send.mime.Mime.prototype.</span>extension (mimeType)](#apidoc.element.send.mime.Mime.prototype.extension)
- description and source-code
```javascript
extension = function (mimeType) {
  var type = mimeType.match(/^\s*([^;\s]*)(?:;|\s|$)/)[1].toLowerCase();
  return this.extensions[type];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.send.mime.Mime.prototype.load"></a>[function <span class="apidocSignatureSpan">send.mime.Mime.prototype.</span>load (file)](#apidoc.element.send.mime.Mime.prototype.load)
- description and source-code
```javascript
load = function (file) {
  this._loading = file;
  // Read file and split into lines
  var map = {},
      content = fs.readFileSync(file, 'ascii'),
      lines = content.split(/[\r\n]+/);

  lines.forEach(function(line) {
    // Clean up whitespace/comments, and split into fields
    var fields = line.replace(/\s*#.*|^\s*|\s*$/g, '').split(/\s+/);
    map[fields.shift()] = fields;
  });

  this.define(map);

  this._loading = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.send.mime.Mime.prototype.lookup"></a>[function <span class="apidocSignatureSpan">send.mime.Mime.prototype.</span>lookup (path, fallback)](#apidoc.element.send.mime.Mime.prototype.lookup)
- description and source-code
```javascript
lookup = function (path, fallback) {
  var ext = path.replace(/.*[\.\/\\]/, '').toLowerCase();

  return this.types[ext] || fallback || this.default_type;
}
```
- example usage
```shell
...
 */

SendStream.prototype.type = function type (path) {
var res = this.res

if (res.getHeader('Content-Type')) return

var type = mime.lookup(path)

if (!type) {
  debug('no content-type')
  return
}

var charset = mime.charsets.lookup(type)
...
```



# <a name="apidoc.module.send.mime.charsets"></a>[module send.mime.charsets](#apidoc.module.send.mime.charsets)

#### <a name="apidoc.element.send.mime.charsets.lookup"></a>[function <span class="apidocSignatureSpan">send.mime.charsets.</span>lookup (mimeType, fallback)](#apidoc.element.send.mime.charsets.lookup)
- description and source-code
```javascript
lookup = function (mimeType, fallback) {
  // Assume text types are utf8
  return (/^text\//).test(mimeType) ? 'UTF-8' : fallback;
}
```
- example usage
```shell
...
 */

SendStream.prototype.type = function type (path) {
var res = this.res

if (res.getHeader('Content-Type')) return

var type = mime.lookup(path)

if (!type) {
  debug('no content-type')
  return
}

var charset = mime.charsets.lookup(type)
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
