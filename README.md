# npmdoc-http-proxy-middleware

#### api documentation for  [http-proxy-middleware (v0.17.4)](https://github.com/chimurai/http-proxy-middleware)  [![npm package](https://img.shields.io/npm/v/npmdoc-http-proxy-middleware.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-http-proxy-middleware) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-http-proxy-middleware.svg)](https://travis-ci.org/npmdoc/node-npmdoc-http-proxy-middleware)

#### The one-liner node.js proxy middleware for connect, express and browser-sync

[![NPM](https://nodei.co/npm/http-proxy-middleware.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/http-proxy-middleware)

- [https://npmdoc.github.io/node-npmdoc-http-proxy-middleware/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-http-proxy-middleware/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-http-proxy-middleware/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-http-proxy-middleware/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-http-proxy-middleware/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-http-proxy-middleware/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Steven Chim"
    },
    "bugs": {
        "url": "https://github.com/chimurai/http-proxy-middleware/issues"
    },
    "dependencies": {
        "http-proxy": "^1.16.2",
        "is-glob": "^3.1.0",
        "lodash": "^4.17.2",
        "micromatch": "^2.3.11"
    },
    "description": "The one-liner node.js proxy middleware for connect, express and browser-sync",
    "devDependencies": {
        "browser-sync": "^2.18.2",
        "chai": "^3.5.0",
        "connect": "^3.5.0",
        "coveralls": "^2.11.15",
        "express": "^4.14.0",
        "istanbul": "^0.4.5",
        "istanbul-coveralls": "^1.0.3",
        "mocha": "^3.2.0",
        "mocha-lcov-reporter": "1.2.0",
        "opn": "^4.0.2",
        "ws": "^1.1.1"
    },
    "directories": {},
    "dist": {
        "shasum": "642e8848851d66f09d4f124912846dbaeb41b833",
        "tarball": "https://registry.npmjs.org/http-proxy-middleware/-/http-proxy-middleware-0.17.4.tgz"
    },
    "files": [
        "index.js",
        "lib"
    ],
    "gitHead": "cb5e084e71bc3202fe4f711f2f5edf4e29355d99",
    "homepage": "https://github.com/chimurai/http-proxy-middleware",
    "keywords": [
        "reverse",
        "proxy",
        "middleware",
        "http",
        "https",
        "connect",
        "express",
        "browser-sync",
        "gulp",
        "grunt-contrib-connect",
        "websocket",
        "ws",
        "cors"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "chimurai"
        }
    ],
    "name": "http-proxy-middleware",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/chimurai/http-proxy-middleware.git"
    },
    "scripts": {
        "clean": "rm -rf coverage",
        "cover": "npm run clean && istanbul cover ./node_modules/mocha/bin/_mocha -- --recursive",
        "coveralls": "istanbul cover ./node_modules/mocha/bin/_mocha --report lcovonly -- --recursive --reporter spec && istanbul-coveralls && npm run clean",
        "test": "mocha --recursive --colors --reporter spec"
    },
    "version": "0.17.4",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
