## erisdb-js

`erisdb-js` is a javascript API for [erisdb-tendermint](https://github.com/eris-ltd/erisdb).

**NOTE: Right now it uses tendermint directly, as it has not yet been fully integrated with GenDoug.**

### Installation and usage

npm install eris-db

The main class is `ErisDb`. A standard `ErisDB` instance is created like this:

```
var edbFactory = require('erisdb');

var edb = edbFactory.createInstance("ws://localhost:1337/rpc");

edb.start(callback);

```

The parameters for `createInstance` is the server endpoint as a string, and whether or not to use websockets (false or no value means it will use the default, which is http).

Once ErisDB is started, it is possible to call its methods as per the docs. 

### API Reference

There are bindings for all the RPC methods.

TODO link to web-api pages and jsdoc

### Tests

Tests are done using `mocha`. At this point, there is only integration tests which requires a running erisdb server. These will be moved into a separate repo and replaced with other tests before 1.0.

### Documentation

### Browser

This library will be possible to run from a web-browser.
