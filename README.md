# api documentation for  [node-zookeeper-client (v0.2.2)](https://github.com/alexguan/node-zookeeper-client)  [![npm package](https://img.shields.io/npm/v/npmdoc-node-zookeeper-client.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-node-zookeeper-client) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-node-zookeeper-client.svg)](https://travis-ci.org/npmdoc/node-npmdoc-node-zookeeper-client)
#### A pure Javascript ZooKeeper client for Node.js.

[![NPM](https://nodei.co/npm/node-zookeeper-client.png?downloads=true)](https://www.npmjs.com/package/node-zookeeper-client)

[![apidoc](https://npmdoc.github.io/node-npmdoc-node-zookeeper-client/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-node-zookeeper-client_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-node-zookeeper-client/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-node-zookeeper-client/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-node-zookeeper-client/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Alex Guan",
        "email": "alex.guan@gmail.com"
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
            "name": "alexguan",
            "email": "alex.guan@gmail.com"
        }
    ],
    "name": "node-zookeeper-client",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module node-zookeeper-client](#apidoc.module.node-zookeeper-client)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.</span>ACL (permission, id)](#apidoc.element.node-zookeeper-client.ACL)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.</span>ConnectionManager (connectionString, options, stateListener)](#apidoc.element.node-zookeeper-client.ConnectionManager)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.</span>ConnectionStringParser (connectionString)](#apidoc.element.node-zookeeper-client.ConnectionStringParser)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.</span>Event (type, name, path)](#apidoc.element.node-zookeeper-client.Event)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.</span>Exception (code, name, path, ctor)](#apidoc.element.node-zookeeper-client.Exception)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.</span>Exception.super_ ()](#apidoc.element.node-zookeeper-client.Exception.super_)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.</span>Id (scheme, id)](#apidoc.element.node-zookeeper-client.Id)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.</span>PacketQueue ()](#apidoc.element.node-zookeeper-client.PacketQueue)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.</span>Transaction (connectionManager)](#apidoc.element.node-zookeeper-client.Transaction)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.</span>WatcherManager ()](#apidoc.element.node-zookeeper-client.WatcherManager)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.</span>createClient (connectionString, options)](#apidoc.element.node-zookeeper-client.createClient)
1.  object <span class="apidocSignatureSpan">node-zookeeper-client.</span>ACL.prototype
1.  object <span class="apidocSignatureSpan">node-zookeeper-client.</span>ConnectionManager.prototype
1.  object <span class="apidocSignatureSpan">node-zookeeper-client.</span>ConnectionStringParser.prototype
1.  object <span class="apidocSignatureSpan">node-zookeeper-client.</span>CreateMode
1.  object <span class="apidocSignatureSpan">node-zookeeper-client.</span>Event.prototype
1.  object <span class="apidocSignatureSpan">node-zookeeper-client.</span>Exception.prototype
1.  object <span class="apidocSignatureSpan">node-zookeeper-client.</span>Id.prototype
1.  object <span class="apidocSignatureSpan">node-zookeeper-client.</span>PacketQueue.prototype
1.  object <span class="apidocSignatureSpan">node-zookeeper-client.</span>Path
1.  object <span class="apidocSignatureSpan">node-zookeeper-client.</span>Permission
1.  object <span class="apidocSignatureSpan">node-zookeeper-client.</span>State
1.  object <span class="apidocSignatureSpan">node-zookeeper-client.</span>Transaction.prototype
1.  object <span class="apidocSignatureSpan">node-zookeeper-client.</span>WatcherManager.prototype

#### [module node-zookeeper-client.ACL](#apidoc.module.node-zookeeper-client.ACL)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.</span>ACL (permission, id)](#apidoc.element.node-zookeeper-client.ACL.ACL)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.ACL.</span>fromRecord (record)](#apidoc.element.node-zookeeper-client.ACL.fromRecord)
1.  object <span class="apidocSignatureSpan">node-zookeeper-client.ACL.</span>CREATOR_ALL_ACL
1.  object <span class="apidocSignatureSpan">node-zookeeper-client.ACL.</span>OPEN_ACL_UNSAFE
1.  object <span class="apidocSignatureSpan">node-zookeeper-client.ACL.</span>READ_ACL_UNSAFE

#### [module node-zookeeper-client.ACL.prototype](#apidoc.module.node-zookeeper-client.ACL.prototype)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.ACL.prototype.</span>toRecord ()](#apidoc.element.node-zookeeper-client.ACL.prototype.toRecord)

#### [module node-zookeeper-client.ConnectionManager](#apidoc.module.node-zookeeper-client.ConnectionManager)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.</span>ConnectionManager (connectionString, options, stateListener)](#apidoc.element.node-zookeeper-client.ConnectionManager.ConnectionManager)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.</span>super_ ()](#apidoc.element.node-zookeeper-client.ConnectionManager.super_)
1.  object <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.</span>STATES

#### [module node-zookeeper-client.ConnectionManager.prototype](#apidoc.module.node-zookeeper-client.ConnectionManager.prototype)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>addAuthInfo (scheme, auth)](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.addAuthInfo)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>cleanupPendingQueue (errorCode)](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.cleanupPendingQueue)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>close ()](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.close)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>connect ()](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.connect)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>findNextServer (callback)](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.findNextServer)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>getSessionId ()](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.getSessionId)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>getSessionPassword ()](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.getSessionPassword)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>getSessionTimeout ()](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.getSessionTimeout)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>onPacketQueueReadable ()](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.onPacketQueueReadable)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>onSocketClosed (hasError)](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.onSocketClosed)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>onSocketConnectTimeout ()](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.onSocketConnectTimeout)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>onSocketConnected ()](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.onSocketConnected)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>onSocketData (buffer)](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.onSocketData)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>onSocketDrain ()](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.onSocketDrain)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>onSocketError (error)](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.onSocketError)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>onSocketTimeout ()](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.onSocketTimeout)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>queue (request, callback)](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.queue)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>registerChildWatcher (path, watcher)](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.registerChildWatcher)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>registerDataWatcher (path, watcher)](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.registerDataWatcher)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>registerExistenceWatcher (path, watcher)](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.registerExistenceWatcher)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>setState (state)](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.setState)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>updateTimeout (sessionTimeout)](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.updateTimeout)

#### [module node-zookeeper-client.ConnectionStringParser](#apidoc.module.node-zookeeper-client.ConnectionStringParser)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.</span>ConnectionStringParser (connectionString)](#apidoc.element.node-zookeeper-client.ConnectionStringParser.ConnectionStringParser)

#### [module node-zookeeper-client.ConnectionStringParser.prototype](#apidoc.module.node-zookeeper-client.ConnectionStringParser.prototype)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionStringParser.prototype.</span>getChrootPath ()](#apidoc.element.node-zookeeper-client.ConnectionStringParser.prototype.getChrootPath)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionStringParser.prototype.</span>getConnectionString ()](#apidoc.element.node-zookeeper-client.ConnectionStringParser.prototype.getConnectionString)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionStringParser.prototype.</span>getServers ()](#apidoc.element.node-zookeeper-client.ConnectionStringParser.prototype.getServers)

#### [module node-zookeeper-client.Event](#apidoc.module.node-zookeeper-client.Event)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.</span>Event (type, name, path)](#apidoc.element.node-zookeeper-client.Event.Event)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.Event.</span>create (watcherEvent)](#apidoc.element.node-zookeeper-client.Event.create)
1.  number <span class="apidocSignatureSpan">node-zookeeper-client.Event.</span>NODE_CHILDREN_CHANGED
1.  number <span class="apidocSignatureSpan">node-zookeeper-client.Event.</span>NODE_CREATED
1.  number <span class="apidocSignatureSpan">node-zookeeper-client.Event.</span>NODE_DATA_CHANGED
1.  number <span class="apidocSignatureSpan">node-zookeeper-client.Event.</span>NODE_DELETED

#### [module node-zookeeper-client.Event.prototype](#apidoc.module.node-zookeeper-client.Event.prototype)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.Event.prototype.</span>getName ()](#apidoc.element.node-zookeeper-client.Event.prototype.getName)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.Event.prototype.</span>getPath ()](#apidoc.element.node-zookeeper-client.Event.prototype.getPath)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.Event.prototype.</span>getType ()](#apidoc.element.node-zookeeper-client.Event.prototype.getType)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.Event.prototype.</span>toString ()](#apidoc.element.node-zookeeper-client.Event.prototype.toString)

#### [module node-zookeeper-client.Exception](#apidoc.module.node-zookeeper-client.Exception)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.</span>Exception (code, name, path, ctor)](#apidoc.element.node-zookeeper-client.Exception.Exception)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.Exception.</span>create (code, path)](#apidoc.element.node-zookeeper-client.Exception.create)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.Exception.</span>super_ ()](#apidoc.element.node-zookeeper-client.Exception.super_)
1.  number <span class="apidocSignatureSpan">node-zookeeper-client.Exception.</span>API_ERROR
1.  number <span class="apidocSignatureSpan">node-zookeeper-client.Exception.</span>AUTH_FAILED
1.  number <span class="apidocSignatureSpan">node-zookeeper-client.Exception.</span>BAD_ARGUMENTS
1.  number <span class="apidocSignatureSpan">node-zookeeper-client.Exception.</span>BAD_VERSION
1.  number <span class="apidocSignatureSpan">node-zookeeper-client.Exception.</span>CONNECTION_LOSS
1.  number <span class="apidocSignatureSpan">node-zookeeper-client.Exception.</span>DATA_INCONSISTENCY
1.  number <span class="apidocSignatureSpan">node-zookeeper-client.Exception.</span>INVALID_ACL
1.  number <span class="apidocSignatureSpan">node-zookeeper-client.Exception.</span>INVALID_CALLBACK
1.  number <span class="apidocSignatureSpan">node-zookeeper-client.Exception.</span>MARSHALLING_ERROR
1.  number <span class="apidocSignatureSpan">node-zookeeper-client.Exception.</span>NODE_EXISTS
1.  number <span class="apidocSignatureSpan">node-zookeeper-client.Exception.</span>NOT_EMPTY
1.  number <span class="apidocSignatureSpan">node-zookeeper-client.Exception.</span>NO_AUTH
1.  number <span class="apidocSignatureSpan">node-zookeeper-client.Exception.</span>NO_CHILDREN_FOR_EPHEMERALS
1.  number <span class="apidocSignatureSpan">node-zookeeper-client.Exception.</span>NO_NODE
1.  number <span class="apidocSignatureSpan">node-zookeeper-client.Exception.</span>OK
1.  number <span class="apidocSignatureSpan">node-zookeeper-client.Exception.</span>OPERATION_TIMEOUT
1.  number <span class="apidocSignatureSpan">node-zookeeper-client.Exception.</span>RUNTIME_INCONSISTENCY
1.  number <span class="apidocSignatureSpan">node-zookeeper-client.Exception.</span>SESSION_EXPIRED
1.  number <span class="apidocSignatureSpan">node-zookeeper-client.Exception.</span>SYSTEM_ERROR
1.  number <span class="apidocSignatureSpan">node-zookeeper-client.Exception.</span>UNIMPLEMENTED

#### [module node-zookeeper-client.Exception.prototype](#apidoc.module.node-zookeeper-client.Exception.prototype)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.Exception.prototype.</span>getCode ()](#apidoc.element.node-zookeeper-client.Exception.prototype.getCode)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.Exception.prototype.</span>getName ()](#apidoc.element.node-zookeeper-client.Exception.prototype.getName)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.Exception.prototype.</span>getPath ()](#apidoc.element.node-zookeeper-client.Exception.prototype.getPath)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.Exception.prototype.</span>toString ()](#apidoc.element.node-zookeeper-client.Exception.prototype.toString)

#### [module node-zookeeper-client.Exception.super_](#apidoc.module.node-zookeeper-client.Exception.super_)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.Exception.</span>super_ ()](#apidoc.element.node-zookeeper-client.Exception.super_.super_)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.Exception.super_.</span>captureStackTrace ()](#apidoc.element.node-zookeeper-client.Exception.super_.captureStackTrace)
1.  number <span class="apidocSignatureSpan">node-zookeeper-client.Exception.super_.</span>stackTraceLimit

#### [module node-zookeeper-client.Id](#apidoc.module.node-zookeeper-client.Id)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.</span>Id (scheme, id)](#apidoc.element.node-zookeeper-client.Id.Id)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.Id.</span>fromRecord (record)](#apidoc.element.node-zookeeper-client.Id.fromRecord)
1.  object <span class="apidocSignatureSpan">node-zookeeper-client.Id.</span>ANYONE_ID_UNSAFE
1.  object <span class="apidocSignatureSpan">node-zookeeper-client.Id.</span>AUTH_IDS

#### [module node-zookeeper-client.Id.prototype](#apidoc.module.node-zookeeper-client.Id.prototype)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.Id.prototype.</span>toRecord ()](#apidoc.element.node-zookeeper-client.Id.prototype.toRecord)

#### [module node-zookeeper-client.PacketQueue](#apidoc.module.node-zookeeper-client.PacketQueue)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.</span>PacketQueue ()](#apidoc.element.node-zookeeper-client.PacketQueue.PacketQueue)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.PacketQueue.</span>super_ ()](#apidoc.element.node-zookeeper-client.PacketQueue.super_)

#### [module node-zookeeper-client.PacketQueue.prototype](#apidoc.module.node-zookeeper-client.PacketQueue.prototype)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.PacketQueue.prototype.</span>push (packet)](#apidoc.element.node-zookeeper-client.PacketQueue.prototype.push)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.PacketQueue.prototype.</span>shift ()](#apidoc.element.node-zookeeper-client.PacketQueue.prototype.shift)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.PacketQueue.prototype.</span>unshift (packet)](#apidoc.element.node-zookeeper-client.PacketQueue.prototype.unshift)

#### [module node-zookeeper-client.Path](#apidoc.module.node-zookeeper-client.Path)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.Path.</span>validate (path)](#apidoc.element.node-zookeeper-client.Path.validate)

#### [module node-zookeeper-client.Transaction](#apidoc.module.node-zookeeper-client.Transaction)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.</span>Transaction (connectionManager)](#apidoc.element.node-zookeeper-client.Transaction.Transaction)

#### [module node-zookeeper-client.Transaction.prototype](#apidoc.module.node-zookeeper-client.Transaction.prototype)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.Transaction.prototype.</span>check (path, version)](#apidoc.element.node-zookeeper-client.Transaction.prototype.check)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.Transaction.prototype.</span>commit (callback)](#apidoc.element.node-zookeeper-client.Transaction.prototype.commit)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.Transaction.prototype.</span>create (path, data, acls, mode)](#apidoc.element.node-zookeeper-client.Transaction.prototype.create)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.Transaction.prototype.</span>remove (path, version)](#apidoc.element.node-zookeeper-client.Transaction.prototype.remove)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.Transaction.prototype.</span>setData (path, data, version)](#apidoc.element.node-zookeeper-client.Transaction.prototype.setData)

#### [module node-zookeeper-client.WatcherManager](#apidoc.module.node-zookeeper-client.WatcherManager)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.</span>WatcherManager ()](#apidoc.element.node-zookeeper-client.WatcherManager.WatcherManager)

#### [module node-zookeeper-client.WatcherManager.prototype](#apidoc.module.node-zookeeper-client.WatcherManager.prototype)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.WatcherManager.prototype.</span>emit (watcherEvent)](#apidoc.element.node-zookeeper-client.WatcherManager.prototype.emit)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.WatcherManager.prototype.</span>getChildWatcherPaths ()](#apidoc.element.node-zookeeper-client.WatcherManager.prototype.getChildWatcherPaths)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.WatcherManager.prototype.</span>getDataWatcherPaths ()](#apidoc.element.node-zookeeper-client.WatcherManager.prototype.getDataWatcherPaths)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.WatcherManager.prototype.</span>getExistenceWatcherPaths ()](#apidoc.element.node-zookeeper-client.WatcherManager.prototype.getExistenceWatcherPaths)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.WatcherManager.prototype.</span>isEmpty ()](#apidoc.element.node-zookeeper-client.WatcherManager.prototype.isEmpty)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.WatcherManager.prototype.</span>registerChildWatcher (path, watcher)](#apidoc.element.node-zookeeper-client.WatcherManager.prototype.registerChildWatcher)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.WatcherManager.prototype.</span>registerDataWatcher (path, watcher)](#apidoc.element.node-zookeeper-client.WatcherManager.prototype.registerDataWatcher)
1.  [function <span class="apidocSignatureSpan">node-zookeeper-client.WatcherManager.prototype.</span>registerExistenceWatcher (path, watcher)](#apidoc.element.node-zookeeper-client.WatcherManager.prototype.registerExistenceWatcher)



# <a name="apidoc.module.node-zookeeper-client"></a>[module node-zookeeper-client](#apidoc.module.node-zookeeper-client)

#### <a name="apidoc.element.node-zookeeper-client.ACL"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.</span>ACL (permission, id)](#apidoc.element.node-zookeeper-client.ACL)
- description and source-code
```javascript
function ACL(permission, id) {
    if (typeof permission !== 'number' || permission < 1 || permission > 31) {
        throw new Error('permission must be a valid integer.');
    }

    if (!(id instanceof Id)) {
        throw new Error('id must be an instance of Id class.');
    }

    this.permission = permission;
    this.id = id;
}
```
- example usage
```shell
...

**Example**

'''javascript
zookeeper.setACL(
'/test/demo',
[
    new zookeeper.ACL(
        zookeeeper.Permission.ADMIN,
        new zookeeper.Id('ip', '127.0.0.1')
    )
],
function (error, acls, stat) {
    if (error) {
        console.log(error.stack);
...
```

#### <a name="apidoc.element.node-zookeeper-client.ConnectionManager"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.</span>ConnectionManager (connectionString, options, stateListener)](#apidoc.element.node-zookeeper-client.ConnectionManager)
- description and source-code
```javascript
function ConnectionManager(connectionString, options, stateListener) {
    events.EventEmitter.call(this);

    this.watcherManager = new WatcherManager();
    this.connectionStringParser = new ConnectionStringParser(connectionString);

    this.servers = this.connectionStringParser.getServers();
    this.chrootPath = this.connectionStringParser.getChrootPath();
    this.nextServerIndex = 0;
    this.serverAttempts = 0;

    this.state = STATES.DISCONNECTED;

    this.options = options;
    this.spinDelay = options.spinDelay;

    this.updateTimeout(options.sessionTimeout);
    this.connectTimeoutHandler = null;

    this.xid = 0;

    this.sessionId = new Buffer(8);
    if (Buffer.isBuffer(options.sessionId)) {
        options.sessionId.copy(this.sessionId);
    } else {
        this.sessionId.fill(0);
    }

    this.sessionPassword = new Buffer(16);
    if (Buffer.isBuffer(options.sessionPassword)) {
        options.sessionPassword.copy(this.sessionPassword);
    } else {
        this.sessionPassword.fill(0);
    }

    // scheme:auth pairs
    this.credentials = [];

    // Last seen zxid.
    this.zxid = new Buffer(8);
    this.zxid.fill(0);


    this.pendingBuffer = null;

    this.packetQueue = new PacketQueue();
    this.packetQueue.on('readable', this.onPacketQueueReadable.bind(this));
    this.pendingQueue = [];

    this.on('state', stateListener);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-zookeeper-client.ConnectionStringParser"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.</span>ConnectionStringParser (connectionString)](#apidoc.element.node-zookeeper-client.ConnectionStringParser)
- description and source-code
```javascript
function ConnectionStringParser(connectionString) {
    assert(
        connectionString && typeof connectionString === 'string',
        'connectionString must be a non-empty string.'
    );

    this.connectionString = connectionString;

    // Handle chroot
    var index = connectionString.indexOf('/'),
        hostList = [],
        servers = [];

    if (index !== -1 && index !== (connectionString.length - 1)) {
        this.chrootPath = connectionString.substring(index);
        Path.validate(this.chrootPath);
    } else {
        this.chrootPath = undefined;
    }

    if (index !== -1) {
        hostList = connectionString.substring(0, index).split(',');
    } else {
        hostList = connectionString.split(',');
    }

    hostList.filter(function (item) {
        // Filter out empty string.
        return item;
    }).forEach(function (item) {
        var parts = item.split(':');
        servers.push({
            host : parts[0],
            port : parts[1] || DEFAULT_PORT
        });
    });

    assert(
        servers.length > 0,
        'connectionString must contain at least one server.'
    );

    // Randomize the list.
    this.servers = u.shuffle(servers);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-zookeeper-client.Event"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.</span>Event (type, name, path)](#apidoc.element.node-zookeeper-client.Event)
- description and source-code
```javascript
function Event(type, name, path) {
    validateType(type);
    assert(
        name && typeof name === 'string',
        'name must be a non-empty string.'
    );

    this.type = type;
    this.name = name;
    this.path = path;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-zookeeper-client.Exception"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.</span>Exception (code, name, path, ctor)](#apidoc.element.node-zookeeper-client.Exception)
- description and source-code
```javascript
function Exception(code, name, path, ctor) {
    if (!ctor) {
        ctor = path;
        path = undefined;
    }

    validateCode(code);
    assert(
        name && typeof name === 'string',
        'name must be a non-empty string.'
    );
    assert(typeof ctor === 'function', 'ctor must be a function.');

    Error.captureStackTrace(this, ctor || Exception);
    this.code = code;
    this.name = name;
    this.path = path;

    this.message = 'Exception: ' + name + '[' + code + ']';

    if (path) {
        this.message += '@' + path;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-zookeeper-client.Exception.super_"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.</span>Exception.super_ ()](#apidoc.element.node-zookeeper-client.Exception.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-zookeeper-client.Id"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.</span>Id (scheme, id)](#apidoc.element.node-zookeeper-client.Id)
- description and source-code
```javascript
function Id(scheme, id) {
    if (!scheme || typeof scheme !== 'string') {
        throw new Error('scheme must be a non-empty string.');
    }

    if (typeof id !== 'string') {
        throw new Error('id must be a string.');
    }

    this.scheme = scheme;
    this.id = id;
}
```
- example usage
```shell
...

'''javascript
zookeeper.setACL(
'/test/demo',
[
    new zookeeper.ACL(
        zookeeeper.Permission.ADMIN,
        new zookeeper.Id('ip', '127.0.0.1')
    )
],
function (error, acls, stat) {
    if (error) {
        console.log(error.stack);
        return;
    }
...
```

#### <a name="apidoc.element.node-zookeeper-client.PacketQueue"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.</span>PacketQueue ()](#apidoc.element.node-zookeeper-client.PacketQueue)
- description and source-code
```javascript
function PacketQueue() {
    events.EventEmitter.call(this);

    this.queue = [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-zookeeper-client.Transaction"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.</span>Transaction (connectionManager)](#apidoc.element.node-zookeeper-client.Transaction)
- description and source-code
```javascript
function Transaction(connectionManager) {
    if (!(this instanceof Transaction)) {
        return new Transaction(connectionManager);
    }

    assert(
        connectionManager instanceof ConnectionManager,
        'connectionManager must be an instance of ConnectionManager.'
    );

    this.ops = [];
    this.connectionManager = connectionManager;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-zookeeper-client.WatcherManager"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.</span>WatcherManager ()](#apidoc.element.node-zookeeper-client.WatcherManager)
- description and source-code
```javascript
function WatcherManager() {
    this.dataWatchers = {};
    this.childWatchers = {};
    this.existenceWatchers = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-zookeeper-client.createClient"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.</span>createClient (connectionString, options)](#apidoc.element.node-zookeeper-client.createClient)
- description and source-code
```javascript
function createClient(connectionString, options) {
    return new Client(connectionString, options);
}
```
- example usage
```shell
...
## Example

1\. Create a node using given path:

'''javascript
var zookeeper = require('node-zookeeper-client');

var client = zookeeper.createClient('localhost:2181');
var path = process.argv[2];

client.once('connected', function () {
console.log('Connected to the server.');

client.create(path, function (error) {
    if (error) {
...
```



# <a name="apidoc.module.node-zookeeper-client.ACL"></a>[module node-zookeeper-client.ACL](#apidoc.module.node-zookeeper-client.ACL)

#### <a name="apidoc.element.node-zookeeper-client.ACL.ACL"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.</span>ACL (permission, id)](#apidoc.element.node-zookeeper-client.ACL.ACL)
- description and source-code
```javascript
function ACL(permission, id) {
    if (typeof permission !== 'number' || permission < 1 || permission > 31) {
        throw new Error('permission must be a valid integer.');
    }

    if (!(id instanceof Id)) {
        throw new Error('id must be an instance of Id class.');
    }

    this.permission = permission;
    this.id = id;
}
```
- example usage
```shell
...

**Example**

'''javascript
zookeeper.setACL(
'/test/demo',
[
    new zookeeper.ACL(
        zookeeeper.Permission.ADMIN,
        new zookeeper.Id('ip', '127.0.0.1')
    )
],
function (error, acls, stat) {
    if (error) {
        console.log(error.stack);
...
```

#### <a name="apidoc.element.node-zookeeper-client.ACL.fromRecord"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.ACL.</span>fromRecord (record)](#apidoc.element.node-zookeeper-client.ACL.fromRecord)
- description and source-code
```javascript
function fromRecord(record) {
    if (!(record instanceof jute.data.ACL)) {
        throw new Error('record must be an instace of jute.data.ACL.');
    }

    return new ACL(record.perms, Id.fromRecord(record.id));
}
```
- example usage
```shell
...
            return;
        }

        var acls;

        if (Array.isArray(response.payload.acl)) {
            acls = response.payload.acl.map(function (item) {
                return ACL.fromRecord(item);
            });
        }

        next(null, acls, response.payload.stat);
    });
},
callback
...
```



# <a name="apidoc.module.node-zookeeper-client.ACL.prototype"></a>[module node-zookeeper-client.ACL.prototype](#apidoc.module.node-zookeeper-client.ACL.prototype)

#### <a name="apidoc.element.node-zookeeper-client.ACL.prototype.toRecord"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.ACL.prototype.</span>toRecord ()](#apidoc.element.node-zookeeper-client.ACL.prototype.toRecord)
- description and source-code
```javascript
toRecord = function () {
    return new jute.data.ACL(
        this.permission,
        this.id.toRecord()
    );
}
```
- example usage
```shell
...

header = new jute.protocol.RequestHeader();
header.type = jute.OP_CODES.CREATE;

payload = new jute.protocol.CreateRequest();
payload.path = path;
payload.acl = acls.map(function (item) {
    return item.toRecord();
});
payload.flags = mode;

if (Buffer.isBuffer(data)) {
    payload.data = new Buffer(data.length);
    data.copy(payload.data);
}
...
```



# <a name="apidoc.module.node-zookeeper-client.ConnectionManager"></a>[module node-zookeeper-client.ConnectionManager](#apidoc.module.node-zookeeper-client.ConnectionManager)

#### <a name="apidoc.element.node-zookeeper-client.ConnectionManager.ConnectionManager"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.</span>ConnectionManager (connectionString, options, stateListener)](#apidoc.element.node-zookeeper-client.ConnectionManager.ConnectionManager)
- description and source-code
```javascript
function ConnectionManager(connectionString, options, stateListener) {
    events.EventEmitter.call(this);

    this.watcherManager = new WatcherManager();
    this.connectionStringParser = new ConnectionStringParser(connectionString);

    this.servers = this.connectionStringParser.getServers();
    this.chrootPath = this.connectionStringParser.getChrootPath();
    this.nextServerIndex = 0;
    this.serverAttempts = 0;

    this.state = STATES.DISCONNECTED;

    this.options = options;
    this.spinDelay = options.spinDelay;

    this.updateTimeout(options.sessionTimeout);
    this.connectTimeoutHandler = null;

    this.xid = 0;

    this.sessionId = new Buffer(8);
    if (Buffer.isBuffer(options.sessionId)) {
        options.sessionId.copy(this.sessionId);
    } else {
        this.sessionId.fill(0);
    }

    this.sessionPassword = new Buffer(16);
    if (Buffer.isBuffer(options.sessionPassword)) {
        options.sessionPassword.copy(this.sessionPassword);
    } else {
        this.sessionPassword.fill(0);
    }

    // scheme:auth pairs
    this.credentials = [];

    // Last seen zxid.
    this.zxid = new Buffer(8);
    this.zxid.fill(0);


    this.pendingBuffer = null;

    this.packetQueue = new PacketQueue();
    this.packetQueue.on('readable', this.onPacketQueueReadable.bind(this));
    this.pendingQueue = [];

    this.on('state', stateListener);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-zookeeper-client.ConnectionManager.super_"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.</span>super_ ()](#apidoc.element.node-zookeeper-client.ConnectionManager.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-zookeeper-client.ConnectionManager.prototype"></a>[module node-zookeeper-client.ConnectionManager.prototype](#apidoc.module.node-zookeeper-client.ConnectionManager.prototype)

#### <a name="apidoc.element.node-zookeeper-client.ConnectionManager.prototype.addAuthInfo"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>addAuthInfo (scheme, auth)](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.addAuthInfo)
- description and source-code
```javascript
addAuthInfo = function (scheme, auth) {
    if (!scheme || typeof scheme !== 'string') {
        throw new Error('scheme must be a non-empty string.');
    }

    if (!Buffer.isBuffer(auth)) {
        throw new Error('auth must be a valid instance of Buffer');
    }

    var header,
        payload,
        request;

    this.credentials.push({
        scheme : scheme,
        auth : auth
    });

    switch (this.state) {
    case STATES.CONNECTED:
    case STATES.CONNECTED_READ_ONLY:
        // Only queue the auth request when connected.
        header = new jute.protocol.RequestHeader();
        payload = new jute.protocol.AuthPacket();

        header.xid = jute.XID_AUTHENTICATION;
        header.type = jute.OP_CODES.AUTH;

        payload.type = 0;
        payload.scheme = scheme;
        payload.auth = auth;

        this.queue(new jute.Request(header, payload));
        break;
    case STATES.DISCONNECTED:
    case STATES.CONNECTING:
    case STATES.CLOSING:
    case STATES.CLOSED:
    case STATES.SESSION_EXPIRED:
    case STATES.AUTHENTICATION_FAILED:
        // Skip when we are not in a live state.
        return;
    default:
        throw new Error('Unknown state: ' + this.state);
    }
}
```
- example usage
```shell
...

* scheme 'String' - The authentication scheme.
* auth 'Buffer' - The authentication data buffer.

**Example**

'''javascript
zookeeper.addAuthInfo('ip', new Buffer('127.0.0.1'));
'''

---

#### State getState()

Return the current client [state](#state).
...
```

#### <a name="apidoc.element.node-zookeeper-client.ConnectionManager.prototype.cleanupPendingQueue"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>cleanupPendingQueue (errorCode)](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.cleanupPendingQueue)
- description and source-code
```javascript
cleanupPendingQueue = function (errorCode) {
    var pendingPacket = this.pendingQueue.shift();

    while (pendingPacket) {
        if (pendingPacket.callback) {
            pendingPacket.callback(Exception.create(errorCode));
        }

        pendingPacket = this.pendingQueue.shift();
    }
}
```
- example usage
```shell
...
    retry = false;
    break;
default:
    errorCode = Exception.CONNECTION_LOSS;
    retry = true;
}

this.cleanupPendingQueue(errorCode);
this.setState(STATES.DISCONNECTED);

if (retry) {
    this.connect();
} else {
    this.setState(STATES.CLOSED);
}
...
```

#### <a name="apidoc.element.node-zookeeper-client.ConnectionManager.prototype.close"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>close ()](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.close)
- description and source-code
```javascript
close = function () {
    var self = this,
        header = new jute.protocol.RequestHeader(),
        request;

    self.setState(STATES.CLOSING);

    header.type = jute.OP_CODES.CLOSE_SESSION;
    request = new jute.Request(header, null);

    self.queue(request);
}
```
- example usage
```shell
...
    client.create(path, function (error) {
        if (error) {
            console.log('Failed to create node: %s due to: %s.', path, error);
        } else {
            console.log('Node: %s is successfully created.', path);
        }

        client.close();
    });
});

client.connect();
'''

2\. List and watch the children of given node:
...
```

#### <a name="apidoc.element.node-zookeeper-client.ConnectionManager.prototype.connect"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>connect ()](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.connect)
- description and source-code
```javascript
connect = function () {
    var self = this;

    self.setState(STATES.CONNECTING);

    self.findNextServer(function (server) {
        self.socket = net.connect(server);

        self.connectTimeoutHandler = setTimeout(
            self.onSocketConnectTimeout.bind(self),
            self.connectTimeout
        );

        // Disable the Nagle algorithm.
        self.socket.setNoDelay();

        self.socket.on('connect', self.onSocketConnected.bind(self));
        self.socket.on('data', self.onSocketData.bind(self));
        self.socket.on('drain', self.onSocketDrain.bind(self));
        self.socket.on('close', self.onSocketClosed.bind(self));
        self.socket.on('error', self.onSocketError.bind(self));
    });
}
```
- example usage
```shell
...
            console.log('Node: %s is successfully created.', path);
        }

        client.close();
    });
});

client.connect();
'''

2\. List and watch the children of given node:

'''javascript
var zookeeper = require('node-zookeeper-client');
...
```

#### <a name="apidoc.element.node-zookeeper-client.ConnectionManager.prototype.findNextServer"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>findNextServer (callback)](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.findNextServer)
- description and source-code
```javascript
findNextServer = function (callback) {
    var self = this;

    self.nextServerIndex %= self.servers.length;

    if (self.serverAttempts === self.servers.length) {
        setTimeout(function () {
            callback(self.servers[self.nextServerIndex]);
            self.nextServerIndex += 1;

            // reset attempts since we already waited for enough time.
            self.serverAttempts = 0;
        }, Math.random() * self.spinDelay);
    } else {
        self.serverAttempts += 1;

        process.nextTick(function () {
            callback(self.servers[self.nextServerIndex]);
            self.nextServerIndex += 1;
        });
    }
}
```
- example usage
```shell
...
};

ConnectionManager.prototype.connect = function () {
    var self = this;

    self.setState(STATES.CONNECTING);

    self.findNextServer(function (server) {
self.socket = net.connect(server);

self.connectTimeoutHandler = setTimeout(
    self.onSocketConnectTimeout.bind(self),
    self.connectTimeout
);
...
```

#### <a name="apidoc.element.node-zookeeper-client.ConnectionManager.prototype.getSessionId"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>getSessionId ()](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.getSessionId)
- description and source-code
```javascript
getSessionId = function () {
    var result = new Buffer(8);

    this.sessionId.copy(result);
    return result;
}
```
- example usage
```shell
...
['Buffer'](http://nodejs.org/api/buffer.html) since Javascript does not support
long integer natively.

**Example**

'''javascript
var client = zookeeper.createClient({...});
var id = client.getSessionId();
console.log('Session id is: %s', id.toString('hex'));
'''

---

#### Buffer getSessionPassword()
...
```

#### <a name="apidoc.element.node-zookeeper-client.ConnectionManager.prototype.getSessionPassword"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>getSessionPassword ()](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.getSessionPassword)
- description and source-code
```javascript
getSessionPassword = function () {
    var result = new Buffer(16);

    this.sessionPassword.copy(result);
    return result;
}
```
- example usage
```shell
...
The value returned is an instance of
['Buffer'](http://nodejs.org/api/buffer.html).

**Example**

'''javascript
var client = zookeeper.createClient({...});
var pwd = client.getSessionPassword();
'''

---

#### Number getSessionTimeout()

Returns the *negotiated* session timeout (in milliseconds) for this client
...
```

#### <a name="apidoc.element.node-zookeeper-client.ConnectionManager.prototype.getSessionTimeout"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>getSessionTimeout ()](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.getSessionTimeout)
- description and source-code
```javascript
getSessionTimeout = function () {
    return this.sessionTimeout;
}
```
- example usage
```shell
...
instance. The value returned is not valid until the client connects to a server
and may change after a re-connect.

**Example**

'''javascript
var client = zookeeper.createClient({...});
var sessionTimeout = client.getSessionTimeout();
'''

---

### State

After the 'connect()' method is invoked, the ZooKeeper client starts its
...
```

#### <a name="apidoc.element.node-zookeeper-client.ConnectionManager.prototype.onPacketQueueReadable"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>onPacketQueueReadable ()](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.onPacketQueueReadable)
- description and source-code
```javascript
onPacketQueueReadable = function () {
    var packet,
        header;

    switch (this.state) {
    case STATES.CONNECTED:
    case STATES.CONNECTED_READ_ONLY:
    case STATES.CLOSING:
        // Continue
        break;
    case STATES.DISCONNECTED:
    case STATES.CONNECTING:
    case STATES.CLOSED:
    case STATES.SESSION_EXPIRED:
    case STATES.AUTHENTICATION_FAILED:
        // Skip since we can not send traffic out
        return;
    default:
        throw new Error('Unknown state: ' + this.state);
    }

    while ((packet = this.packetQueue.shift()) !== undefined) {
        header = packet.request.header;
        if (header !== null &&
                header.type !== jute.OP_CODES.PING &&
                header.type !== jute.OP_CODES.AUTH) {

            header.xid = this.xid;
            this.xid += 1;

            // Only put requests that are not connect, ping and auth into
            // the pending queue.
            this.pendingQueue.push(packet);
        }

        if (!this.socket.write(packet.request.toBuffer())) {
            // Back pressure is handled here, when the socket emit
            // drain event, this method will be invoked again.
            break;
        }

        if (header.type === jute.OP_CODES.CLOSE_SESSION) {
            // The close session should be the final packet sent to the
            // server.
            break;
        }
    }
}
```
- example usage
```shell
...
    self.sessionId = connectResponse.sessionId;
    self.sessionPassword = connectResponse.passwd;
    self.updateTimeout(connectResponse.timeOut);

    self.setState(STATES.CONNECTED);

    // Check if we have anything to send out just in case.
    self.onPacketQueueReadable();

    self.socket.setTimeout(
        self.pingTimeout,
        self.onSocketTimeout.bind(self)
    );

}
...
```

#### <a name="apidoc.element.node-zookeeper-client.ConnectionManager.prototype.onSocketClosed"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>onSocketClosed (hasError)](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.onSocketClosed)
- description and source-code
```javascript
onSocketClosed = function (hasError) {
    var retry = false,
        errorCode,
        pendingPacket;

    switch (this.state) {
    case STATES.CLOSING:
        errorCode = Exception.CONNECTION_LOSS;
        retry = false;
        break;
    case STATES.SESSION_EXPIRED:
        errorCode = Exception.SESSION_EXPIRED;
        retry = false;
        break;
    case STATES.AUTHENTICATION_FAILED:
        errorCode = Exception.AUTH_FAILED;
        retry = false;
        break;
    default:
        errorCode = Exception.CONNECTION_LOSS;
        retry = true;
    }

    this.cleanupPendingQueue(errorCode);
    this.setState(STATES.DISCONNECTED);

    if (retry) {
        this.connect();
    } else {
        this.setState(STATES.CLOSED);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-zookeeper-client.ConnectionManager.prototype.onSocketConnectTimeout"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>onSocketConnectTimeout ()](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.onSocketConnectTimeout)
- description and source-code
```javascript
onSocketConnectTimeout = function () {
    // Destroy the current socket so the socket closed event
    // will be trigger.
    this.socket.destroy();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-zookeeper-client.ConnectionManager.prototype.onSocketConnected"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>onSocketConnected ()](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.onSocketConnected)
- description and source-code
```javascript
onSocketConnected = function () {
    var connectRequest,
        authRequest,
        setWatchesRequest,
        header,
        payload;

    if (this.connectTimeoutHandler) {
        clearTimeout(this.connectTimeoutHandler);
    }

    connectRequest = new jute.Request(null, new jute.protocol.ConnectRequest(
        jute.PROTOCOL_VERSION,
        this.zxid,
        this.sessionTimeout,
        this.sessionId,
        this.sessionPassword
    ));

    // XXX No read only support yet.
    this.socket.write(connectRequest.toBuffer());

    // Set auth info
    if (this.credentials.length > 0) {
        this.credentials.forEach(function (credential) {
            header = new jute.protocol.RequestHeader();
            payload = new jute.protocol.AuthPacket();

            header.xid = jute.XID_AUTHENTICATION;
            header.type = jute.OP_CODES.AUTH;

            payload.type = 0;
            payload.scheme = credential.scheme;
            payload.auth = credential.auth;

            authRequest = new jute.Request(header, payload);
            this.queue(authRequest);

        },  this);
    }

    // Reset the watchers if we have any.
    if (!this.watcherManager.isEmpty()) {
        header = new jute.protocol.RequestHeader();
        payload = new jute.protocol.SetWatches();

        header.type = jute.OP_CODES.SET_WATCHES;
        header.xid = jute.XID_SET_WATCHES;

        payload.setChrootPath(this.chrootPath);
        payload.relativeZxid = this.zxid;
        payload.dataWatches = this.watcherManager.getDataWatcherPaths();
        payload.existWatches = this.watcherManager.getExistenceWatcherPaths();
        payload.childWatches = this.watcherManager.getChildWatcherPaths();

        setWatchesRequest = new jute.Request(header, payload);
        this.queue(setWatchesRequest);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-zookeeper-client.ConnectionManager.prototype.onSocketData"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>onSocketData (buffer)](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.onSocketData)
- description and source-code
```javascript
onSocketData = function (buffer) {
    var self = this,
        offset = 0,
        size = 0,
        connectResponse,
        pendingPacket,
        responseHeader,
        responsePayload,
        response,
        event;

    // Combine the pending buffer with the new buffer.
    if (self.pendingBuffer) {
        buffer = Buffer.concat(
            [self.pendingBuffer, buffer],
            self.pendingBuffer.length + buffer.length
        );
    }

    // We need at least 4 bytes
    if (buffer.length < 4) {
        self.pendingBuffer = buffer;
        return;
    }

    size = buffer.readInt32BE(offset);
    offset += 4;

    if (buffer.length < size + 4) {
        // More data are coming.
        self.pendingBuffer = buffer;
        return;
    }

    if (buffer.length === size + 4) {
        // The size is perfect.
        self.pendingBuffer = null;
    } else {
        // We have extra bytes, splice them out as pending buffer.
        self.pendingBuffer = buffer.slice(size + 4);
        buffer = buffer.slice(0, size + 4);
    }

    if (self.state === STATES.CONNECTING) {
        // Handle connect response.
        connectResponse = new jute.protocol.ConnectResponse();
        offset += connectResponse.deserialize(buffer, offset);


        if (connectResponse.timeOut <= 0) {
            self.setState(STATES.SESSION_EXPIRED);

        } else {
            // Reset the server connection attempts since we connected now.
            self.serverAttempts = 0;

            self.sessionId = connectResponse.sessionId;
            self.sessionPassword = connectResponse.passwd;
            self.updateTimeout(connectResponse.timeOut);

            self.setState(STATES.CONNECTED);

            // Check if we have anything to send out just in case.
            self.onPacketQueueReadable();

            self.socket.setTimeout(
                self.pingTimeout,
                self.onSocketTimeout.bind(self)
            );

        }
    } else {
        // Handle  all other repsonses.
        responseHeader = new jute.protocol.ReplyHeader();
        offset += responseHeader.deserialize(buffer, offset);

        //TODO BETTTER LOGGING
        switch (responseHeader.xid) {
        case jute.XID_PING:
            break;
        case jute.XID_AUTHENTICATION:
            if (responseHeader.err === Exception.AUTH_FAILED) {
                self.setState(STATES.AUTHENTICATION_FAILED);
            }
            break;
        case jute.XID_NOTIFICATION:
            event = new jute.protocol.WatcherEvent();

            if (self.chrootPath) {
                event.setChrootPath(self.chrootPath);
            }

            offset += event.deserialize(buffer, offset);
            self.watcherManager.emit(event);
            break;
        default:
            pendingPacket = self.pendingQueue.shift();

            if (!pendingPacket) {
                // TODO, better error handling and logging need to be done.
                // Need to clean up and do a reconnect.
                // throw new Error(
                //    'Nothing in pending queue but got data from server.'
                // );
                self.socket.destroy(); // this will trigger reconnect
                return;
            }

            if (pendingPacket.request.header.xid !== responseHeader.xid) {
                // TODO, better error handling/logging need to bee done here.
                // Need to clean up and do a reconnect.
                //throw new Error(
                    //'Xid out of order. Got xid: ' +
                        //responseHeader.xid + ' with error code: ' +
                        //responseHeader.err + ', expected xid: ' +
                        //pendingPacket.request.header.xid + '.'
                //);
                self.socket.destroy(); // this will trigger reconnect
                return;
            }

            if (responseHeader.zxid) {
                // TODO, In Java implementation, the condition is to
                // check whether the long zxid is greater than 0, here
                // use buffer so we simplify. ...
```
- example usage
```shell
...
                }
            }
        }
    }

    // We have more data to process, need to recursively process it.
    if (self.pendingBuffer) {
        self.onSocketData(new Buffer(0));
    }
};

ConnectionManager.prototype.onSocketDrain = function () {
    // Trigger write on socket.
    this.onPacketQueueReadable();
};
...
```

#### <a name="apidoc.element.node-zookeeper-client.ConnectionManager.prototype.onSocketDrain"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>onSocketDrain ()](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.onSocketDrain)
- description and source-code
```javascript
onSocketDrain = function () {
    // Trigger write on socket.
    this.onPacketQueueReadable();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-zookeeper-client.ConnectionManager.prototype.onSocketError"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>onSocketError (error)](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.onSocketError)
- description and source-code
```javascript
onSocketError = function (error) {
    if (this.connectTimeoutHandler) {
        clearTimeout(this.connectTimeoutHandler);
    }

    // After socket error, the socket closed event will be triggered,
    // we will retry connect in that listener function.
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-zookeeper-client.ConnectionManager.prototype.onSocketTimeout"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>onSocketTimeout ()](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.onSocketTimeout)
- description and source-code
```javascript
onSocketTimeout = function () {
    var header,
        request;

    if (this.socket &&
            (this.state === STATES.CONNECTED ||
             this.state === STATES.CONNECTED_READ_ONLY)) {
        header = new jute.protocol.RequestHeader(
            jute.XID_PING,
            jute.OP_CODES.PING
        );

        request = new jute.Request(header, null);
        this.queue(request);

        // Re-register the timeout handler since it only fired once.
        this.socket.setTimeout(
            this.pingTimeout,
            this.onSocketTimeout.bind(this)
        );
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-zookeeper-client.ConnectionManager.prototype.queue"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>queue (request, callback)](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.queue)
- description and source-code
```javascript
queue = function (request, callback) {
    if (typeof request !== 'object') {
        throw new Error('request must be a valid instance of jute.Request.');
    }

    if (this.chrootPath && request.payload) {
        request.payload.setChrootPath(this.chrootPath);
    }


    callback = callback || function () {};

    switch (this.state) {
    case STATES.DISCONNECTED:
    case STATES.CONNECTING:
    case STATES.CONNECTED:
    case STATES.CONNECTED_READ_ONLY:
        // queue the packet
        this.packetQueue.push({
            request : request,
            callback : callback
        });
        break;
    case STATES.CLOSING:
        if (request.header &&
                request.header.type === jute.OP_CODES.CLOSE_SESSION) {
            this.packetQueue.push({
                request : request,
                callback : callback
            });
        } else {
            callback(Exception.create(Exception.CONNECTION_LOSS));
        }
        break;
    case STATES.CLOSED:
        callback(Exception.create(Exception.CONNECTION_LOSS));
        return;
    case STATES.SESSION_EXPIRED:
        callback(Exception.create(Exception.SESSION_EXPIRED));
        return;
    case STATES.AUTHENTICATION_FAILED:
        callback(Exception.create(Exception.AUTH_FAILED));
        return;
    default:
        throw new Error('Unknown state: ' + this.state);
    }
}
```
- example usage
```shell
...
    }

    request = new jute.Request(header, payload);

    attempt(
        self,
        function (attempts, next) {
self.connectionManager.queue(request, function (error, response) {
    if (error) {
        next(error);
        return;
    }

    next(null, response.payload.path);
});
...
```

#### <a name="apidoc.element.node-zookeeper-client.ConnectionManager.prototype.registerChildWatcher"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>registerChildWatcher (path, watcher)](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.registerChildWatcher)
- description and source-code
```javascript
registerChildWatcher = function (path, watcher) {
    this.watcherManager.registerChildWatcher(path, watcher);
}
```
- example usage
```shell
...
        self.connectionManager.queue(request, function (error, response) {
            if (error) {
                next(error);
                return;
            }

            if (watcher) {
                self.connectionManager.registerChildWatcher(path, watcher);
            }

            next(null, response.payload.children, response.payload.stat);
        });
    },
    callback
);
...
```

#### <a name="apidoc.element.node-zookeeper-client.ConnectionManager.prototype.registerDataWatcher"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>registerDataWatcher (path, watcher)](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.registerDataWatcher)
- description and source-code
```javascript
registerDataWatcher = function (path, watcher) {
    this.watcherManager.registerDataWatcher(path, watcher);
}
```
- example usage
```shell
...
        self.connectionManager.queue(request, function (error, response) {
            if (error) {
                next(error);
                return;
            }

            if (watcher) {
                self.connectionManager.registerDataWatcher(path, watcher);
            }

            next(null, response.payload.data, response.payload.stat);
        });
    },
    callback
);
...
```

#### <a name="apidoc.element.node-zookeeper-client.ConnectionManager.prototype.registerExistenceWatcher"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>registerExistenceWatcher (path, watcher)](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.registerExistenceWatcher)
- description and source-code
```javascript
registerExistenceWatcher = function (path, watcher) {
    this.watcherManager.registerExistenceWatcher(path, watcher);
}
```
- example usage
```shell
...
if (watcher) {
    if (existence) {
        self.connectionManager.registerDataWatcher(
            path,
            watcher
        );
    } else {
        self.connectionManager.registerExistenceWatcher(
            path,
            watcher
        );
    }
}

next(
...
```

#### <a name="apidoc.element.node-zookeeper-client.ConnectionManager.prototype.setState"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>setState (state)](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.setState)
- description and source-code
```javascript
setState = function (state) {
    if (typeof state !== 'number') {
        throw new Error('state must be a valid number.');
    }

    if (this.state !== state) {
        this.state = state;
        this.emit('state', this.state);
    }
}
```
- example usage
```shell
...
ConnectionManager.prototype.getSessionTimeout = function () {
    return this.sessionTimeout;
};

ConnectionManager.prototype.connect = function () {
    var self = this;

    self.setState(STATES.CONNECTING);

    self.findNextServer(function (server) {
self.socket = net.connect(server);

self.connectTimeoutHandler = setTimeout(
    self.onSocketConnectTimeout.bind(self),
    self.connectTimeout
...
```

#### <a name="apidoc.element.node-zookeeper-client.ConnectionManager.prototype.updateTimeout"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionManager.prototype.</span>updateTimeout (sessionTimeout)](#apidoc.element.node-zookeeper-client.ConnectionManager.prototype.updateTimeout)
- description and source-code
```javascript
updateTimeout = function (sessionTimeout) {
    this.sessionTimeout = sessionTimeout;

    // Designed to have time to try all the servers.
    this.connectTimeout = Math.floor(sessionTimeout / this.servers.length);

    // We at least send out one ping one third of the session timeout, so
    // the read timeout is two third of the session timeout.
    this.pingTimeout = Math.floor(this.sessionTimeout / 3);
    //this.readTimeout = Math.floor(sessionTimeout * 2 / 3);
}
```
- example usage
```shell
...
this.serverAttempts = 0;

this.state = STATES.DISCONNECTED;

this.options = options;
this.spinDelay = options.spinDelay;

this.updateTimeout(options.sessionTimeout);
this.connectTimeoutHandler = null;

this.xid = 0;

this.sessionId = new Buffer(8);
if (Buffer.isBuffer(options.sessionId)) {
    options.sessionId.copy(this.sessionId);
...
```



# <a name="apidoc.module.node-zookeeper-client.ConnectionStringParser"></a>[module node-zookeeper-client.ConnectionStringParser](#apidoc.module.node-zookeeper-client.ConnectionStringParser)

#### <a name="apidoc.element.node-zookeeper-client.ConnectionStringParser.ConnectionStringParser"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.</span>ConnectionStringParser (connectionString)](#apidoc.element.node-zookeeper-client.ConnectionStringParser.ConnectionStringParser)
- description and source-code
```javascript
function ConnectionStringParser(connectionString) {
    assert(
        connectionString && typeof connectionString === 'string',
        'connectionString must be a non-empty string.'
    );

    this.connectionString = connectionString;

    // Handle chroot
    var index = connectionString.indexOf('/'),
        hostList = [],
        servers = [];

    if (index !== -1 && index !== (connectionString.length - 1)) {
        this.chrootPath = connectionString.substring(index);
        Path.validate(this.chrootPath);
    } else {
        this.chrootPath = undefined;
    }

    if (index !== -1) {
        hostList = connectionString.substring(0, index).split(',');
    } else {
        hostList = connectionString.split(',');
    }

    hostList.filter(function (item) {
        // Filter out empty string.
        return item;
    }).forEach(function (item) {
        var parts = item.split(':');
        servers.push({
            host : parts[0],
            port : parts[1] || DEFAULT_PORT
        });
    });

    assert(
        servers.length > 0,
        'connectionString must contain at least one server.'
    );

    // Randomize the list.
    this.servers = u.shuffle(servers);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-zookeeper-client.ConnectionStringParser.prototype"></a>[module node-zookeeper-client.ConnectionStringParser.prototype](#apidoc.module.node-zookeeper-client.ConnectionStringParser.prototype)

#### <a name="apidoc.element.node-zookeeper-client.ConnectionStringParser.prototype.getChrootPath"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionStringParser.prototype.</span>getChrootPath ()](#apidoc.element.node-zookeeper-client.ConnectionStringParser.prototype.getChrootPath)
- description and source-code
```javascript
getChrootPath = function () {
    return this.chrootPath;
}
```
- example usage
```shell
...
function ConnectionManager(connectionString, options, stateListener) {
events.EventEmitter.call(this);

this.watcherManager = new WatcherManager();
this.connectionStringParser = new ConnectionStringParser(connectionString);

this.servers = this.connectionStringParser.getServers();
this.chrootPath = this.connectionStringParser.getChrootPath();
this.nextServerIndex = 0;
this.serverAttempts = 0;

this.state = STATES.DISCONNECTED;

this.options = options;
this.spinDelay = options.spinDelay;
...
```

#### <a name="apidoc.element.node-zookeeper-client.ConnectionStringParser.prototype.getConnectionString"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionStringParser.prototype.</span>getConnectionString ()](#apidoc.element.node-zookeeper-client.ConnectionStringParser.prototype.getConnectionString)
- description and source-code
```javascript
getConnectionString = function () {
    return this.connectionString;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-zookeeper-client.ConnectionStringParser.prototype.getServers"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.ConnectionStringParser.prototype.</span>getServers ()](#apidoc.element.node-zookeeper-client.ConnectionStringParser.prototype.getServers)
- description and source-code
```javascript
getServers = function () {
    return this.servers.slice(0);
}
```
- example usage
```shell
...
 */
function ConnectionManager(connectionString, options, stateListener) {
events.EventEmitter.call(this);

this.watcherManager = new WatcherManager();
this.connectionStringParser = new ConnectionStringParser(connectionString);

this.servers = this.connectionStringParser.getServers();
this.chrootPath = this.connectionStringParser.getChrootPath();
this.nextServerIndex = 0;
this.serverAttempts = 0;

this.state = STATES.DISCONNECTED;

this.options = options;
...
```



# <a name="apidoc.module.node-zookeeper-client.Event"></a>[module node-zookeeper-client.Event](#apidoc.module.node-zookeeper-client.Event)

#### <a name="apidoc.element.node-zookeeper-client.Event.Event"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.</span>Event (type, name, path)](#apidoc.element.node-zookeeper-client.Event.Event)
- description and source-code
```javascript
function Event(type, name, path) {
    validateType(type);
    assert(
        name && typeof name === 'string',
        'name must be a non-empty string.'
    );

    this.type = type;
    this.name = name;
    this.path = path;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-zookeeper-client.Event.create"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.Event.</span>create (watcherEvent)](#apidoc.element.node-zookeeper-client.Event.create)
- description and source-code
```javascript
function create(watcherEvent) {
    assert(watcherEvent, 'watcherEvent must be a valid object.');
    validateType(watcherEvent.type);

    var name,
        i = 0,
        keys = Object.keys(TYPES);

    while (i < keys.length) {
        if (TYPES[keys[i]] === watcherEvent.type) {
            name = keys[i];
            break;
        }

        i += 1;
    }

    return new Event(watcherEvent.type, name, watcherEvent.path);
}
```
- example usage
```shell
...

var client = zookeeper.createClient('localhost:2181');
var path = process.argv[2];

client.once('connected', function () {
    console.log('Connected to the server.');

    client.create(path, function (error) {
if (error) {
    console.log('Failed to create node: %s due to: %s.', path, error);
} else {
    console.log('Node: %s is successfully created.', path);
}

client.close();
...
```



# <a name="apidoc.module.node-zookeeper-client.Event.prototype"></a>[module node-zookeeper-client.Event.prototype](#apidoc.module.node-zookeeper-client.Event.prototype)

#### <a name="apidoc.element.node-zookeeper-client.Event.prototype.getName"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.Event.prototype.</span>getName ()](#apidoc.element.node-zookeeper-client.Event.prototype.getName)
- description and source-code
```javascript
getName = function () {
    return this.name;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-zookeeper-client.Event.prototype.getPath"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.Event.prototype.</span>getPath ()](#apidoc.element.node-zookeeper-client.Event.prototype.getPath)
- description and source-code
```javascript
getPath = function () {
    return this.path;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-zookeeper-client.Event.prototype.getType"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.Event.prototype.</span>getType ()](#apidoc.element.node-zookeeper-client.Event.prototype.getType)
- description and source-code
```javascript
getType = function () {
    return this.type;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-zookeeper-client.Event.prototype.toString"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.Event.prototype.</span>toString ()](#apidoc.element.node-zookeeper-client.Event.prototype.toString)
- description and source-code
```javascript
toString = function () {
    var result = this.name + '[' + this.type + ']';

    if (this.path) {
        result += '@' + this.path;
    }

    return result;
}
```
- example usage
```shell
...
    },
    function (error, data, stat) {
        if (error) {
            console.log(error.stack);
            return;
        }

        console.log('Got data: %s', data.toString('utf8'));
    }
);
'''

---

#### void setData(path, data, [version], callback)
...
```



# <a name="apidoc.module.node-zookeeper-client.Exception"></a>[module node-zookeeper-client.Exception](#apidoc.module.node-zookeeper-client.Exception)

#### <a name="apidoc.element.node-zookeeper-client.Exception.Exception"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.</span>Exception (code, name, path, ctor)](#apidoc.element.node-zookeeper-client.Exception.Exception)
- description and source-code
```javascript
function Exception(code, name, path, ctor) {
    if (!ctor) {
        ctor = path;
        path = undefined;
    }

    validateCode(code);
    assert(
        name && typeof name === 'string',
        'name must be a non-empty string.'
    );
    assert(typeof ctor === 'function', 'ctor must be a function.');

    Error.captureStackTrace(this, ctor || Exception);
    this.code = code;
    this.name = name;
    this.path = path;

    this.message = 'Exception: ' + name + '[' + code + ']';

    if (path) {
        this.message += '@' + path;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-zookeeper-client.Exception.create"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.Exception.</span>create (code, path)](#apidoc.element.node-zookeeper-client.Exception.create)
- description and source-code
```javascript
function create(code, path) {
    validateCode(code);

    var name,
        i = 0,
        keys = Object.keys(CODES);

    while (i < keys.length) {
        if (CODES[keys[i]] === code) {
            name = keys[i];
            break;
        }

        i += 1;
    }

    return new Exception(code, name, path, create);
}
```
- example usage
```shell
...

var client = zookeeper.createClient('localhost:2181');
var path = process.argv[2];

client.once('connected', function () {
    console.log('Connected to the server.');

    client.create(path, function (error) {
if (error) {
    console.log('Failed to create node: %s due to: %s.', path, error);
} else {
    console.log('Node: %s is successfully created.', path);
}

client.close();
...
```

#### <a name="apidoc.element.node-zookeeper-client.Exception.super_"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.Exception.</span>super_ ()](#apidoc.element.node-zookeeper-client.Exception.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-zookeeper-client.Exception.prototype"></a>[module node-zookeeper-client.Exception.prototype](#apidoc.module.node-zookeeper-client.Exception.prototype)

#### <a name="apidoc.element.node-zookeeper-client.Exception.prototype.getCode"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.Exception.prototype.</span>getCode ()](#apidoc.element.node-zookeeper-client.Exception.prototype.getCode)
- description and source-code
```javascript
getCode = function () {
    return this.code;
}
```
- example usage
```shell
...
* 'Exception.AUTH_FAILED'

**Example**

'''javascript
zookeeper.create('/test/demo', function (error, path) {
if (error) {
    if (error.getCode() == zookeeper.Exception.NODE_EXISTS) {
        console.log('Node exists.');
    } else {
        console.log(error.stack);
    }
    return;
}
...
```

#### <a name="apidoc.element.node-zookeeper-client.Exception.prototype.getName"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.Exception.prototype.</span>getName ()](#apidoc.element.node-zookeeper-client.Exception.prototype.getName)
- description and source-code
```javascript
getName = function () {
    return this.name;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-zookeeper-client.Exception.prototype.getPath"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.Exception.prototype.</span>getPath ()](#apidoc.element.node-zookeeper-client.Exception.prototype.getPath)
- description and source-code
```javascript
getPath = function () {
    return this.path;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-zookeeper-client.Exception.prototype.toString"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.Exception.prototype.</span>toString ()](#apidoc.element.node-zookeeper-client.Exception.prototype.toString)
- description and source-code
```javascript
toString = function () {
    return this.message;
}
```
- example usage
```shell
...
    },
    function (error, data, stat) {
        if (error) {
            console.log(error.stack);
            return;
        }

        console.log('Got data: %s', data.toString('utf8'));
    }
);
'''

---

#### void setData(path, data, [version], callback)
...
```



# <a name="apidoc.module.node-zookeeper-client.Exception.super_"></a>[module node-zookeeper-client.Exception.super_](#apidoc.module.node-zookeeper-client.Exception.super_)

#### <a name="apidoc.element.node-zookeeper-client.Exception.super_.super_"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.Exception.</span>super_ ()](#apidoc.element.node-zookeeper-client.Exception.super_.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-zookeeper-client.Exception.super_.captureStackTrace"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.Exception.super_.</span>captureStackTrace ()](#apidoc.element.node-zookeeper-client.Exception.super_.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-zookeeper-client.Id"></a>[module node-zookeeper-client.Id](#apidoc.module.node-zookeeper-client.Id)

#### <a name="apidoc.element.node-zookeeper-client.Id.Id"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.</span>Id (scheme, id)](#apidoc.element.node-zookeeper-client.Id.Id)
- description and source-code
```javascript
function Id(scheme, id) {
    if (!scheme || typeof scheme !== 'string') {
        throw new Error('scheme must be a non-empty string.');
    }

    if (typeof id !== 'string') {
        throw new Error('id must be a string.');
    }

    this.scheme = scheme;
    this.id = id;
}
```
- example usage
```shell
...

'''javascript
zookeeper.setACL(
'/test/demo',
[
    new zookeeper.ACL(
        zookeeeper.Permission.ADMIN,
        new zookeeper.Id('ip', '127.0.0.1')
    )
],
function (error, acls, stat) {
    if (error) {
        console.log(error.stack);
        return;
    }
...
```

#### <a name="apidoc.element.node-zookeeper-client.Id.fromRecord"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.Id.</span>fromRecord (record)](#apidoc.element.node-zookeeper-client.Id.fromRecord)
- description and source-code
```javascript
function fromRecord(record) {
    if (!(record instanceof jute.data.Id)) {
        throw new Error('record must be an instace of jute.data.Id.');
    }

    return new Id(record.scheme, record.id);
}
```
- example usage
```shell
...
            return;
        }

        var acls;

        if (Array.isArray(response.payload.acl)) {
            acls = response.payload.acl.map(function (item) {
                return ACL.fromRecord(item);
            });
        }

        next(null, acls, response.payload.stat);
    });
},
callback
...
```



# <a name="apidoc.module.node-zookeeper-client.Id.prototype"></a>[module node-zookeeper-client.Id.prototype](#apidoc.module.node-zookeeper-client.Id.prototype)

#### <a name="apidoc.element.node-zookeeper-client.Id.prototype.toRecord"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.Id.prototype.</span>toRecord ()](#apidoc.element.node-zookeeper-client.Id.prototype.toRecord)
- description and source-code
```javascript
toRecord = function () {
    return new jute.data.Id(
        this.scheme,
        this.id
    );
}
```
- example usage
```shell
...

header = new jute.protocol.RequestHeader();
header.type = jute.OP_CODES.CREATE;

payload = new jute.protocol.CreateRequest();
payload.path = path;
payload.acl = acls.map(function (item) {
    return item.toRecord();
});
payload.flags = mode;

if (Buffer.isBuffer(data)) {
    payload.data = new Buffer(data.length);
    data.copy(payload.data);
}
...
```



# <a name="apidoc.module.node-zookeeper-client.PacketQueue"></a>[module node-zookeeper-client.PacketQueue](#apidoc.module.node-zookeeper-client.PacketQueue)

#### <a name="apidoc.element.node-zookeeper-client.PacketQueue.PacketQueue"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.</span>PacketQueue ()](#apidoc.element.node-zookeeper-client.PacketQueue.PacketQueue)
- description and source-code
```javascript
function PacketQueue() {
    events.EventEmitter.call(this);

    this.queue = [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-zookeeper-client.PacketQueue.super_"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.PacketQueue.</span>super_ ()](#apidoc.element.node-zookeeper-client.PacketQueue.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-zookeeper-client.PacketQueue.prototype"></a>[module node-zookeeper-client.PacketQueue.prototype](#apidoc.module.node-zookeeper-client.PacketQueue.prototype)

#### <a name="apidoc.element.node-zookeeper-client.PacketQueue.prototype.push"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.PacketQueue.prototype.</span>push (packet)](#apidoc.element.node-zookeeper-client.PacketQueue.prototype.push)
- description and source-code
```javascript
push = function (packet) {
    if (typeof packet !== 'object') {
        throw new Error('packet must be a valid object.');
    }

    this.queue.push(packet);

    this.emit('readable');
}
```
- example usage
```shell
...
            });
        },
        function (error) {
            var args = [],
                result = results[count - 1];

            if (callback) {
                args.push(result.error);
                Array.prototype.push.apply(args, result.args);

                callback.apply(null, args);
            }
        }
    );
}
...
```

#### <a name="apidoc.element.node-zookeeper-client.PacketQueue.prototype.shift"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.PacketQueue.prototype.</span>shift ()](#apidoc.element.node-zookeeper-client.PacketQueue.prototype.shift)
- description and source-code
```javascript
shift = function () {
    return this.queue.shift();
}
```
- example usage
```shell
...
};

ConnectionManager.prototype.registerExistenceWatcher = function (path, watcher) {
    this.watcherManager.registerExistenceWatcher(path, watcher);
};

ConnectionManager.prototype.cleanupPendingQueue = function (errorCode) {
    var pendingPacket = this.pendingQueue.shift();

    while (pendingPacket) {
if (pendingPacket.callback) {
    pendingPacket.callback(Exception.create(errorCode));
}

pendingPacket = this.pendingQueue.shift();
...
```

#### <a name="apidoc.element.node-zookeeper-client.PacketQueue.prototype.unshift"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.PacketQueue.prototype.</span>unshift (packet)](#apidoc.element.node-zookeeper-client.PacketQueue.prototype.unshift)
- description and source-code
```javascript
unshift = function (packet) {
    if (typeof packet !== 'object') {
        throw new Error('packet must be a valid object.');
    }

    this.queue.unshift(packet);
    this.emit('readable');
}
```
- example usage
```shell
...


PacketQueue.prototype.unshift = function (packet) {
    if (typeof packet !== 'object') {
        throw new Error('packet must be a valid object.');
    }

    this.queue.unshift(packet);
    this.emit('readable');
};

PacketQueue.prototype.shift = function () {
    return this.queue.shift();
};
...
```



# <a name="apidoc.module.node-zookeeper-client.Path"></a>[module node-zookeeper-client.Path](#apidoc.module.node-zookeeper-client.Path)

#### <a name="apidoc.element.node-zookeeper-client.Path.validate"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.Path.</span>validate (path)](#apidoc.element.node-zookeeper-client.Path.validate)
- description and source-code
```javascript
function validate(path) {
    assert(
        path && typeof path === 'string',
        'Node path must be a non-empty string.'
    );

    assert(path[0] === '/', 'Node path must start with / character.');

    // Shortcut, no need to check more since the path is the root.
    if (path.length === 1) {
        return;
    }

    assert(
        path[path.length - 1] !== '/',
        'Node path must not end with / character.'
    );

    assert(
        !/\/\//.test(path),
        'Node path must not contain empty node name.'
    );

    assert(
        !/\/\.(\.)?(\/|$)/.test(path),
        'Node path must not contain relative path(s).'
    );

    // TODO filter out special characters
}
```
- example usage
```shell
...
Client.prototype.create = function (path, data, acls, mode, callback) {
var self = this,
    optionalArgs = [data, acls, mode, callback],
    header,
    payload,
    request;

Path.validate(path);

// Reset arguments so we can reassign correct value to them.
data = acls = mode = callback = undefined;
optionalArgs.forEach(function (arg, index) {
    if (Array.isArray(arg)) {
        acls = arg;
    } else if (typeof arg === 'number') {
...
```



# <a name="apidoc.module.node-zookeeper-client.Transaction"></a>[module node-zookeeper-client.Transaction](#apidoc.module.node-zookeeper-client.Transaction)

#### <a name="apidoc.element.node-zookeeper-client.Transaction.Transaction"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.</span>Transaction (connectionManager)](#apidoc.element.node-zookeeper-client.Transaction.Transaction)
- description and source-code
```javascript
function Transaction(connectionManager) {
    if (!(this instanceof Transaction)) {
        return new Transaction(connectionManager);
    }

    assert(
        connectionManager instanceof ConnectionManager,
        'connectionManager must be an instance of ConnectionManager.'
    );

    this.ops = [];
    this.connectionManager = connectionManager;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-zookeeper-client.Transaction.prototype"></a>[module node-zookeeper-client.Transaction.prototype](#apidoc.module.node-zookeeper-client.Transaction.prototype)

#### <a name="apidoc.element.node-zookeeper-client.Transaction.prototype.check"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.Transaction.prototype.</span>check (path, version)](#apidoc.element.node-zookeeper-client.Transaction.prototype.check)
- description and source-code
```javascript
check = function (path, version) {
    version = version || -1;

    Path.validate(path);
    assert(typeof version === 'number', 'version must be a number.');

    this.ops.push({
        type : jute.OP_CODES.CHECK,
        path : path,
        version : version
    });

    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-zookeeper-client.Transaction.prototype.commit"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.Transaction.prototype.</span>commit (callback)](#apidoc.element.node-zookeeper-client.Transaction.prototype.commit)
- description and source-code
```javascript
commit = function (callback) {
    assert(typeof callback === 'function', 'callback must be a function');

    var self = this,
        header = new jute.protocol.RequestHeader(),
        payload = new jute.TransactionRequest(this.ops),
        request;

    header.type = jute.OP_CODES.MULTI;
    request = new jute.Request(header, payload);

    this.connectionManager.queue(request, function (error, response) {
        if (error) {
            callback(error);
            return;
        }

        var result,
            i;

        for (i = 0; i < response.payload.results.length; i += 1) {
            result = response.payload.results[i];

            // Find if there is an op which caused the transaction to fail.
            if (result.type === jute.OP_CODES.ERROR &&
                    result.err !== Exception.OK) {
                error = Exception.create(result.err);
                break;
            }
        }

        callback(error, response.payload.results);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-zookeeper-client.Transaction.prototype.create"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.Transaction.prototype.</span>create (path, data, acls, mode)](#apidoc.element.node-zookeeper-client.Transaction.prototype.create)
- description and source-code
```javascript
create = function (path, data, acls, mode) {
    var optionalArgs = [data, acls, mode],
        self = this,
        currentPath = '',
        nodes;

    Path.validate(path);

    // Reset arguments so we can reassign correct value to them.
    data = acls = mode = undefined;
    optionalArgs.forEach(function (arg, index) {
        if (Array.isArray(arg)) {
            acls = arg;
        } else if (typeof arg === 'number') {
            mode = arg;
        } else if (Buffer.isBuffer(arg)) {
            data = arg;
        }
    });

    acls = Array.isArray(acls) ? acls : ACL.OPEN_ACL_UNSAFE;
    mode = typeof mode === 'number' ? mode : CreateMode.PERSISTENT;

    assert(
        data === null || data === undefined || Buffer.isBuffer(data),
        'data must be a valid buffer, null or undefined.'
    );

    assert(acls.length > 0, 'acls must be a non-empty array.');

    this.ops.push({
        type : jute.OP_CODES.CREATE,
        path : path,
        data : data,
        acls : acls,
        mode : mode
    });

    return this;
}
```
- example usage
```shell
...

var client = zookeeper.createClient('localhost:2181');
var path = process.argv[2];

client.once('connected', function () {
    console.log('Connected to the server.');

    client.create(path, function (error) {
if (error) {
    console.log('Failed to create node: %s due to: %s.', path, error);
} else {
    console.log('Node: %s is successfully created.', path);
}

client.close();
...
```

#### <a name="apidoc.element.node-zookeeper-client.Transaction.prototype.remove"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.Transaction.prototype.</span>remove (path, version)](#apidoc.element.node-zookeeper-client.Transaction.prototype.remove)
- description and source-code
```javascript
remove = function (path, version) {
    version = version || -1;

    Path.validate(path);
    assert(typeof version === 'number', 'version must be a number.');

    this.ops.push({
        type : jute.OP_CODES.DELETE,
        path : path,
        version : version
    });

    return this;
}
```
- example usage
```shell
...
* path 'String' - Path of the node.
* version 'Number' - The version of the node, optional, defaults to -1.
* callback(error) 'Function' - The callback function.

**Example**

'''javascript
zookeeper.remove('/test/demo', -1, function (error) {
    if (error) {
        console.log(error.stack);
        return;
    }

    console.log('Node is deleted.');
});
...
```

#### <a name="apidoc.element.node-zookeeper-client.Transaction.prototype.setData"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.Transaction.prototype.</span>setData (path, data, version)](#apidoc.element.node-zookeeper-client.Transaction.prototype.setData)
- description and source-code
```javascript
setData = function (path, data, version) {
    version = version || -1;

    Path.validate(path);
    assert(
        data === null || data === undefined || Buffer.isBuffer(data),
        'data must be a valid buffer, null or undefined.'
    );
    assert(typeof version === 'number', 'version must be a number.');

    this.ops.push({
        type : jute.OP_CODES.SET_DATA,
        path : path,
        data : data,
        version : version
    });

    return this;
}
```
- example usage
```shell
...
* version 'Number' - The version of the node, optional, defaults to -1.
* callback(error, stat) 'Function' - The callback function. The 'stat' is an
  instance of ['Stat'](#stat).

**Example**

'''javascript
zookeeper.setData('/test/demo', null, 2, function (error, stat) {
    if (error) {
        console.log(error.stack);
        return;
    }

    console.log('Data is set.');
});
...
```



# <a name="apidoc.module.node-zookeeper-client.WatcherManager"></a>[module node-zookeeper-client.WatcherManager](#apidoc.module.node-zookeeper-client.WatcherManager)

#### <a name="apidoc.element.node-zookeeper-client.WatcherManager.WatcherManager"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.</span>WatcherManager ()](#apidoc.element.node-zookeeper-client.WatcherManager.WatcherManager)
- description and source-code
```javascript
function WatcherManager() {
    this.dataWatchers = {};
    this.childWatchers = {};
    this.existenceWatchers = {};
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-zookeeper-client.WatcherManager.prototype"></a>[module node-zookeeper-client.WatcherManager.prototype](#apidoc.module.node-zookeeper-client.WatcherManager.prototype)

#### <a name="apidoc.element.node-zookeeper-client.WatcherManager.prototype.emit"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.WatcherManager.prototype.</span>emit (watcherEvent)](#apidoc.element.node-zookeeper-client.WatcherManager.prototype.emit)
- description and source-code
```javascript
emit = function (watcherEvent) {
    if (!watcherEvent) {
        throw new Error('watcherEvent must be a valid object.');
    }

    var emitters = [],
        event;

    switch (watcherEvent.type) {
    case Event.NODE_DATA_CHANGED:
    case Event.NODE_CREATED:
        if (this.dataWatchers[watcherEvent.path]) {
            emitters.push(this.dataWatchers[watcherEvent.path]);
            delete this.dataWatchers[watcherEvent.path];
        }

        if (this.existenceWatchers[watcherEvent.path]) {
            emitters.push(this.existenceWatchers[watcherEvent.path]);
            delete this.existenceWatchers[watcherEvent.path];
        }
        break;
    case Event.NODE_CHILDREN_CHANGED:
        if (this.childWatchers[watcherEvent.path]) {
            emitters.push(this.childWatchers[watcherEvent.path]);
            delete this.childWatchers[watcherEvent.path];
        }
        break;
    case Event.NODE_DELETED:
        if (this.dataWatchers[watcherEvent.path]) {
            emitters.push(this.dataWatchers[watcherEvent.path]);
            delete this.dataWatchers[watcherEvent.path];
        }
        if (this.childWatchers[watcherEvent.path]) {
            emitters.push(this.childWatchers[watcherEvent.path]);
            delete this.childWatchers[watcherEvent.path];
        }
        break;
    default:
        throw new Error('Unknown event type: ' + watcherEvent.type);
    }

    if (emitters.length < 1) {
        return;
    }

    event = Event.create(watcherEvent);

    emitters.forEach(function (emitter) {
        emitter.emit('notification', event);
    });
}
```
- example usage
```shell
...

/**
 * Default state listener to emit user-friendly events.
 */
function defaultStateListener(state) {
switch (state) {
case State.DISCONNECTED:
    this.emit('disconnected');
    break;
case State.SYNC_CONNECTED:
    this.emit('connected');
    break;
case State.CONNECTED_READ_ONLY:
    this.emit('connectedReadOnly');
    break;
...
```

#### <a name="apidoc.element.node-zookeeper-client.WatcherManager.prototype.getChildWatcherPaths"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.WatcherManager.prototype.</span>getChildWatcherPaths ()](#apidoc.element.node-zookeeper-client.WatcherManager.prototype.getChildWatcherPaths)
- description and source-code
```javascript
getChildWatcherPaths = function () {
    return getWatcherPaths(this, 'child');
}
```
- example usage
```shell
...
        header.type = jute.OP_CODES.SET_WATCHES;
        header.xid = jute.XID_SET_WATCHES;

        payload.setChrootPath(this.chrootPath);
        payload.relativeZxid = this.zxid;
        payload.dataWatches = this.watcherManager.getDataWatcherPaths();
        payload.existWatches = this.watcherManager.getExistenceWatcherPaths();
        payload.childWatches = this.watcherManager.getChildWatcherPaths();

        setWatchesRequest = new jute.Request(header, payload);
        this.queue(setWatchesRequest);
    }
};

ConnectionManager.prototype.onSocketTimeout = function () {
...
```

#### <a name="apidoc.element.node-zookeeper-client.WatcherManager.prototype.getDataWatcherPaths"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.WatcherManager.prototype.</span>getDataWatcherPaths ()](#apidoc.element.node-zookeeper-client.WatcherManager.prototype.getDataWatcherPaths)
- description and source-code
```javascript
getDataWatcherPaths = function () {
    return getWatcherPaths(this, 'data');
}
```
- example usage
```shell
...
        payload = new jute.protocol.SetWatches();

        header.type = jute.OP_CODES.SET_WATCHES;
        header.xid = jute.XID_SET_WATCHES;

        payload.setChrootPath(this.chrootPath);
        payload.relativeZxid = this.zxid;
        payload.dataWatches = this.watcherManager.getDataWatcherPaths();
        payload.existWatches = this.watcherManager.getExistenceWatcherPaths();
        payload.childWatches = this.watcherManager.getChildWatcherPaths();

        setWatchesRequest = new jute.Request(header, payload);
        this.queue(setWatchesRequest);
    }
};
...
```

#### <a name="apidoc.element.node-zookeeper-client.WatcherManager.prototype.getExistenceWatcherPaths"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.WatcherManager.prototype.</span>getExistenceWatcherPaths ()](#apidoc.element.node-zookeeper-client.WatcherManager.prototype.getExistenceWatcherPaths)
- description and source-code
```javascript
getExistenceWatcherPaths = function () {
    return getWatcherPaths(this, 'existence');
}
```
- example usage
```shell
...

        header.type = jute.OP_CODES.SET_WATCHES;
        header.xid = jute.XID_SET_WATCHES;

        payload.setChrootPath(this.chrootPath);
        payload.relativeZxid = this.zxid;
        payload.dataWatches = this.watcherManager.getDataWatcherPaths();
        payload.existWatches = this.watcherManager.getExistenceWatcherPaths();
        payload.childWatches = this.watcherManager.getChildWatcherPaths();

        setWatchesRequest = new jute.Request(header, payload);
        this.queue(setWatchesRequest);
    }
};
...
```

#### <a name="apidoc.element.node-zookeeper-client.WatcherManager.prototype.isEmpty"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.WatcherManager.prototype.</span>isEmpty ()](#apidoc.element.node-zookeeper-client.WatcherManager.prototype.isEmpty)
- description and source-code
```javascript
isEmpty = function () {
    var empty = true,
        watchers,
        paths,
        i,
        j;

    watchers = [this.dataWatchers, this.existenceWatchers, this.childWatchers];

    for (i = 0; i < watchers.length; i += 1) {
        paths = Object.keys(watchers[i]);

        for (j = 0; j < paths.length; j += 1) {
            if (watchers[i][paths[j]].listeners('notification').length > 0) {
                empty = false;
                break;
            }
        }
    }

    return empty;
}
```
- example usage
```shell
...
    authRequest = new jute.Request(header, payload);
    this.queue(authRequest);

},  this);
    }

    // Reset the watchers if we have any.
    if (!this.watcherManager.isEmpty()) {
header = new jute.protocol.RequestHeader();
payload = new jute.protocol.SetWatches();

header.type = jute.OP_CODES.SET_WATCHES;
header.xid = jute.XID_SET_WATCHES;

payload.setChrootPath(this.chrootPath);
...
```

#### <a name="apidoc.element.node-zookeeper-client.WatcherManager.prototype.registerChildWatcher"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.WatcherManager.prototype.</span>registerChildWatcher (path, watcher)](#apidoc.element.node-zookeeper-client.WatcherManager.prototype.registerChildWatcher)
- description and source-code
```javascript
registerChildWatcher = function (path, watcher) {
    registerWatcher(this, 'child', path, watcher);
}
```
- example usage
```shell
...
        self.connectionManager.queue(request, function (error, response) {
            if (error) {
                next(error);
                return;
            }

            if (watcher) {
                self.connectionManager.registerChildWatcher(path, watcher);
            }

            next(null, response.payload.children, response.payload.stat);
        });
    },
    callback
);
...
```

#### <a name="apidoc.element.node-zookeeper-client.WatcherManager.prototype.registerDataWatcher"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.WatcherManager.prototype.</span>registerDataWatcher (path, watcher)](#apidoc.element.node-zookeeper-client.WatcherManager.prototype.registerDataWatcher)
- description and source-code
```javascript
registerDataWatcher = function (path, watcher) {
    registerWatcher(this, 'data', path, watcher);
}
```
- example usage
```shell
...
        self.connectionManager.queue(request, function (error, response) {
            if (error) {
                next(error);
                return;
            }

            if (watcher) {
                self.connectionManager.registerDataWatcher(path, watcher);
            }

            next(null, response.payload.data, response.payload.stat);
        });
    },
    callback
);
...
```

#### <a name="apidoc.element.node-zookeeper-client.WatcherManager.prototype.registerExistenceWatcher"></a>[function <span class="apidocSignatureSpan">node-zookeeper-client.WatcherManager.prototype.</span>registerExistenceWatcher (path, watcher)](#apidoc.element.node-zookeeper-client.WatcherManager.prototype.registerExistenceWatcher)
- description and source-code
```javascript
registerExistenceWatcher = function (path, watcher) {
    registerWatcher(this, 'existence', path, watcher);
}
```
- example usage
```shell
...
if (watcher) {
    if (existence) {
        self.connectionManager.registerDataWatcher(
            path,
            watcher
        );
    } else {
        self.connectionManager.registerExistenceWatcher(
            path,
            watcher
        );
    }
}

next(
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
