# api documentation for  [socketcluster (v5.9.1)](http://socketcluster.io)  [![npm package](https://img.shields.io/npm/v/npmdoc-socketcluster.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-socketcluster) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-socketcluster.svg)](https://travis-ci.org/npmdoc/node-npmdoc-socketcluster)
#### SocketCluster - A Highly parallelized WebSocket server cluster to make the most of multi-core machines/instances.

[![NPM](https://nodei.co/npm/socketcluster.png?downloads=true)](https://www.npmjs.com/package/socketcluster)

[![apidoc](https://npmdoc.github.io/node-npmdoc-socketcluster/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-socketcluster_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-socketcluster/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-socketcluster/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-socketcluster/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "bin": {
        "socketcluster": "bin/cli.js"
    },
    "bugs": {
        "url": "https://github.com/SocketCluster/socketcluster/issues"
    },
    "contributors": [
        {
            "name": "Jonathan Gros-Dubois",
            "email": "grosjona@yahoo.com.au"
        }
    ],
    "dependencies": {
        "async": "2.0.0",
        "base64id": "0.1.0",
        "fs-extra": "2.0.0",
        "inquirer": "1.1.3",
        "minimist": "1.1.0",
        "sc-auth": "~3.2.1",
        "sc-broker-cluster": "~4.0.0",
        "sc-domain": "~1.0.1",
        "sc-emitter": "~1.1.0",
        "sc-errors": "~1.1.0",
        "socketcluster-server": "~5.10.2",
        "uid-number": "0.0.5",
        "uuid": "3.0.1"
    },
    "description": "SocketCluster - A Highly parallelized WebSocket server cluster to make the most of multi-core machines/instances.",
    "devDependencies": {
        "socketcluster-client": "~5.3.0"
    },
    "directories": {},
    "dist": {
        "shasum": "110ab264e3325c6cf5ecfc1a04c4343a9d806844",
        "tarball": "https://registry.npmjs.org/socketcluster/-/socketcluster-5.9.1.tgz"
    },
    "gitHead": "30fe1390746f43c63f0ff9e12e1d3c46064ae371",
    "homepage": "http://socketcluster.io",
    "keywords": [
        "websocket",
        "server",
        "realtime",
        "cluster",
        "scalable"
    ],
    "license": "MIT",
    "maintainers": [
        {
            "name": "topcloudsystems",
            "email": "grosjona@yahoo.com.au"
        }
    ],
    "name": "socketcluster",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/SocketCluster/socketcluster.git"
    },
    "scripts": {},
    "version": "5.9.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module socketcluster](#apidoc.module.socketcluster)
1.  [function <span class="apidocSignatureSpan">socketcluster.</span>SocketCluster (options)](#apidoc.element.socketcluster.SocketCluster)
1.  [function <span class="apidocSignatureSpan">socketcluster.</span>scworker (options)](#apidoc.element.socketcluster.scworker)
1.  object <span class="apidocSignatureSpan">socketcluster.</span>SocketCluster.prototype
1.  object <span class="apidocSignatureSpan">socketcluster.</span>scworker.prototype

#### [module socketcluster.SocketCluster](#apidoc.module.socketcluster.SocketCluster)
1.  [function <span class="apidocSignatureSpan">socketcluster.</span>SocketCluster (options)](#apidoc.element.socketcluster.SocketCluster.SocketCluster)

#### [module socketcluster.SocketCluster.prototype](#apidoc.module.socketcluster.SocketCluster.prototype)
1.  [function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>_brokerEngineErrorHandler (pid, error)](#apidoc.element.socketcluster.SocketCluster.prototype._brokerEngineErrorHandler)
1.  [function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>_brokerErrorHandler (brokerPid, error)](#apidoc.element.socketcluster.SocketCluster.prototype._brokerErrorHandler)
1.  [function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>_capitaliseFirstLetter (str)](#apidoc.element.socketcluster.SocketCluster.prototype._capitaliseFirstLetter)
1.  [function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>_cloneObject (object)](#apidoc.element.socketcluster.SocketCluster.prototype._cloneObject)
1.  [function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>_getBrokerSocketName (brokerId)](#apidoc.element.socketcluster.SocketCluster.prototype._getBrokerSocketName)
1.  [function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>_getBrokerSocketPaths ()](#apidoc.element.socketcluster.SocketCluster.prototype._getBrokerSocketPaths)
1.  [function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>_handleWorkerClusterExit (errorCode)](#apidoc.element.socketcluster.SocketCluster.prototype._handleWorkerClusterExit)
1.  [function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>_init (options)](#apidoc.element.socketcluster.SocketCluster.prototype._init)
1.  [function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>_launchWorkerCluster ()](#apidoc.element.socketcluster.SocketCluster.prototype._launchWorkerCluster)
1.  [function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>_logDeploymentDetails ()](#apidoc.element.socketcluster.SocketCluster.prototype._logDeploymentDetails)
1.  [function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>_logObject (obj, objType, time)](#apidoc.element.socketcluster.SocketCluster.prototype._logObject)
1.  [function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>_start ()](#apidoc.element.socketcluster.SocketCluster.prototype._start)
1.  [function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>_workerClusterErrorHandler (pid, error)](#apidoc.element.socketcluster.SocketCluster.prototype._workerClusterErrorHandler)
1.  [function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>_workerClusterReadyHandler ()](#apidoc.element.socketcluster.SocketCluster.prototype._workerClusterReadyHandler)
1.  [function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>_workerErrorHandler (workerPid, error)](#apidoc.element.socketcluster.SocketCluster.prototype._workerErrorHandler)
1.  [function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>_workerExitHandler (workerInfo)](#apidoc.element.socketcluster.SocketCluster.prototype._workerExitHandler)
1.  [function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>_workerStartHandler (workerInfo)](#apidoc.element.socketcluster.SocketCluster.prototype._workerStartHandler)
1.  [function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>_workerWarningHandler (workerPid, warning)](#apidoc.element.socketcluster.SocketCluster.prototype._workerWarningHandler)
1.  [function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>colorText (message, color)](#apidoc.element.socketcluster.SocketCluster.prototype.colorText)
1.  [function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>errorHandler (err, origin)](#apidoc.element.socketcluster.SocketCluster.prototype.errorHandler)
1.  [function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>killBrokers ()](#apidoc.element.socketcluster.SocketCluster.prototype.killBrokers)
1.  [function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>killWorkers (options)](#apidoc.element.socketcluster.SocketCluster.prototype.killWorkers)
1.  [function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>log (message, time)](#apidoc.element.socketcluster.SocketCluster.prototype.log)
1.  [function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>sendToBroker (brokerId, data)](#apidoc.element.socketcluster.SocketCluster.prototype.sendToBroker)
1.  [function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>sendToWorker (workerId, data)](#apidoc.element.socketcluster.SocketCluster.prototype.sendToWorker)
1.  [function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>triggerInfo (info, origin)](#apidoc.element.socketcluster.SocketCluster.prototype.triggerInfo)
1.  [function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>warningHandler (warning, origin)](#apidoc.element.socketcluster.SocketCluster.prototype.warningHandler)

#### [module socketcluster.scworker](#apidoc.module.socketcluster.scworker)
1.  [function <span class="apidocSignatureSpan">socketcluster.</span>scworker (options)](#apidoc.element.socketcluster.scworker.scworker)

#### [module socketcluster.scworker.prototype](#apidoc.module.socketcluster.scworker.prototype)
1.  [function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>_calculateStatus ()](#apidoc.element.socketcluster.scworker.prototype._calculateStatus)
1.  [function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>_httpRequestHandler (req, res)](#apidoc.element.socketcluster.scworker.prototype._httpRequestHandler)
1.  [function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>_init (options)](#apidoc.element.socketcluster.scworker.prototype._init)
1.  [function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>_start ()](#apidoc.element.socketcluster.scworker.prototype._start)
1.  [function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>_startServer ()](#apidoc.element.socketcluster.scworker.prototype._startServer)
1.  [function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>addMiddleware (type, middleware)](#apidoc.element.socketcluster.scworker.prototype.addMiddleware)
1.  [function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>close (callback)](#apidoc.element.socketcluster.scworker.prototype.close)
1.  [function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>errorHandler (err)](#apidoc.element.socketcluster.scworker.prototype.errorHandler)
1.  [function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>getHTTPServer ()](#apidoc.element.socketcluster.scworker.prototype.getHTTPServer)
1.  [function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>getSCServer ()](#apidoc.element.socketcluster.scworker.prototype.getSCServer)
1.  [function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>getSocketPath ()](#apidoc.element.socketcluster.scworker.prototype.getSocketPath)
1.  [function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>getSocketURL ()](#apidoc.element.socketcluster.scworker.prototype.getSocketURL)
1.  [function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>getStatus ()](#apidoc.element.socketcluster.scworker.prototype.getStatus)
1.  [function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>handleMasterEvent ()](#apidoc.element.socketcluster.scworker.prototype.handleMasterEvent)
1.  [function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>handleMasterMessage (message)](#apidoc.element.socketcluster.scworker.prototype.handleMasterMessage)
1.  [function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>open ()](#apidoc.element.socketcluster.scworker.prototype.open)
1.  [function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>removeMiddleware (type, middleware)](#apidoc.element.socketcluster.scworker.prototype.removeMiddleware)
1.  [function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>sendToMaster (data)](#apidoc.element.socketcluster.scworker.prototype.sendToMaster)
1.  [function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>setAuthEngine (authEngine)](#apidoc.element.socketcluster.scworker.prototype.setAuthEngine)
1.  [function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>setCodecEngine (codecEngine)](#apidoc.element.socketcluster.scworker.prototype.setCodecEngine)
1.  [function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>warningHandler (warning)](#apidoc.element.socketcluster.scworker.prototype.warningHandler)



# <a name="apidoc.module.socketcluster"></a>[module socketcluster](#apidoc.module.socketcluster)

#### <a name="apidoc.element.socketcluster.SocketCluster"></a>[function <span class="apidocSignatureSpan">socketcluster.</span>SocketCluster (options)](#apidoc.element.socketcluster.SocketCluster)
- description and source-code
```javascript
SocketCluster = function (options) {
  var self = this;
  if (socketClusterSingleton) {
    var doubleInstantiationError = new Error('The SocketCluster master object is a singleton - It can only be instantiated once
per process.');
    doubleInstantiationError.name = 'DoubleInstantiationError';
    throw doubleInstantiationError;
  }
  socketClusterSingleton = self;

  self.EVENT_FAIL = 'fail';
  self.EVENT_WARNING = 'warning';
  self.EVENT_INFO = 'info';
  self.EVENT_READY = 'ready';
  self.EVENT_WORKER_START = 'workerStart';
  self.EVENT_WORKER_EXIT = 'workerExit';

  self._errorAnnotations = {
    'EADDRINUSE': 'Failed to bind to a port because it was already used by another process.'
  };

  self._errorDomain = domain.create();
  self._errorDomain.on('error', function (err) {
    self.errorHandler(err, {
      type: 'master'
    });
  });
  self._errorDomain.add(self);

  self._errorDomain.run(function () {
    self._init(options);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socketcluster.scworker"></a>[function <span class="apidocSignatureSpan">socketcluster.</span>scworker (options)](#apidoc.element.socketcluster.scworker)
- description and source-code
```javascript
scworker = function (options) {
  var self = this;

  this.EVENT_ERROR = 'error';
  this.EVENT_WARNING = 'warning';
  this.EVENT_EXIT = 'exit';
  this.EVENT_READY = 'ready';
  this.EVENT_CONNECTION = 'connection';

  this.MIDDLEWARE_START = 'start';

  this.type = 'worker';

  this._errorDomain = domain.create();
  this._errorDomain.on('error', function () {
    self.errorHandler.apply(self, arguments);
  });

  this.start = this._errorDomain.bind(this._start);
  this._errorDomain.run(function () {
    self._init(options);
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.socketcluster.SocketCluster"></a>[module socketcluster.SocketCluster](#apidoc.module.socketcluster.SocketCluster)

#### <a name="apidoc.element.socketcluster.SocketCluster.SocketCluster"></a>[function <span class="apidocSignatureSpan">socketcluster.</span>SocketCluster (options)](#apidoc.element.socketcluster.SocketCluster.SocketCluster)
- description and source-code
```javascript
SocketCluster = function (options) {
  var self = this;
  if (socketClusterSingleton) {
    var doubleInstantiationError = new Error('The SocketCluster master object is a singleton - It can only be instantiated once
per process.');
    doubleInstantiationError.name = 'DoubleInstantiationError';
    throw doubleInstantiationError;
  }
  socketClusterSingleton = self;

  self.EVENT_FAIL = 'fail';
  self.EVENT_WARNING = 'warning';
  self.EVENT_INFO = 'info';
  self.EVENT_READY = 'ready';
  self.EVENT_WORKER_START = 'workerStart';
  self.EVENT_WORKER_EXIT = 'workerExit';

  self._errorAnnotations = {
    'EADDRINUSE': 'Failed to bind to a port because it was already used by another process.'
  };

  self._errorDomain = domain.create();
  self._errorDomain.on('error', function (err) {
    self.errorHandler(err, {
      type: 'master'
    });
  });
  self._errorDomain.add(self);

  self._errorDomain.run(function () {
    self._init(options);
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.socketcluster.SocketCluster.prototype"></a>[module socketcluster.SocketCluster.prototype](#apidoc.module.socketcluster.SocketCluster.prototype)

#### <a name="apidoc.element.socketcluster.SocketCluster.prototype._brokerEngineErrorHandler"></a>[function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>_brokerEngineErrorHandler (pid, error)](#apidoc.element.socketcluster.SocketCluster.prototype._brokerEngineErrorHandler)
- description and source-code
```javascript
_brokerEngineErrorHandler = function (pid, error) {
  if (typeof error == 'string') {
    error = new BrokerError(error);
  }
  this.errorHandler(error, {
    type: 'BrokerEngine',
    pid: pid
  });
}
```
- example usage
```shell
...
  appInitControllerPath: self._paths.appInitControllerPath
});

self._brokerEngineServer.on('error', function (err) {
  if (err.brokerPid) {
    self._brokerErrorHandler(err.brokerPid, err);
  } else {
    self._brokerEngineErrorHandler(err.pid, err);
  }
});

self._brokerEngineServer.on('ready', brokerEngineServerReady);

self._brokerEngineServer.on('brokerMessage', function (brokerId, data) {
  self.emit('brokerMessage', brokerId, data);
...
```

#### <a name="apidoc.element.socketcluster.SocketCluster.prototype._brokerErrorHandler"></a>[function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>_brokerErrorHandler (brokerPid, error)](#apidoc.element.socketcluster.SocketCluster.prototype._brokerErrorHandler)
- description and source-code
```javascript
_brokerErrorHandler = function (brokerPid, error) {
  if (typeof error == 'string') {
    error = new BrokerError(error);
  }
  this.errorHandler(error, {
    type: 'Broker',
    pid: brokerPid
  });
}
```
- example usage
```shell
...
  brokerOptions: self.options,
  appBrokerControllerPath: self._paths.appBrokerControllerPath,
  appInitControllerPath: self._paths.appInitControllerPath
});

self._brokerEngineServer.on('error', function (err) {
  if (err.brokerPid) {
    self._brokerErrorHandler(err.brokerPid, err);
  } else {
    self._brokerEngineErrorHandler(err.pid, err);
  }
});

self._brokerEngineServer.on('ready', brokerEngineServerReady);
...
```

#### <a name="apidoc.element.socketcluster.SocketCluster.prototype._capitaliseFirstLetter"></a>[function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>_capitaliseFirstLetter (str)](#apidoc.element.socketcluster.SocketCluster.prototype._capitaliseFirstLetter)
- description and source-code
```javascript
_capitaliseFirstLetter = function (str) {
  if (str == null) {
    str = '';
  }
  return str.charAt(0).toUpperCase() + str.slice(1);
}
```
- example usage
```shell
...
  if (!obj.origin.type) {
    obj.origin.type = 'Undefined';
  }
  var output = obj.stack || obj.message || obj;

  var logMessage;
  if (obj.origin.pid == null) {
    logMessage = 'Origin: ' + this._capitaliseFirstLetter(obj.origin.type) + '\n' +
      '   [' + objType + '] ' + output;
  } else {
    logMessage = 'Origin: ' + this._capitaliseFirstLetter(obj.origin.type) + ' (PID ' + obj.origin.pid + ')\n' +
      '   [' + objType + '] ' + output;
  }
  this.log(logMessage, time);
};
...
```

#### <a name="apidoc.element.socketcluster.SocketCluster.prototype._cloneObject"></a>[function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>_cloneObject (object)](#apidoc.element.socketcluster.SocketCluster.prototype._cloneObject)
- description and source-code
```javascript
_cloneObject = function (object) {
  var clone = {};
  for (var i in object) {
    if (object.hasOwnProperty(i)) {
      clone[i] = object[i];
    }
  }
  return clone;
}
```
- example usage
```shell
...
  }
  execOptions.execArgv.push('--debug-port=' + inspectPort);
  execOptions.execArgv.push('--inspect=' + inspectPort);
}

this._workerCluster = fork(__dirname + '/lib/workercluster.js', process.argv.slice(2), execOptions);

var workerOpts = this._cloneObject(this.options);
workerOpts.paths = this._paths;
workerOpts.sourcePort = this.options.port;
workerOpts.workerCount = this.options.workers;
workerOpts.brokers = this._getBrokerSocketPaths();
workerOpts.secretKey = this.options.secretKey;
workerOpts.authKey = this.options.authKey;
workerOpts.authPrivateKey = this.options.authPrivateKey;
...
```

#### <a name="apidoc.element.socketcluster.SocketCluster.prototype._getBrokerSocketName"></a>[function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>_getBrokerSocketName (brokerId)](#apidoc.element.socketcluster.SocketCluster.prototype._getBrokerSocketName)
- description and source-code
```javascript
_getBrokerSocketName = function (brokerId) {
  return 'b' + brokerId;
}
```
- example usage
```shell
...
SocketCluster.prototype._getBrokerSocketName = function (brokerId) {
return 'b' + brokerId;
};

SocketCluster.prototype._getBrokerSocketPaths = function () {
var socketPaths = [];
for (var i = 0; i < this.options.brokers; i++) {
  socketPaths.push(this._socketDirPath + this._getBrokerSocketName(i));
}
return socketPaths;
};

SocketCluster.prototype._capitaliseFirstLetter = function (str) {
if (str == null) {
  str = '';
...
```

#### <a name="apidoc.element.socketcluster.SocketCluster.prototype._getBrokerSocketPaths"></a>[function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>_getBrokerSocketPaths ()](#apidoc.element.socketcluster.SocketCluster.prototype._getBrokerSocketPaths)
- description and source-code
```javascript
_getBrokerSocketPaths = function () {
  var socketPaths = [];
  for (var i = 0; i < this.options.brokers; i++) {
    socketPaths.push(this._socketDirPath + this._getBrokerSocketName(i));
  }
  return socketPaths;
}
```
- example usage
```shell
...

this._workerCluster = fork(__dirname + '/lib/workercluster.js', process.argv.slice(2), execOptions);

var workerOpts = this._cloneObject(this.options);
workerOpts.paths = this._paths;
workerOpts.sourcePort = this.options.port;
workerOpts.workerCount = this.options.workers;
workerOpts.brokers = this._getBrokerSocketPaths();
workerOpts.secretKey = this.options.secretKey;
workerOpts.authKey = this.options.authKey;
workerOpts.authPrivateKey = this.options.authPrivateKey;
workerOpts.authPublicKey = this.options.authPublicKey;
workerOpts.authDefaultExpiry = this.options.authDefaultExpiry;
workerOpts.authAlgorithm = this.options.authAlgorithm;
workerOpts.authSignAsync = this.options.authSignAsync;
...
```

#### <a name="apidoc.element.socketcluster.SocketCluster.prototype._handleWorkerClusterExit"></a>[function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>_handleWorkerClusterExit (errorCode)](#apidoc.element.socketcluster.SocketCluster.prototype._handleWorkerClusterExit)
- description and source-code
```javascript
_handleWorkerClusterExit = function (errorCode) {
  var message = 'workerCluster exited with code: ' + errorCode;
  if (errorCode == 0) {
    this.log(message);
  } else {
    var error = new ProcessExitError(message, errorCode);
    this.errorHandler(error, {
      type: 'workerCluster'
    });
  }
  this._launchWorkerCluster();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socketcluster.SocketCluster.prototype._init"></a>[function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>_init (options)](#apidoc.element.socketcluster.SocketCluster.prototype._init)
- description and source-code
```javascript
_init = function (options) {
  var self = this;

  var backslashRegex = /\\/g;
  var appDirPath = path.dirname(require.main.filename).replace(backslashRegex, '/');

  self.options = {
    port: 8000,
    workers: null,
    brokers: null,
    appName: null,
    instanceId: null,
    secretKey: null,
    authKey: null,
    authPrivateKey: null,
    authPublicKey: null,
    authDefaultExpiry: 86400,
    authAlgorithm: null,
    authSignAsync: false,
    authVerifyAsync: true,
    crashWorkerOnError: true,
    rebootWorkerOnCrash: true,
    killWorkerMemoryThreshold: null,
    protocol: 'http',
    protocolOptions: null,
    logLevel: 2,
    handshakeTimeout: 10000,
    ackTimeout: 10000,
    pingInterval: 8000,
    pingTimeout: 20000,
    origins: '*:*',
    socketChannelLimit: 1000,
    workerStatusInterval: 10000,
    processTermTimeout: 10000,
    propagateErrors: true,
    propagateWarnings: true,
    middlewareEmitWarnings: true,
    host: null,
    tcpSynBacklog: null,
    workerController: null,
    brokerController: null,
    initController: null,
    rebootOnSignal: true,
    downgradeToUser: false,
    path: '/socketcluster/',
    socketRoot: null,
    schedulingPolicy: null,
    allowClientPublish: true,
    defaultWorkerDebugPort: 5858,
    defaultBrokerDebugPort: 6858,
    httpServerModule: null,
    pubSubBatchDuration: null,
    environment: 'dev',
    killMasterOnSignal: false,
    wsEngine: 'uws',
    brokerEngine: 'sc-broker-cluster'
  };

  self._active = false;
  self._workerCluster = null;

  self._colorCodes = {
    red: 31,
    green: 32,
    yellow: 33
  };

  for (var i in options) {
    if (options.hasOwnProperty(i)) {
      self.options[i] = options[i];
    }
  }

  // Make sure there is always a trailing slash in WS path
  self.options.path = self.options.path.replace(/\/?$/, '/');

  var maxTimeout = Math.pow(2, 31) - 1;

  var verifyDuration = function (propertyName) {
    if (self.options[propertyName] > maxTimeout) {
      throw new InvalidOptionsError('The ' + propertyName +
        ' value provided exceeded the maximum amount allowed');
    }
  };

  verifyDuration('ackTimeout');
  verifyDuration('pingInterval');
  verifyDuration('pingTimeout');
  verifyDuration('workerStatusInterval');
  verifyDuration('processTermTimeout');

  if (self.options.appName == null) {
    self.options.appName = uuid.v4();
  }

  if (self.options.workerController == null) {
    throw new InvalidOptionsError("Compulsory option 'workerController' was not specified " +
      "- It needs to be a path to a JavaScript file which will act as the " +
      "boot controller for each worker in the cluster");
  }

  self._paths = {
    appDirPath: appDirPath,
    statusURL: '/~status',
    appWorkerControllerPath: path.resolve(self.options.workerController)
  };

  if (self.options.initController) {
      self._paths.appInitControllerPath = path.resolve(self.options.initController);
  } else {
      self._paths.appInitControllerPath = null;
  }

  if (/\.js$/.test(self.options.wsEngine)) {
    self._paths.wsEnginePath = path.resolve(self.options.wsEngine);
  } else {
    self._paths.wsEnginePath = self.options.wsEngine;
  }

  var pathHasher = crypto.createHash('md5');
  pathHasher.update(self._paths.appDirPath, 'utf8');
  var pathHash = pathHasher.digest('hex').substr(0, 10);
  // Trimp it because some OSes (e.g. OSX) do not like long path names for domain sockets.
  var shortAppName = self.options.appName.substr(0, 13);

  if (process.platform == 'win32') {
    if (self.options.socketRoot) {
      self._socketDirPath = self.options.socketRoot + '_';
    } else {
      self._socketDirPath = '\\\\.\\pipe\\socketcluster_' + shortAppName + '_' + pathHash + '_';
    }
  } else {
    var socketDir, socketParentDir;
    if (self.options.socketRoot) {
      socketDir = self.options.socketRoot.replace(/\/$/, '') + '/';
    } else {
      socketParentDir = os.tmpdir() + '/socketcluster/';
      socketDir = socketParentDir + shortAppName + '_' + pathHash + '/';
    }
    if (fs.existsSync(socketDir)) {
      try {
        fs.removeSync(soc ...
```
- example usage
```shell
...
  self.errorHandler(err, {
    type: 'master'
  });
});
self._errorDomain.add(self);

self._errorDomain.run(function () {
  self._init(options);
});
};

SocketCluster.prototype = Object.create(EventEmitter.prototype);

SocketCluster.prototype._init = function (options) {
var self = this;
...
```

#### <a name="apidoc.element.socketcluster.SocketCluster.prototype._launchWorkerCluster"></a>[function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>_launchWorkerCluster ()](#apidoc.element.socketcluster.SocketCluster.prototype._launchWorkerCluster)
- description and source-code
```javascript
_launchWorkerCluster = function () {
  var self = this;

  var debugPort, inspectPort;

  // Workers should not inherit the master --debug argument
  // because they have their own --debug-workers option.
  var execOptions = {
    execArgv: process.execArgv.filter(function (arg) {
      return arg != '--debug' && arg != '--debug-brk' && arg != '--inspect';
    })
  };

  if (argv['debug-workers']) {
    if (argv['debug-workers'] == true) {
      debugPort = this.options.defaultWorkerDebugPort;
    } else {
      debugPort = argv['debug-workers'];
    }
    execOptions.execArgv.push('--debug=' + debugPort);
  }

  if (argv['inspect-workers']) {
    if (argv['inspect-workers'] == true) {
      inspectPort = this.options.defaultWorkerDebugPort;
    } else {
      inspectPort = argv['inspect-workers'];
    }
    execOptions.execArgv.push('--debug-port=' + inspectPort);
    execOptions.execArgv.push('--inspect=' + inspectPort);
  }

  this._workerCluster = fork(__dirname + '/lib/workercluster.js', process.argv.slice(2), execOptions);

  var workerOpts = this._cloneObject(this.options);
  workerOpts.paths = this._paths;
  workerOpts.sourcePort = this.options.port;
  workerOpts.workerCount = this.options.workers;
  workerOpts.brokers = this._getBrokerSocketPaths();
  workerOpts.secretKey = this.options.secretKey;
  workerOpts.authKey = this.options.authKey;
  workerOpts.authPrivateKey = this.options.authPrivateKey;
  workerOpts.authPublicKey = this.options.authPublicKey;
  workerOpts.authDefaultExpiry = this.options.authDefaultExpiry;
  workerOpts.authAlgorithm = this.options.authAlgorithm;
  workerOpts.authSignAsync = this.options.authSignAsync;
  workerOpts.authVerifyAsync = this.options.authVerifyAsync;

  if (typeof workerOpts.schedulingPolicy == 'string') {
    if (workerOpts.schedulingPolicy == 'rr') {
      workerOpts.schedulingPolicy = cluster.SCHED_RR;
    } else if (workerOpts.schedulingPolicy == 'none') {
      workerOpts.schedulingPolicy = cluster.SCHED_NONE;
    }
  }

  this._workerCluster.send({
    type: 'init',
    data: workerOpts
  });

  this._workerCluster.on('message', function workerHandler(m) {
    if (m.type == 'error') {
      var error = scErrors.hydrateError(m.data.error);
      if (m.data.workerPid) {
        self._workerErrorHandler(m.data.workerPid, error);
      } else {
        self._workerClusterErrorHandler(m.data.pid, error);
      }
    } else if (m.type == 'warning') {
      var warning = scErrors.hydrateError(m.data.error);
      self._workerWarningHandler(m.data.workerPid, warning);
    } else if (m.type == 'ready') {
      self._workerClusterReadyHandler();
    } else if (m.type == 'workerStart') {
      self._workerStartHandler(m.data);
    } else if (m.type == 'workerExit') {
      self._workerExitHandler(m.data);
    } else if (m.type == 'workerMessage') {
      self.emit('workerMessage', m.workerId, m.data);
    }
  });

  this._workerCluster.on('exit', this._handleWorkerClusterExit.bind(this));
}
```
- example usage
```shell
...
  this.log(message);
} else {
  var error = new ProcessExitError(message, errorCode);
  this.errorHandler(error, {
    type: 'workerCluster'
  });
}
this._launchWorkerCluster();
};

SocketCluster.prototype._launchWorkerCluster = function () {
var self = this;

var debugPort, inspectPort;
...
```

#### <a name="apidoc.element.socketcluster.SocketCluster.prototype._logDeploymentDetails"></a>[function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>_logDeploymentDetails ()](#apidoc.element.socketcluster.SocketCluster.prototype._logDeploymentDetails)
- description and source-code
```javascript
_logDeploymentDetails = function () {
  if (this.options.logLevel > 0) {
    console.log('   ' + this.colorText('[Active]', 'green') + ' SocketCluster started');
    console.log('            Version: ' + pkg.version);
    console.log('            Environment: ' + this.options.environment);
    console.log('            WebSocket engine: ' + this.options.wsEngine);
    console.log('            Port: ' + this.options.port);
    console.log('            Master PID: ' + process.pid);
    console.log('            Worker count: ' + this.options.workers);
    console.log('            Broker count: ' + this.options.brokers);
    console.log();
  }
  this.emit(this.EVENT_READY);
}
```
- example usage
```shell
...
      if (self.options.killMasterOnSignal) {
        process.exit();
      }
    });
  }

  this._active = true;
  this._logDeploymentDetails();
}
};

SocketCluster.prototype._workerExitHandler = function (workerInfo) {
if (this.options.logLevel > 0) {
  var message = 'Worker ' + workerInfo.id + ' exited - Exit code: ' + workerInfo.code;
  if (workerInfo.signal) {
...
```

#### <a name="apidoc.element.socketcluster.SocketCluster.prototype._logObject"></a>[function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>_logObject (obj, objType, time)](#apidoc.element.socketcluster.SocketCluster.prototype._logObject)
- description and source-code
```javascript
_logObject = function (obj, objType, time) {
  if (!objType) {
    objType = 'Error';
  }
  if (!obj.origin) {
    obj.origin = {};
  }
  if (!obj.origin.type) {
    obj.origin.type = 'Undefined';
  }
  var output = obj.stack || obj.message || obj;

  var logMessage;
  if (obj.origin.pid == null) {
    logMessage = 'Origin: ' + this._capitaliseFirstLetter(obj.origin.type) + '\n' +
      '   [' + objType + '] ' + output;
  } else {
    logMessage = 'Origin: ' + this._capitaliseFirstLetter(obj.origin.type) + ' (PID ' + obj.origin.pid + ')\n' +
      '   [' + objType + '] ' + output;
  }
  this.log(logMessage, time);
}
```
- example usage
```shell
...
  err.stack += '\n    ' + this.colorText('!!', 'red') + ' ' + annotation;
}

err.origin = origin;
err.time = Date.now();
this.emit(this.EVENT_FAIL, err);

this._logObject(err, 'Error');
};

SocketCluster.prototype.warningHandler = function (warning, origin) {
if (!(warning instanceof Object)) {
  // If a string (or null...)
  warning = new UnknownError(warning);
} else if (warning.stack == null) {
...
```

#### <a name="apidoc.element.socketcluster.SocketCluster.prototype._start"></a>[function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>_start ()](#apidoc.element.socketcluster.SocketCluster.prototype._start)
- description and source-code
```javascript
_start = function () {
  var self = this;

  if (self.options.secretKey == null) {
    self.options.secretKey = crypto.randomBytes(32).toString('hex');
  }
  if (this.options.authKey == null && this.options.authPrivateKey == null && this.options.authPublicKey == null) {
    this.options.authKey = crypto.randomBytes(32).toString('hex');
  }
  if (self.options.instanceId == null) {
    self.options.instanceId = uuid.v4();
  }

  self._active = false;

  var brokerEngineServerReady = function () {
    self._brokerEngineServer.removeListener('ready', brokerEngineServerReady);
    self._launchWorkerCluster();
  };

  var launchBrokerEngine = function () {
    var brokerDebugPort = argv['debug-brokers'];
    if (brokerDebugPort == true) {
      brokerDebugPort = self.options.defaultBrokerDebugPort;
    }

    var brokerInspectPort = argv['inspect-brokers'];
    if (brokerInspectPort == true) {
      brokerInspectPort = self.options.defaultBrokerDebugPort;
    }

    self._brokerEngineServer = new self._brokerEngine.Server({
      brokers: self._getBrokerSocketPaths(),
      debug: brokerDebugPort,
      inspect: brokerInspectPort,
      instanceId: self.options.instanceId,
      secretKey: self.options.secretKey,
      expiryAccuracy: self._dataExpiryAccuracy,
      downgradeToUser: self.options.downgradeToUser,
      processTermTimeout: self.options.processTermTimeout,
      brokerOptions: self.options,
      appBrokerControllerPath: self._paths.appBrokerControllerPath,
      appInitControllerPath: self._paths.appInitControllerPath
    });

    self._brokerEngineServer.on('error', function (err) {
      if (err.brokerPid) {
        self._brokerErrorHandler(err.brokerPid, err);
      } else {
        self._brokerEngineErrorHandler(err.pid, err);
      }
    });

    self._brokerEngineServer.on('ready', brokerEngineServerReady);

    self._brokerEngineServer.on('brokerMessage', function (brokerId, data) {
      self.emit('brokerMessage', brokerId, data);
    });
  };

  launchBrokerEngine();
}
```
- example usage
```shell
...
  process.stdin.resume();
  process.stdin.setEncoding('utf8');
}

if (self.options.downgradeToUser && process.platform != 'win32') {
  if (typeof self.options.downgradeToUser == 'number') {
    fs.chownSync(self._socketDirPath, self.options.downgradeToUser, 0);
    self._start();
  } else {
    uidNumber(self.options.downgradeToUser, function (err, uid, gid) {
      if (err) {
        throw new InvalidActionError('Failed to downgrade to user "' + self.options.downgradeToUser + '" - ' + err);
      } else {
        fs.chownSync(self._socketDirPath, uid, gid);
        self._start();
...
```

#### <a name="apidoc.element.socketcluster.SocketCluster.prototype._workerClusterErrorHandler"></a>[function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>_workerClusterErrorHandler (pid, error)](#apidoc.element.socketcluster.SocketCluster.prototype._workerClusterErrorHandler)
- description and source-code
```javascript
_workerClusterErrorHandler = function (pid, error) {
  this.errorHandler(error, {
    type: 'WorkerCluster',
    pid: pid
  });
}
```
- example usage
```shell
...

  this._workerCluster.on('message', function workerHandler(m) {
if (m.type == 'error') {
  var error = scErrors.hydrateError(m.data.error);
  if (m.data.workerPid) {
    self._workerErrorHandler(m.data.workerPid, error);
  } else {
    self._workerClusterErrorHandler(m.data.pid, error);
  }
} else if (m.type == 'warning') {
  var warning = scErrors.hydrateError(m.data.error);
  self._workerWarningHandler(m.data.workerPid, warning);
} else if (m.type == 'ready') {
  self._workerClusterReadyHandler();
} else if (m.type == 'workerStart') {
...
```

#### <a name="apidoc.element.socketcluster.SocketCluster.prototype._workerClusterReadyHandler"></a>[function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>_workerClusterReadyHandler ()](#apidoc.element.socketcluster.SocketCluster.prototype._workerClusterReadyHandler)
- description and source-code
```javascript
_workerClusterReadyHandler = function () {
  var self = this;

  if (!this._active) {
    if (this.options.rebootOnSignal) {
      process.on('SIGUSR2', function () {
        var warning;
        var killOptions = {};
        if (self.options.environment == 'dev') {
          warning = 'Master received SIGUSR2 signal - Shutting down all workers immediately';
          killOptions.immediate = true;
        } else {
          warning = 'Master received SIGUSR2 signal - Shutting down all workers in accordance with processTermTimeout';
        }
        self.warningHandler(warning, {type: 'master'});
        self.killWorkers(killOptions);
        if (self.options.killMasterOnSignal) {
          process.exit();
        }
      });
    }

    this._active = true;
    this._logDeploymentDetails();
  }
}
```
- example usage
```shell
...
  } else {
    self._workerClusterErrorHandler(m.data.pid, error);
  }
} else if (m.type == 'warning') {
  var warning = scErrors.hydrateError(m.data.error);
  self._workerWarningHandler(m.data.workerPid, warning);
} else if (m.type == 'ready') {
  self._workerClusterReadyHandler();
} else if (m.type == 'workerStart') {
  self._workerStartHandler(m.data);
} else if (m.type == 'workerExit') {
  self._workerExitHandler(m.data);
} else if (m.type == 'workerMessage') {
  self.emit('workerMessage', m.workerId, m.data);
}
...
```

#### <a name="apidoc.element.socketcluster.SocketCluster.prototype._workerErrorHandler"></a>[function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>_workerErrorHandler (workerPid, error)](#apidoc.element.socketcluster.SocketCluster.prototype._workerErrorHandler)
- description and source-code
```javascript
_workerErrorHandler = function (workerPid, error) {
  this.errorHandler(error, {
    type: 'Worker',
    pid: workerPid
  });
}
```
- example usage
```shell
...
  data: workerOpts
});

this._workerCluster.on('message', function workerHandler(m) {
  if (m.type == 'error') {
    var error = scErrors.hydrateError(m.data.error);
    if (m.data.workerPid) {
      self._workerErrorHandler(m.data.workerPid, error);
    } else {
      self._workerClusterErrorHandler(m.data.pid, error);
    }
  } else if (m.type == 'warning') {
    var warning = scErrors.hydrateError(m.data.error);
    self._workerWarningHandler(m.data.workerPid, warning);
  } else if (m.type == 'ready') {
...
```

#### <a name="apidoc.element.socketcluster.SocketCluster.prototype._workerExitHandler"></a>[function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>_workerExitHandler (workerInfo)](#apidoc.element.socketcluster.SocketCluster.prototype._workerExitHandler)
- description and source-code
```javascript
_workerExitHandler = function (workerInfo) {
  if (this.options.logLevel > 0) {
    var message = 'Worker ' + workerInfo.id + ' exited - Exit code: ' + workerInfo.code;
    if (workerInfo.signal) {
      message += ', signal: ' + workerInfo.signal;
    }
    this.log(message);
  }
  this.emit(this.EVENT_WORKER_EXIT, workerInfo);
}
```
- example usage
```shell
...
      var warning = scErrors.hydrateError(m.data.error);
      self._workerWarningHandler(m.data.workerPid, warning);
    } else if (m.type == 'ready') {
      self._workerClusterReadyHandler();
    } else if (m.type == 'workerStart') {
      self._workerStartHandler(m.data);
    } else if (m.type == 'workerExit') {
      self._workerExitHandler(m.data);
    } else if (m.type == 'workerMessage') {
      self.emit('workerMessage', m.workerId, m.data);
    }
  });

  this._workerCluster.on('exit', this._handleWorkerClusterExit.bind(this));
};
...
```

#### <a name="apidoc.element.socketcluster.SocketCluster.prototype._workerStartHandler"></a>[function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>_workerStartHandler (workerInfo)](#apidoc.element.socketcluster.SocketCluster.prototype._workerStartHandler)
- description and source-code
```javascript
_workerStartHandler = function (workerInfo) {
  if (this._active && this.options.logLevel > 0 && workerInfo.respawn) {
    this.log('Worker ' + workerInfo.id + ' was respawned');
  }
  this.emit(this.EVENT_WORKER_START, workerInfo);
}
```
- example usage
```shell
...
    }
  } else if (m.type == 'warning') {
    var warning = scErrors.hydrateError(m.data.error);
    self._workerWarningHandler(m.data.workerPid, warning);
  } else if (m.type == 'ready') {
    self._workerClusterReadyHandler();
  } else if (m.type == 'workerStart') {
    self._workerStartHandler(m.data);
  } else if (m.type == 'workerExit') {
    self._workerExitHandler(m.data);
  } else if (m.type == 'workerMessage') {
    self.emit('workerMessage', m.workerId, m.data);
  }
});
...
```

#### <a name="apidoc.element.socketcluster.SocketCluster.prototype._workerWarningHandler"></a>[function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>_workerWarningHandler (workerPid, warning)](#apidoc.element.socketcluster.SocketCluster.prototype._workerWarningHandler)
- description and source-code
```javascript
_workerWarningHandler = function (workerPid, warning) {
  var origin = {
    type: 'Worker',
    pid: workerPid
  };
  this.warningHandler(warning, origin);
}
```
- example usage
```shell
...
  if (m.data.workerPid) {
    self._workerErrorHandler(m.data.workerPid, error);
  } else {
    self._workerClusterErrorHandler(m.data.pid, error);
  }
} else if (m.type == 'warning') {
  var warning = scErrors.hydrateError(m.data.error);
  self._workerWarningHandler(m.data.workerPid, warning);
} else if (m.type == 'ready') {
  self._workerClusterReadyHandler();
} else if (m.type == 'workerStart') {
  self._workerStartHandler(m.data);
} else if (m.type == 'workerExit') {
  self._workerExitHandler(m.data);
} else if (m.type == 'workerMessage') {
...
```

#### <a name="apidoc.element.socketcluster.SocketCluster.prototype.colorText"></a>[function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>colorText (message, color)](#apidoc.element.socketcluster.SocketCluster.prototype.colorText)
- description and source-code
```javascript
colorText = function (message, color) {
  if (this._colorCodes[color]) {
    return '\x1b[0;' + this._colorCodes[color] + 'm' + message + '\x1b[0m';
  } else if (color) {
    return '\x1b[' + color + 'm' + message + '\x1b[0m';
  }
  return message;
}
```
- example usage
```shell
...
self._startSlashRegex = /^\//;

self._dataExpiryAccuracy = 5000;

self._brokerEngine = require(self.options.brokerEngine);

if (self.options.logLevel > 0) {
  console.log('   ' + self.colorText('[Busy]', 'yellow') + ' Launching SocketCluster');
}

process.stdin.on('error', function (err) {
  self.warningHandler(err, {type: 'master'});
});

/*
...
```

#### <a name="apidoc.element.socketcluster.SocketCluster.prototype.errorHandler"></a>[function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>errorHandler (err, origin)](#apidoc.element.socketcluster.SocketCluster.prototype.errorHandler)
- description and source-code
```javascript
errorHandler = function (err, origin) {
  if (!(err instanceof Object)) {
    // If a string (or null...)
    err = new UnknownError(err);
  } else if (err.stack == null) {
    err.stack = err.message;
  }
  var annotation = this._errorAnnotations[err.code];
  if (annotation) {
    err.stack += '\n    ' + this.colorText('!!', 'red') + ' ' + annotation;
  }

  err.origin = origin;
  err.time = Date.now();
  this.emit(this.EVENT_FAIL, err);

  this._logObject(err, 'Error');
}
```
- example usage
```shell
...

self._errorAnnotations = {
  'EADDRINUSE': 'Failed to bind to a port because it was already used by another process.'
};

self._errorDomain = domain.create();
self._errorDomain.on('error', function (err) {
  self.errorHandler(err, {
    type: 'master'
  });
});
self._errorDomain.add(self);

self._errorDomain.run(function () {
  self._init(options);
...
```

#### <a name="apidoc.element.socketcluster.SocketCluster.prototype.killBrokers"></a>[function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>killBrokers ()](#apidoc.element.socketcluster.SocketCluster.prototype.killBrokers)
- description and source-code
```javascript
killBrokers = function () {
  if (this._brokerEngineServer) {
    this._brokerEngineServer.destroy();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socketcluster.SocketCluster.prototype.killWorkers"></a>[function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>killWorkers (options)](#apidoc.element.socketcluster.SocketCluster.prototype.killWorkers)
- description and source-code
```javascript
killWorkers = function (options) {
  if (this._workerCluster) {
    this._workerCluster.send({
      type: 'terminate',
      data: options || {}
    });
  }
}
```
- example usage
```shell
...
    if (self.options.environment == 'dev') {
      warning = 'Master received SIGUSR2 signal - Shutting down all workers immediately';
      killOptions.immediate = true;
    } else {
      warning = 'Master received SIGUSR2 signal - Shutting down all workers in accordance with processTermTimeout';
    }
    self.warningHandler(warning, {type: 'master'});
    self.killWorkers(killOptions);
    if (self.options.killMasterOnSignal) {
      process.exit();
    }
  });
}

this._active = true;
...
```

#### <a name="apidoc.element.socketcluster.SocketCluster.prototype.log"></a>[function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>log (message, time)](#apidoc.element.socketcluster.SocketCluster.prototype.log)
- description and source-code
```javascript
log = function (message, time) {
  if (time == null) {
    time = Date.now();
  }
  console.log(time + ' - ' + message);
}
```
- example usage
```shell
...
self._startSlashRegex = /^\//;

self._dataExpiryAccuracy = 5000;

self._brokerEngine = require(self.options.brokerEngine);

if (self.options.logLevel > 0) {
  console.log('   ' + self.colorText('[Busy]', 'yellow') + ' Launching SocketCluster');
}

process.stdin.on('error', function (err) {
  self.warningHandler(err, {type: 'master'});
});

/*
...
```

#### <a name="apidoc.element.socketcluster.SocketCluster.prototype.sendToBroker"></a>[function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>sendToBroker (brokerId, data)](#apidoc.element.socketcluster.SocketCluster.prototype.sendToBroker)
- description and source-code
```javascript
sendToBroker = function (brokerId, data) {
  this._brokerEngineServer.sendToBroker(brokerId, data);
}
```
- example usage
```shell
...
  type: 'masterMessage',
  workerId: workerId,
  data: data
});
};

SocketCluster.prototype.sendToBroker = function (brokerId, data) {
this._brokerEngineServer.sendToBroker(brokerId, data);
};

// The options object is optional and can have two boolean fields:
// immediate: Shut down the workers immediately without waiting for termination timeout.
// killClusterMaster: Shut down the cluster master (load balancer) as well as all the workers.
SocketCluster.prototype.killWorkers = function (options) {
if (this._workerCluster) {
...
```

#### <a name="apidoc.element.socketcluster.SocketCluster.prototype.sendToWorker"></a>[function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>sendToWorker (workerId, data)](#apidoc.element.socketcluster.SocketCluster.prototype.sendToWorker)
- description and source-code
```javascript
sendToWorker = function (workerId, data) {
  this._workerCluster.send({
    type: 'masterMessage',
    workerId: workerId,
    data: data
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socketcluster.SocketCluster.prototype.triggerInfo"></a>[function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>triggerInfo (info, origin)](#apidoc.element.socketcluster.SocketCluster.prototype.triggerInfo)
- description and source-code
```javascript
triggerInfo = function (info, origin) {
  if (this._active) {
    if (!(origin instanceof Object)) {
      origin = {
        type: origin
      };
    }
    var infoData = {
      origin: origin,
      message: info,
      time: Date.now()
    };
    this.emit(this.EVENT_WARNING, infoData);

    if (this.options.logLevel > 0) {
      this._logObject(infoData, 'Info', infoData.time)
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socketcluster.SocketCluster.prototype.warningHandler"></a>[function <span class="apidocSignatureSpan">socketcluster.SocketCluster.prototype.</span>warningHandler (warning, origin)](#apidoc.element.socketcluster.SocketCluster.prototype.warningHandler)
- description and source-code
```javascript
warningHandler = function (warning, origin) {
  if (!(warning instanceof Object)) {
    // If a string (or null...)
    warning = new UnknownError(warning);
  } else if (warning.stack == null) {
    warning.stack = warning.message;
  }
  warning.origin = origin;
  warning.time = Date.now();

  this.emit(this.EVENT_WARNING, warning);

  if (this.options.logLevel > 1) {
    this._logObject(warning, 'Warning');
  }
}
```
- example usage
```shell
...
self._brokerEngine = require(self.options.brokerEngine);

if (self.options.logLevel > 0) {
  console.log('   ' + self.colorText('[Busy]', 'yellow') + ' Launching SocketCluster');
}

process.stdin.on('error', function (err) {
  self.warningHandler(err, {type: 'master'});
});

/*
  To allow inserting blank lines in console on Windows to aid with debugging.
*/
if (process.platform == 'win32') {
  process.stdin.resume();
...
```



# <a name="apidoc.module.socketcluster.scworker"></a>[module socketcluster.scworker](#apidoc.module.socketcluster.scworker)

#### <a name="apidoc.element.socketcluster.scworker.scworker"></a>[function <span class="apidocSignatureSpan">socketcluster.</span>scworker (options)](#apidoc.element.socketcluster.scworker.scworker)
- description and source-code
```javascript
scworker = function (options) {
  var self = this;

  this.EVENT_ERROR = 'error';
  this.EVENT_WARNING = 'warning';
  this.EVENT_EXIT = 'exit';
  this.EVENT_READY = 'ready';
  this.EVENT_CONNECTION = 'connection';

  this.MIDDLEWARE_START = 'start';

  this.type = 'worker';

  this._errorDomain = domain.create();
  this._errorDomain.on('error', function () {
    self.errorHandler.apply(self, arguments);
  });

  this.start = this._errorDomain.bind(this._start);
  this._errorDomain.run(function () {
    self._init(options);
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.socketcluster.scworker.prototype"></a>[module socketcluster.scworker.prototype](#apidoc.module.socketcluster.scworker.prototype)

#### <a name="apidoc.element.socketcluster.scworker.prototype._calculateStatus"></a>[function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>_calculateStatus ()](#apidoc.element.socketcluster.scworker.prototype._calculateStatus)
- description and source-code
```javascript
_calculateStatus = function () {
  var perMinuteFactor = 60000 / this.options.workerStatusInterval;
  this._httpRPM = this._httpRequestCount * perMinuteFactor;
  this._wsRPM = this._wsRequestCount * perMinuteFactor;
  this._httpRequestCount = 0;
  this._wsRequestCount = 0;

  var memThreshold = this.options.killWorkerMemoryThreshold;

  if (memThreshold != null) {
    var memoryUsage = process.memoryUsage();
    if (memoryUsage.heapUsed > memThreshold) {
      var message = 'Worker killed itself because its memory ';
      message += 'usage of ' + memoryUsage.heapUsed + ' exceeded ';
      message += 'the killWorkerMemoryThreshold of ' + memThreshold;
      var warning = new ResourceLimitError(message);
      this.warningHandler(warning);
      process.exit();
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socketcluster.scworker.prototype._httpRequestHandler"></a>[function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>_httpRequestHandler (req, res)](#apidoc.element.socketcluster.scworker.prototype._httpRequestHandler)
- description and source-code
```javascript
_httpRequestHandler = function (req, res) {
  var self = this;

  this._httpRequestCount++;

  req.exchange = req.global = this.exchange;

  var forwardedFor = req.headers['x-forwarded-for'];

  if (forwardedFor) {
    var forwardedClientIP;
    if (forwardedFor.indexOf(',') > -1) {
      forwardedClientIP = forwardedFor.split(',')[0];
    } else {
      forwardedClientIP = forwardedFor;
    }
    req.forwardedForAddress = forwardedClientIP;
  }
  if (req.connection) {
    req.remoteAddress = req.connection.remoteAddress;
    req.remoteFamily = req.connection.remoteFamily;
    req.remotePort = req.connection.remotePort;
  } else if (req.socket) {
    req.remoteAddress = req.socket.remoteAddress;
    req.remoteFamily = req.socket.remoteFamily;
    req.remotePort = req.socket.remotePort;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socketcluster.scworker.prototype._init"></a>[function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>_init (options)](#apidoc.element.socketcluster.scworker.prototype._init)
- description and source-code
```javascript
_init = function (options) {
  var self = this;

  this.options = {};

  for (var i in options) {
    if (options.hasOwnProperty(i)) {
      this.options[i] = options[i];
    }
  }

  this.id = this.options.id;
  this.isLeader = this.id == 0;

  this._middleware = {};
  this._middleware[this.MIDDLEWARE_START] = [];

  if (this.options.downgradeToUser && process.setuid) {
    try {
      process.setuid(this.options.downgradeToUser);
    } catch (err) {
      this._errorDomain.emit('error', new InvalidActionError('Could not downgrade to user "' + this.options.downgradeToUser +
        '" - Either this user does not exist or the current process does not have the permission' +
        ' to switch to it.'));
    }
  }

  this.brokerEngine = require(this.options.brokerEngine);

  this._paths = options.paths;

  this._httpRequestCount = 0;
  this._wsRequestCount = 0;
  this._httpRPM = 0;
  this._wsRPM = 0;

  this.brokerEngineClient = new this.brokerEngine.Client({
    brokers: this.options.brokers,
    secretKey: this.options.secretKey,
    pubSubBatchDuration: this.options.pubSubBatchDuration
  });

  this.brokerEngineClient.on('error', function (err) {
    var error;
    if (typeof err == 'string') {
      error = new BrokerError(err);
    } else {
      error = err;
    }
    self._errorDomain.emit('error', error);
  });
  this.brokerEngineClient.on('warning', function () {
    self.warningHandler.apply(self, arguments);
  });
  this.exchange = this.global = this.brokerEngineClient.exchange();

  if (this.options.httpServerModule) {
    var httpServerFactory = require(this.options.httpServerModule);
    this.httpServer = httpServerFactory.createServer(this.options.protocolOptions);
  } else {
    if (this.options.protocol == 'https') {
      this.httpServer = https.createServer(this.options.protocolOptions);
    } else {
      this.httpServer = http.createServer();
    }
  }
  this.httpServer.on('request', this._httpRequestHandler.bind(this));
  this.httpServer.on('upgrade', this._httpRequestHandler.bind(this));

  this.httpServer.exchange = this.httpServer.global = this.exchange;

  var httpServerErrorDomain = domain.create();
  httpServerErrorDomain.add(this.httpServer);
  httpServerErrorDomain.on('error', function (err) {
    if (typeof err == 'string') {
      error = new HTTPServerError(err);
    } else {
      error = err;
    }
    self._errorDomain.emit('error', error);
  });

  var secure = this.options.protocol == 'https' ? 1 : 0;

  this.scServer = socketClusterServer.attach(this.httpServer, {
    brokerEngine: this.brokerEngineClient,
    wsEngine: this._paths.wsEnginePath,
    allowClientPublish: this.options.allowClientPublish,
    handshakeTimeout: this.options.handshakeTimeout,
    ackTimeout: this.options.ackTimeout,
    pingTimeout: this.options.pingTimeout,
    pingInterval: this.options.pingInterval,
    origins: this.options.origins,
    appName: this.options.appName,
    path: this.options.path,
    authKey: this.options.authKey,
    authPrivateKey: this.options.authPrivateKey,
    authPublicKey: this.options.authPublicKey,
    authAlgorithm: this.options.authAlgorithm,
    authSignAsync: this.options.authSignAsync,
    authVerifyAsync: this.options.authVerifyAsync,
    authDefaultExpiry: this.options.authDefaultExpiry,
    middlewareEmitWarnings: this.options.middlewareEmitWarnings,
    socketChannelLimit: this.options.socketChannelLimit,
    perMessageDeflate: this.options.perMessageDeflate
  });

  if (this.brokerEngineClient.setSCServer) {
    this.brokerEngineClient.setSCServer(this.scServer);
  }

  // Default authentication engine
  this.setAuthEngine(new AuthEngine());
  this.codec = this.scServer.codec;

  this.scServer.on('_connection', function (socket) {
    // The connection event counts as a WS request
    self._wsRequestCount++;
    socket.on('message', function () {
      self._wsRequestCount++;
    });
    self.emit(self.EVENT_CONNECTION, socket);
  });

  this.scServer.on('warning', function () {
    self.warningHandler.apply(self, arguments);
  });

  this._socketPath = this.scServer.getPath ...
```
- example usage
```shell
...
  self.errorHandler(err, {
    type: 'master'
  });
});
self._errorDomain.add(self);

self._errorDomain.run(function () {
  self._init(options);
});
};

SocketCluster.prototype = Object.create(EventEmitter.prototype);

SocketCluster.prototype._init = function (options) {
var self = this;
...
```

#### <a name="apidoc.element.socketcluster.scworker.prototype._start"></a>[function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>_start ()](#apidoc.element.socketcluster.scworker.prototype._start)
- description and source-code
```javascript
_start = function () {
  var self = this;

  this._httpRequestCount = 0;
  this._wsRequestCount = 0;
  this._httpRPM = 0;
  this._wsRPM = 0;

  if (this._statusInterval != null) {
    clearInterval(this._statusInterval);
  }
  this._statusInterval = setInterval(this._calculateStatus.bind(this), this.options.workerStatusInterval);

  // Run the initController to initialize the global context
  if (this._paths.appInitControllerPath != null) {
      this._initController = require(this._paths.appInitControllerPath);
      this._initController.run(this);
  }

  this._workerController = require(this._paths.appWorkerControllerPath);
  this._workerController.run(this);

  this._startServer();
}
```
- example usage
```shell
...
  process.stdin.resume();
  process.stdin.setEncoding('utf8');
}

if (self.options.downgradeToUser && process.platform != 'win32') {
  if (typeof self.options.downgradeToUser == 'number') {
    fs.chownSync(self._socketDirPath, self.options.downgradeToUser, 0);
    self._start();
  } else {
    uidNumber(self.options.downgradeToUser, function (err, uid, gid) {
      if (err) {
        throw new InvalidActionError('Failed to downgrade to user "' + self.options.downgradeToUser + '" - ' + err);
      } else {
        fs.chownSync(self._socketDirPath, uid, gid);
        self._start();
...
```

#### <a name="apidoc.element.socketcluster.scworker.prototype._startServer"></a>[function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>_startServer ()](#apidoc.element.socketcluster.scworker.prototype._startServer)
- description and source-code
```javascript
_startServer = function () {
  var self = this;

  var options = this.options;

  var start = function () {
    if (options.tcpSynBacklog != null) {
      self.httpServer.listen(options.sourcePort, options.host, options.tcpSynBacklog);
    } else if (options.host != null) {
      self.httpServer.listen(options.sourcePort, options.host);
    } else {
      self.httpServer.listen(options.sourcePort);
    }
  };

  var startMiddleware = this._middleware[this.MIDDLEWARE_START];
  if (startMiddleware.length) {
    var callbackInvoked = false;

    async.applyEachSeries(startMiddleware, options, function (err) {
      if (callbackInvoked) {
        self.emit('warning', new InvalidActionError('Callback for ' + self.MIDDLEWARE_START + ' middleware was already invoked'));
      } else {
        callbackInvoked = true;
        if (err) {
          throw err;
        } else {
          start();
        }
      }
    });
  } else {
    start();
  }
}
```
- example usage
```shell
...

  this.scServer.on('ready', function () {
    self.emit(self.EVENT_READY);
  });
};

SCWorker.prototype.open = function () {
  this._startServer();
};

SCWorker.prototype.close = function (callback) {
  this.scServer.close();
  this.httpServer.close(callback);
};
...
```

#### <a name="apidoc.element.socketcluster.scworker.prototype.addMiddleware"></a>[function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>addMiddleware (type, middleware)](#apidoc.element.socketcluster.scworker.prototype.addMiddleware)
- description and source-code
```javascript
addMiddleware = function (type, middleware) {
  this._middleware[type].push(middleware);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socketcluster.scworker.prototype.close"></a>[function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>close (callback)](#apidoc.element.socketcluster.scworker.prototype.close)
- description and source-code
```javascript
close = function (callback) {
  this.scServer.close();
  this.httpServer.close(callback);
}
```
- example usage
```shell
...
};

SCWorker.prototype.open = function () {
  this._startServer();
};

SCWorker.prototype.close = function (callback) {
  this.scServer.close();
  this.httpServer.close(callback);
};

// getSocketURL is deprecated
SCWorker.prototype.getSocketPath = SCWorker.prototype.getSocketURL = function () {
  return this._socketPath;
};
...
```

#### <a name="apidoc.element.socketcluster.scworker.prototype.errorHandler"></a>[function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>errorHandler (err)](#apidoc.element.socketcluster.scworker.prototype.errorHandler)
- description and source-code
```javascript
errorHandler = function (err) {
  this.emit(this.EVENT_ERROR, err);
}
```
- example usage
```shell
...

self._errorAnnotations = {
  'EADDRINUSE': 'Failed to bind to a port because it was already used by another process.'
};

self._errorDomain = domain.create();
self._errorDomain.on('error', function (err) {
  self.errorHandler(err, {
    type: 'master'
  });
});
self._errorDomain.add(self);

self._errorDomain.run(function () {
  self._init(options);
...
```

#### <a name="apidoc.element.socketcluster.scworker.prototype.getHTTPServer"></a>[function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>getHTTPServer ()](#apidoc.element.socketcluster.scworker.prototype.getHTTPServer)
- description and source-code
```javascript
getHTTPServer = function () {
  return this.httpServer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socketcluster.scworker.prototype.getSCServer"></a>[function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>getSCServer ()](#apidoc.element.socketcluster.scworker.prototype.getSCServer)
- description and source-code
```javascript
getSCServer = function () {
  return this.scServer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socketcluster.scworker.prototype.getSocketPath"></a>[function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>getSocketPath ()](#apidoc.element.socketcluster.scworker.prototype.getSocketPath)
- description and source-code
```javascript
getSocketPath = function () {
  return this._socketPath;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socketcluster.scworker.prototype.getSocketURL"></a>[function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>getSocketURL ()](#apidoc.element.socketcluster.scworker.prototype.getSocketURL)
- description and source-code
```javascript
getSocketURL = function () {
  return this._socketPath;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socketcluster.scworker.prototype.getStatus"></a>[function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>getStatus ()](#apidoc.element.socketcluster.scworker.prototype.getStatus)
- description and source-code
```javascript
getStatus = function () {
  return {
    clientCount: this.scServer.clientsCount,
    httpRPM: this._httpRPM,
    wsRPM: this._wsRPM
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socketcluster.scworker.prototype.handleMasterEvent"></a>[function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>handleMasterEvent ()](#apidoc.element.socketcluster.scworker.prototype.handleMasterEvent)
- description and source-code
```javascript
handleMasterEvent = function () {
  this.emit.apply(this, arguments);
}
```
- example usage
```shell
...

  worker.on('ready', function () {
    worker.start();
    handleReady();
  });
} else if (m.type == 'emit') {
  if (m.data) {
    worker.handleMasterEvent(m.event, m.data);
  } else {
    worker.handleMasterEvent(m.event);
  }
} else if (m.type == 'masterMessage') {
  worker.handleMasterMessage(m);
} else if (m.type == 'terminate') {
  if (worker && !m.data.immediate) {
...
```

#### <a name="apidoc.element.socketcluster.scworker.prototype.handleMasterMessage"></a>[function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>handleMasterMessage (message)](#apidoc.element.socketcluster.scworker.prototype.handleMasterMessage)
- description and source-code
```javascript
handleMasterMessage = function (message) {
  this.emit('masterMessage', message.data);
}
```
- example usage
```shell
...
} else if (m.type == 'emit') {
  if (m.data) {
    worker.handleMasterEvent(m.event, m.data);
  } else {
    worker.handleMasterEvent(m.event);
  }
} else if (m.type == 'masterMessage') {
  worker.handleMasterMessage(m);
} else if (m.type == 'terminate') {
  if (worker && !m.data.immediate) {
    worker.close(function () {
      process.exit();
    });
    setTimeout(function () {
      process.exit();
...
```

#### <a name="apidoc.element.socketcluster.scworker.prototype.open"></a>[function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>open ()](#apidoc.element.socketcluster.scworker.prototype.open)
- description and source-code
```javascript
open = function () {
  this._startServer();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socketcluster.scworker.prototype.removeMiddleware"></a>[function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>removeMiddleware (type, middleware)](#apidoc.element.socketcluster.scworker.prototype.removeMiddleware)
- description and source-code
```javascript
removeMiddleware = function (type, middleware) {
  var middlewareFunctions = this._middleware[type];

  this._middleware[type] = middlewareFunctions.filter(function (fn) {
    return fn != middleware;
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socketcluster.scworker.prototype.sendToMaster"></a>[function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>sendToMaster (data)](#apidoc.element.socketcluster.scworker.prototype.sendToMaster)
- description and source-code
```javascript
sendToMaster = function (data) {
  process.send({
    type: 'workerMessage',
    data: data,
    workerId: this.id
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socketcluster.scworker.prototype.setAuthEngine"></a>[function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>setAuthEngine (authEngine)](#apidoc.element.socketcluster.scworker.prototype.setAuthEngine)
- description and source-code
```javascript
setAuthEngine = function (authEngine) {
  this.auth = authEngine;

  this.httpServer.auth = this.auth;
  this.scServer.setAuthEngine(this.auth);
}
```
- example usage
```shell
...

SCWorker.prototype = Object.create(EventEmitter.prototype);

SCWorker.prototype.setAuthEngine = function (authEngine) {
  this.auth = authEngine;

  this.httpServer.auth = this.auth;
  this.scServer.setAuthEngine(this.auth);
};

SCWorker.prototype.setCodecEngine = function (codecEngine) {
  this.codec = codecEngine;
  this.scServer.setCodecEngine(this.codec);
};
...
```

#### <a name="apidoc.element.socketcluster.scworker.prototype.setCodecEngine"></a>[function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>setCodecEngine (codecEngine)](#apidoc.element.socketcluster.scworker.prototype.setCodecEngine)
- description and source-code
```javascript
setCodecEngine = function (codecEngine) {
  this.codec = codecEngine;
  this.scServer.setCodecEngine(this.codec);
}
```
- example usage
```shell
...

this.httpServer.auth = this.auth;
this.scServer.setAuthEngine(this.auth);
};

SCWorker.prototype.setCodecEngine = function (codecEngine) {
this.codec = codecEngine;
this.scServer.setCodecEngine(this.codec);
};

SCWorker.prototype._init = function (options) {
var self = this;

this.options = {};
...
```

#### <a name="apidoc.element.socketcluster.scworker.prototype.warningHandler"></a>[function <span class="apidocSignatureSpan">socketcluster.scworker.prototype.</span>warningHandler (warning)](#apidoc.element.socketcluster.scworker.prototype.warningHandler)
- description and source-code
```javascript
warningHandler = function (warning) {
  this.emit(this.EVENT_WARNING, warning);
}
```
- example usage
```shell
...
self._brokerEngine = require(self.options.brokerEngine);

if (self.options.logLevel > 0) {
  console.log('   ' + self.colorText('[Busy]', 'yellow') + ' Launching SocketCluster');
}

process.stdin.on('error', function (err) {
  self.warningHandler(err, {type: 'master'});
});

/*
  To allow inserting blank lines in console on Windows to aid with debugging.
*/
if (process.platform == 'win32') {
  process.stdin.resume();
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
