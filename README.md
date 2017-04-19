# npmdoc-node-zookeeper-client

#### api documentation for  [node-zookeeper-client (v0.2.2)](https://github.com/alexguan/node-zookeeper-client)  [![npm package](https://img.shields.io/npm/v/npmdoc-node-zookeeper-client.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-node-zookeeper-client) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-node-zookeeper-client.svg)](https://travis-ci.org/npmdoc/node-npmdoc-node-zookeeper-client)

#### A pure Javascript ZooKeeper client for Node.js.

[![NPM](https://nodei.co/npm/node-zookeeper-client.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/node-zookeeper-client)

- [https://npmdoc.github.io/node-npmdoc-node-zookeeper-client/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-node-zookeeper-client/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-node-zookeeper-client/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-node-zookeeper-client/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-node-zookeeper-client/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-node-zookeeper-client/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Alex Guan"
    },
    "bugs": {
        "url": "https://github.com/alexguan/node-zookeeper-client/issues"
    },
    "dependencies": {
        "async": "~0.2.7",
        "underscore": "~1.4.4"
    },
    "description": "A pure Javascript ZooKeeper client for Node.js.",
    "devDependencies": {
        "chai": "~1.5.0",
        "istanbul": "~0.1.34",
        "jslint": "~0.1.9",
        "mocha": "~1.9.0"
    },
    "directories": {},
    "dist": {
        "shasum": "097bda01999eef8f602ce068b632600069dbf685",
        "tarball": "https://registry.npmjs.org/node-zookeeper-client/-/node-zookeeper-client-0.2.2.tgz"
    },
    "engines": {
        "node": ">=0.6.0"
    },
    "gitHead": "db474832e7f6ee084d683f873ca8eaf7c37feeff",
    "homepage": "https://github.com/alexguan/node-zookeeper-client",
    "keywords": [
        "zookeeper",
        "client",
        "pure",
        "javascript"
    ],
    "licenses": [
        {
            "type": "MIT",
            "url": "http://github.com/alexguan/node-zookeeper-client/raw/master/LICENSE"
        }
    ],
    "main": "index.js",
    "maintainers": [
        {
            "name": "alexguan"
        }
    ],
    "name": "node-zookeeper-client",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/alexguan/node-zookeeper-client.git"
    },
    "scripts": {
        "coverage": "istanbul cover _mocha --recursive test/*",
        "pretest": "jslint --node --sloppy index.js lib/*.js lib/jute/*.js",
        "test": "mocha --recursive --reporter spec test/*"
    },
    "version": "0.2.2"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
