# npmdoc-choo

#### basic api documentation for  [choo (v5.3.0)](https://github.com/yoshuawuyts/choo#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-choo.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-choo) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-choo.svg)](https://travis-ci.org/npmdoc/node-npmdoc-choo)

#### A 4kb framework for creating sturdy frontend applications

[![NPM](https://nodei.co/npm/choo.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/choo)

- [https://npmdoc.github.io/node-npmdoc-choo/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-choo/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-choo/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-choo/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-choo/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-choo/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "bugs": {
        "url": "https://github.com/yoshuawuyts/choo/issues"
    },
    "dependencies": {
        "bel": "^4.5.1",
        "document-ready": "^2.0.1",
        "nanobus": "^3.1.0",
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
        "shasum": "d2ed1701d4d0b61387420861c915629b09fc5dbf",
        "tarball": "https://registry.npmjs.org/choo/-/choo-5.3.0.tgz"
    },
    "gitHead": "d17b3e480120f3cd809c7f87abfe3a36b62ce29f",
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
    "version": "5.3.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
