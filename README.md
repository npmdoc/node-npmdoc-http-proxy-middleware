# api documentation for  [http-proxy-middleware (v0.17.4)](https://github.com/chimurai/http-proxy-middleware)  [![npm package](https://img.shields.io/npm/v/npmdoc-http-proxy-middleware.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-http-proxy-middleware) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-http-proxy-middleware.svg)](https://travis-ci.org/npmdoc/node-npmdoc-http-proxy-middleware)
#### The one-liner node.js proxy middleware for connect, express and browser-sync

[![NPM](https://nodei.co/npm/http-proxy-middleware.png?downloads=true)](https://www.npmjs.com/package/http-proxy-middleware)

[![apidoc](https://npmdoc.github.io/node-npmdoc-http-proxy-middleware/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-http-proxy-middleware_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-http-proxy-middleware/build..beta..travis-ci.org/apidoc.html)

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
            "name": "chimurai",
            "email": "stevenchim@gmail.com"
        }
    ],
    "name": "http-proxy-middleware",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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
    "version": "0.17.4"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module http-proxy-middleware](#apidoc.module.http-proxy-middleware)
1.  object <span class="apidocSignatureSpan">http-proxy-middleware.</span>config_factory
1.  object <span class="apidocSignatureSpan">http-proxy-middleware.</span>context_matcher
1.  object <span class="apidocSignatureSpan">http-proxy-middleware.</span>handlers
1.  object <span class="apidocSignatureSpan">http-proxy-middleware.</span>logger
1.  object <span class="apidocSignatureSpan">http-proxy-middleware.</span>path_rewriter
1.  object <span class="apidocSignatureSpan">http-proxy-middleware.</span>router

#### [module http-proxy-middleware.config_factory](#apidoc.module.http-proxy-middleware.config_factory)
1.  [function <span class="apidocSignatureSpan">http-proxy-middleware.config_factory.</span>createConfig (context, opts)](#apidoc.element.http-proxy-middleware.config_factory.createConfig)

#### [module http-proxy-middleware.context_matcher](#apidoc.module.http-proxy-middleware.context_matcher)
1.  [function <span class="apidocSignatureSpan">http-proxy-middleware.context_matcher.</span>match (context, uri, req)](#apidoc.element.http-proxy-middleware.context_matcher.match)

#### [module http-proxy-middleware.handlers](#apidoc.module.http-proxy-middleware.handlers)
1.  [function <span class="apidocSignatureSpan">http-proxy-middleware.handlers.</span>getHandlers (opts)](#apidoc.element.http-proxy-middleware.handlers.getHandlers)
1.  [function <span class="apidocSignatureSpan">http-proxy-middleware.handlers.</span>init (proxy, opts)](#apidoc.element.http-proxy-middleware.handlers.init)

#### [module http-proxy-middleware.logger](#apidoc.module.http-proxy-middleware.logger)
1.  [function <span class="apidocSignatureSpan">http-proxy-middleware.logger.</span>getArrow (originalPath, newPath, originalTarget, newTarget)](#apidoc.element.http-proxy-middleware.logger.getArrow)
1.  [function <span class="apidocSignatureSpan">http-proxy-middleware.logger.</span>getInstance ()](#apidoc.element.http-proxy-middleware.logger.getInstance)

#### [module http-proxy-middleware.path_rewriter](#apidoc.module.http-proxy-middleware.path_rewriter)
1.  [function <span class="apidocSignatureSpan">http-proxy-middleware.path_rewriter.</span>create (rewriteConfig)](#apidoc.element.http-proxy-middleware.path_rewriter.create)

#### [module http-proxy-middleware.router](#apidoc.module.http-proxy-middleware.router)
1.  [function <span class="apidocSignatureSpan">http-proxy-middleware.router.</span>getTarget (req, config)](#apidoc.element.http-proxy-middleware.router.getTarget)



# <a name="apidoc.module.http-proxy-middleware"></a>[module http-proxy-middleware](#apidoc.module.http-proxy-middleware)



# <a name="apidoc.module.http-proxy-middleware.config_factory"></a>[module http-proxy-middleware.config_factory](#apidoc.module.http-proxy-middleware.config_factory)

#### <a name="apidoc.element.http-proxy-middleware.config_factory.createConfig"></a>[function <span class="apidocSignatureSpan">http-proxy-middleware.config_factory.</span>createConfig (context, opts)](#apidoc.element.http-proxy-middleware.config_factory.createConfig)
- description and source-code
```javascript
function createConfig(context, opts) {
    // structure of config object to be returned
    var config = {
        context: undefined,
        options: {}
    };

    // app.use('/api', proxy({target:'http://localhost:9000'}));
    if (isContextless(context, opts)) {
        config.context = '/';
        config.options = _.assign(config.options, context);
    }
    // app.use('/api', proxy('http://localhost:9000'));
    // app.use(proxy('http://localhost:9000/api'));
    else if (isStringShortHand(context)) {
        var oUrl   = url.parse(context);
        var target = [oUrl.protocol, '//', oUrl.host].join('');

        config.context = oUrl.pathname || '/';
        config.options = _.assign(config.options, {target: target}, opts);

        if (oUrl.protocol === 'ws:' || oUrl.protocol === 'wss:') {
            config.options.ws = true;
        }
    // app.use('/api', proxy({target:'http://localhost:9000'}));
    } else {
        config.context = context;
        config.options = _.assign(config.options, opts);
    }

    configureLogger(config.options);

    if (!config.options.target) {
        throw new Error('[HPM] Missing "target" option. Example: {target: "http://www.example.org"}');
    }

    // Legacy option.proxyHost
    config.options = mapLegacyProxyHostOption(config.options);

    // Legacy option.proxyTable > option.router
    config.options = mapLegacyProxyTableOption(config.options);

    return config;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.http-proxy-middleware.context_matcher"></a>[module http-proxy-middleware.context_matcher](#apidoc.module.http-proxy-middleware.context_matcher)

#### <a name="apidoc.element.http-proxy-middleware.context_matcher.match"></a>[function <span class="apidocSignatureSpan">http-proxy-middleware.context_matcher.</span>match (context, uri, req)](#apidoc.element.http-proxy-middleware.context_matcher.match)
- description and source-code
```javascript
function matchContext(context, uri, req) {

    // single path
    if (isStringPath(context)) {
        return matchSingleStringPath(context, uri);
    }

    // single glob path
    if (isGlobPath(context)) {
        return matchSingleGlobPath(context, uri);
    }

    // multi path
    if (Array.isArray(context)) {
        if (context.every(isStringPath)) {
            return matchMultiPath(context, uri);
        }
        if (context.every(isGlobPath)) {
            return matchMultiGlobPath(context, uri);
        }

        throw new Error('[HPM] Invalid context. Expecting something like: ["/api", "/ajax"] or ["/api/**", "!**.html"]');
    }

    // custom matching
    if (_.isFunction(context)) {
        var pathname = getUrlPathName(uri);
        return context(pathname, req);
    }

    throw new Error('[HPM] Invalid context. Expecting something like: "/api" or ["/api", "/ajax"]');
}
```
- example usage
```shell
...

    For full control you can provide a custom function to determine which requests should be proxied or not.
    '''javascript
    /**
     * @return {Boolean}
     */
    var filter = function (pathname, req) {
        return (pathname.match('^/api') && req.method === 'GET');
    };

    var apiProxy = proxy(filter, {target: 'http://www.example.org'})
    '''

## Options
...
```



# <a name="apidoc.module.http-proxy-middleware.handlers"></a>[module http-proxy-middleware.handlers](#apidoc.module.http-proxy-middleware.handlers)

#### <a name="apidoc.element.http-proxy-middleware.handlers.getHandlers"></a>[function <span class="apidocSignatureSpan">http-proxy-middleware.handlers.</span>getHandlers (opts)](#apidoc.element.http-proxy-middleware.handlers.getHandlers)
- description and source-code
```javascript
function getProxyEventHandlers(opts) {
    // https://github.com/nodejitsu/node-http-proxy#listening-for-proxy-events
    var proxyEvents = ['error', 'proxyReq', 'proxyReqWs', 'proxyRes', 'open', 'close'];
    var handlers = {};

    _.forEach(proxyEvents, function(event) {
        // all handlers for the http-proxy events are prefixed with 'on'.
        // loop through options and try to find these handlers
        // and add them to the handlers object for subscription in init().
        var eventName = _.camelCase('on ' + event);
        var fnHandler = _.get(opts, eventName);

        if (_.isFunction(fnHandler)) {
            handlers[event] = fnHandler;
        }
    });

    // add default error handler in absence of error handler
    if (!_.isFunction(handlers.error)) {
        handlers.error = defaultErrorHandler;
    }

    // add default close handler in absence of close handler
    if (!_.isFunction(handlers.close)) {
        handlers.close = logClose;
    }

    return handlers;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.http-proxy-middleware.handlers.init"></a>[function <span class="apidocSignatureSpan">http-proxy-middleware.handlers.</span>init (proxy, opts)](#apidoc.element.http-proxy-middleware.handlers.init)
- description and source-code
```javascript
function init(proxy, opts) {
    var handlers = getProxyEventHandlers(opts);

    _.forIn(handlers, function(handler, eventName) {
        proxy.on(eventName, handlers[eventName]);
    });

    logger.debug('[HPM] Subscribed to http-proxy events: ', _.keys(handlers));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.http-proxy-middleware.logger"></a>[module http-proxy-middleware.logger](#apidoc.module.http-proxy-middleware.logger)

#### <a name="apidoc.element.http-proxy-middleware.logger.getArrow"></a>[function <span class="apidocSignatureSpan">http-proxy-middleware.logger.</span>getArrow (originalPath, newPath, originalTarget, newTarget)](#apidoc.element.http-proxy-middleware.logger.getArrow)
- description and source-code
```javascript
function getArrow(originalPath, newPath, originalTarget, newTarget) {
    var arrow = ['>'];
    var isNewTarget = (originalTarget !== newTarget); // router
    var isNewPath = (originalPath !== newPath); // pathRewrite

    if (isNewPath && !isNewTarget) {arrow.unshift('~');} else if (!isNewPath && isNewTarget) {arrow.unshift('=');} else if (isNewPath
 && isNewTarget) {arrow.unshift('≈');} else {arrow.unshift('-');}

    return arrow.join('');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.http-proxy-middleware.logger.getInstance"></a>[function <span class="apidocSignatureSpan">http-proxy-middleware.logger.</span>getInstance ()](#apidoc.element.http-proxy-middleware.logger.getInstance)
- description and source-code
```javascript
getInstance = function () {
    if (!loggerInstance) {
        loggerInstance = new Logger();
    }

    return loggerInstance;
}
```
- example usage
```shell
...





var _      = require('lodash');
var url    = require('url');
var logger = require('./logger').getInstance();

module.exports = {
createConfig: createConfig
};

function createConfig(context, opts) {
// structure of config object to be returned
...
```



# <a name="apidoc.module.http-proxy-middleware.path_rewriter"></a>[module http-proxy-middleware.path_rewriter](#apidoc.module.http-proxy-middleware.path_rewriter)

#### <a name="apidoc.element.http-proxy-middleware.path_rewriter.create"></a>[function <span class="apidocSignatureSpan">http-proxy-middleware.path_rewriter.</span>create (rewriteConfig)](#apidoc.element.http-proxy-middleware.path_rewriter.create)
- description and source-code
```javascript
function createPathRewriter(rewriteConfig) {
    var rulesCache;

    if (!isValidRewriteConfig(rewriteConfig)) {
        return;
    }

    if (_.isFunction(rewriteConfig)) {
        var customRewriteFn = rewriteConfig;
        return customRewriteFn;
    } else {
        rulesCache = parsePathRewriteRules(rewriteConfig);
        return rewritePath;
    }

    function rewritePath(path) {
        var result = path;

        _.forEach(rulesCache, function(rule) {
            if (rule.regex.test(path)) {
                result = result.replace(rule.regex, rule.value);
                logger.debug('[HPM] Rewriting path from "%s" to "%s"', path, result);
                return false;
            }
        });

        return result;
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.http-proxy-middleware.router"></a>[module http-proxy-middleware.router](#apidoc.module.http-proxy-middleware.router)

#### <a name="apidoc.element.http-proxy-middleware.router.getTarget"></a>[function <span class="apidocSignatureSpan">http-proxy-middleware.router.</span>getTarget (req, config)](#apidoc.element.http-proxy-middleware.router.getTarget)
- description and source-code
```javascript
function getTarget(req, config) {
    var newTarget;
    var router = config.router;

    if (_.isPlainObject(router)) {
        newTarget = getTargetFromProxyTable(req, router);
    } else if (_.isFunction(router)) {
        newTarget = router(req);
    }

    return newTarget;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
