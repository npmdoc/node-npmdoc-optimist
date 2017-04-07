# api documentation for  [optimist (v0.6.1)](https://github.com/substack/node-optimist)  [![npm package](https://img.shields.io/npm/v/npmdoc-optimist.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-optimist) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-optimist.svg)](https://travis-ci.org/npmdoc/node-npmdoc-optimist)
#### Light-weight option parsing with an argv hash. No optstrings attached.

[![NPM](https://nodei.co/npm/optimist.png?downloads=true)](https://www.npmjs.com/package/optimist)

[![apidoc](https://npmdoc.github.io/node-npmdoc-optimist/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-optimist_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-optimist/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-optimist/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-optimist/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "James Halliday",
        "email": "mail@substack.net",
        "url": "http://substack.net"
    },
    "bugs": {
        "url": "https://github.com/substack/node-optimist/issues"
    },
    "dependencies": {
        "minimist": "~0.0.1",
        "wordwrap": "~0.0.2"
    },
    "description": "Light-weight option parsing with an argv hash. No optstrings attached.",
    "devDependencies": {
        "hashish": "~0.0.4",
        "tap": "~0.4.0"
    },
    "directories": {},
    "dist": {
        "shasum": "da3ea74686fa21a19a111c326e90eb15a0196686",
        "tarball": "https://registry.npmjs.org/optimist/-/optimist-0.6.1.tgz"
    },
    "engine": {
        "node": ">=0.4"
    },
    "homepage": "https://github.com/substack/node-optimist",
    "keywords": [
        "argument",
        "args",
        "option",
        "parser",
        "parsing",
        "cli",
        "command"
    ],
    "license": "MIT/X11",
    "main": "./index.js",
    "maintainers": [
        {
            "name": "substack",
            "email": "mail@substack.net"
        }
    ],
    "name": "optimist",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/substack/node-optimist.git"
    },
    "scripts": {
        "test": "tap ./test/*.js"
    },
    "version": "0.6.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module optimist](#apidoc.module.optimist)
1.  [function <span class="apidocSignatureSpan">optimist.</span>alias ()](#apidoc.element.optimist.alias)
1.  [function <span class="apidocSignatureSpan">optimist.</span>boolean ()](#apidoc.element.optimist.boolean)
1.  [function <span class="apidocSignatureSpan">optimist.</span>check ()](#apidoc.element.optimist.check)
1.  [function <span class="apidocSignatureSpan">optimist.</span>default ()](#apidoc.element.optimist.default)
1.  [function <span class="apidocSignatureSpan">optimist.</span>demand ()](#apidoc.element.optimist.demand)
1.  [function <span class="apidocSignatureSpan">optimist.</span>describe ()](#apidoc.element.optimist.describe)
1.  [function <span class="apidocSignatureSpan">optimist.</span>help ()](#apidoc.element.optimist.help)
1.  [function <span class="apidocSignatureSpan">optimist.</span>option ()](#apidoc.element.optimist.option)
1.  [function <span class="apidocSignatureSpan">optimist.</span>options ()](#apidoc.element.optimist.options)
1.  [function <span class="apidocSignatureSpan">optimist.</span>parse ()](#apidoc.element.optimist.parse)
1.  [function <span class="apidocSignatureSpan">optimist.</span>rebase (base, dir)](#apidoc.element.optimist.rebase)
1.  [function <span class="apidocSignatureSpan">optimist.</span>showHelp ()](#apidoc.element.optimist.showHelp)
1.  [function <span class="apidocSignatureSpan">optimist.</span>string ()](#apidoc.element.optimist.string)
1.  [function <span class="apidocSignatureSpan">optimist.</span>usage ()](#apidoc.element.optimist.usage)
1.  [function <span class="apidocSignatureSpan">optimist.</span>wrap ()](#apidoc.element.optimist.wrap)
1.  object <span class="apidocSignatureSpan">optimist.</span>argv



# <a name="apidoc.module.optimist"></a>[module optimist](#apidoc.module.optimist)

#### <a name="apidoc.element.optimist.alias"></a>[function <span class="apidocSignatureSpan">optimist.</span>alias ()](#apidoc.element.optimist.alias)
- description and source-code
```javascript
alias = function () { [native code] }
```
- example usage
```shell
...
    }
    return self;
};

self.alias = function (x, y) {
    if (typeof x === 'object') {
        Object.keys(x).forEach(function (key) {
            self.alias(key, x[key]);
        });
    }
    else {
        options.alias[x] = (options.alias[x] || []).concat(y);
    }
    return self;
};
...
```

#### <a name="apidoc.element.optimist.boolean"></a>[function <span class="apidocSignatureSpan">optimist.</span>boolean ()](#apidoc.element.optimist.boolean)
- description and source-code
```javascript
boolean = function () { [native code] }
```
- example usage
```shell
...
if (opt.alias) self.alias(key, opt.alias);
if (opt.demand) self.demand(key);
if (typeof opt.default !== 'undefined') {
    self.default(key, opt.default);
}

if (opt.boolean || opt.type === 'boolean') {
    self.boolean(key);
}
if (opt.string || opt.type === 'string') {
    self.string(key);
}

var desc = opt.describe || opt.description || opt.desc;
if (desc) {
...
```

#### <a name="apidoc.element.optimist.check"></a>[function <span class="apidocSignatureSpan">optimist.</span>check ()](#apidoc.element.optimist.check)
- description and source-code
```javascript
check = function () { [native code] }
```
- example usage
```shell
...
.usage(message)
---------------

Set a usage message to show which commands to use. Inside 'message', the string
'$0' will get interpolated to the current script name or node command for the
present script similar to how '$0' works in bash or perl.

.check(fn)
----------

Check that certain conditions are met in the provided arguments.

If 'fn' throws or returns 'false', show the thrown error, usage information, and
exit.
...
```

#### <a name="apidoc.element.optimist.default"></a>[function <span class="apidocSignatureSpan">optimist.</span>default ()](#apidoc.element.optimist.default)
- description and source-code
```javascript
default = function () { [native code] }
```
- example usage
```shell
...
    options.string.push.apply(options.string, [].concat(strings));
    return self;
};

self.default = function (key, value) {
    if (typeof key === 'object') {
        Object.keys(key).forEach(function (k) {
            self.default(k, key[k]);
        });
    }
    else {
        options.default[key] = value;
    }
    return self;
};
...
```

#### <a name="apidoc.element.optimist.demand"></a>[function <span class="apidocSignatureSpan">optimist.</span>demand ()](#apidoc.element.optimist.demand)
- description and source-code
```javascript
demand = function () { [native code] }
```
- example usage
```shell
...
    self.demand = function (keys) {
if (typeof keys == 'number') {
    if (!demanded._) demanded._ = 0;
    demanded._ += keys;
}
else if (Array.isArray(keys)) {
    keys.forEach(function (key) {
        self.demand(key);
    });
}
else {
    demanded[keys] = true;
}

return self;
...
```

#### <a name="apidoc.element.optimist.describe"></a>[function <span class="apidocSignatureSpan">optimist.</span>describe ()](#apidoc.element.optimist.describe)
- description and source-code
```javascript
describe = function () { [native code] }
```
- example usage
```shell
...
    return self;
};

var descriptions = {};
self.describe = function (key, desc) {
    if (typeof key === 'object') {
        Object.keys(key).forEach(function (k) {
            self.describe(k, key[k]);
        });
    }
    else {
        descriptions[key] = desc;
    }
    return self;
};
...
```

#### <a name="apidoc.element.optimist.help"></a>[function <span class="apidocSignatureSpan">optimist.</span>help ()](#apidoc.element.optimist.help)
- description and source-code
```javascript
help = function () { [native code] }
```
- example usage
```shell
...
self.wrap = function (cols) {
    wrap = cols;
    return self;
};

self.showHelp = function (fn) {
    if (!fn) fn = console.error;
    fn(self.help());
};

self.help = function () {
    var keys = Object.keys(
        Object.keys(descriptions)
        .concat(Object.keys(demanded))
        .concat(Object.keys(options.default))
...
```

#### <a name="apidoc.element.optimist.option"></a>[function <span class="apidocSignatureSpan">optimist.</span>option ()](#apidoc.element.optimist.option)
- description and source-code
```javascript
option = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.optimist.options"></a>[function <span class="apidocSignatureSpan">optimist.</span>options ()](#apidoc.element.optimist.options)
- description and source-code
```javascript
options = function () { [native code] }
```
- example usage
```shell
...
    if (!opts && typeof msg === 'object') {
        opts = msg;
        msg = null;
    }

    usage = msg;

    if (opts) self.options(opts);

    return self;
};

function fail (msg) {
    self.showHelp();
    if (msg) console.error(msg);
...
```

#### <a name="apidoc.element.optimist.parse"></a>[function <span class="apidocSignatureSpan">optimist.</span>parse ()](#apidoc.element.optimist.parse)
- description and source-code
```javascript
parse = function () { [native code] }
```
- example usage
```shell
...

You can pass in the 'process.argv' yourself:

''''javascript
require('optimist')([ '-x', '1', '-y', '2' ]).argv
''''

or use .parse() to do the same thing:

''''javascript
require('optimist').parse([ '-x', '1', '-y', '2' ])
''''

The rest of these methods below come in just before the terminating '.argv'.
...
```

#### <a name="apidoc.element.optimist.rebase"></a>[function <span class="apidocSignatureSpan">optimist.</span>rebase (base, dir)](#apidoc.element.optimist.rebase)
- description and source-code
```javascript
function rebase(base, dir) {
    var ds = path.normalize(dir).split('/').slice(1);
    var bs = path.normalize(base).split('/').slice(1);

    for (var i = 0; ds[i] && ds[i] == bs[i]; i++);
    ds.splice(0, i); bs.splice(0, i);

    var p = path.normalize(
        bs.map(function () { return '..' }).concat(ds).join('/')
    ).replace(/\/$/,'').replace(/^$/, '.');
    return p.match(/^[.\/]/) ? p : './' + p;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.optimist.showHelp"></a>[function <span class="apidocSignatureSpan">optimist.</span>showHelp ()](#apidoc.element.optimist.showHelp)
- description and source-code
```javascript
showHelp = function () { [native code] }
```
- example usage
```shell
...

    if (opts) self.options(opts);

    return self;
};

function fail (msg) {
    self.showHelp();
    if (msg) console.error(msg);
    process.exit(1);
}

var checks = [];
self.check = function (f) {
    checks.push(f);
...
```

#### <a name="apidoc.element.optimist.string"></a>[function <span class="apidocSignatureSpan">optimist.</span>string ()](#apidoc.element.optimist.string)
- description and source-code
```javascript
string = function () { [native code] }
```
- example usage
```shell
...
        self.default(key, opt.default);
    }

    if (opt.boolean || opt.type === 'boolean') {
        self.boolean(key);
    }
    if (opt.string || opt.type === 'string') {
        self.string(key);
    }

    var desc = opt.describe || opt.description || opt.desc;
    if (desc) {
        self.describe(key, desc);
    }
}
...
```

#### <a name="apidoc.element.optimist.usage"></a>[function <span class="apidocSignatureSpan">optimist.</span>usage ()](#apidoc.element.optimist.usage)
- description and source-code
```javascript
usage = function () { [native code] }
```
- example usage
```shell
...
    (6.82,3.35)
    [ 'moo' ]

    $ ./nonopt.js foo -x 0.54 bar -y 1.12 baz
    (0.54,1.12)
    [ 'foo', 'bar', 'baz' ]

Plus, Optimist comes with .usage() and .demand()!
-------------------------------------------------

divide.js:

''''javascript
#!/usr/bin/env node
var argv = require('optimist')
...
```

#### <a name="apidoc.element.optimist.wrap"></a>[function <span class="apidocSignatureSpan">optimist.</span>wrap ()](#apidoc.element.optimist.wrap)
- description and source-code
```javascript
wrap = function () { [native code] }
```
- example usage
```shell
...
------------

Tell the parser logic not to interpret 'key' as a number or boolean.
This can be useful if you need to preserve leading zeros in an input.

If 'key' is an Array, interpret all the elements as strings.

.wrap(columns)
--------------

Format usage output to wrap at 'columns' many columns.

.help()
-------
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
