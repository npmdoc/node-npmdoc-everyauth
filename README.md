# api documentation for  [everyauth (v0.4.9)](https://github.com/bnoguchi/everyauth/)  [![npm package](https://img.shields.io/npm/v/npmdoc-everyauth.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-everyauth) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-everyauth.svg)](https://travis-ci.org/npmdoc/node-npmdoc-everyauth)
#### Auth solution (password, facebook, & more) for your node.js Connect & Express apps

[![NPM](https://nodei.co/npm/everyauth.png?downloads=true)](https://www.npmjs.com/package/everyauth)

[![apidoc](https://npmdoc.github.io/node-npmdoc-everyauth/build/screenCapture.buildNpmdoc.browser.%2Fhome%2Ftravis%2Fbuild%2Fnpmdoc%2Fnode-npmdoc-everyauth%2Ftmp%2Fbuild%2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-everyauth/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-everyauth/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-everyauth/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Brian Noguchi",
        "email": "brian.noguchi@gmail.com",
        "url": "https://github.com/bnoguchi/"
    },
    "bugs": {
        "url": "https://github.com/bnoguchi/everyauth/issues"
    },
    "dependencies": {
        "connect": "2.x",
        "debug": "0.x",
        "express": "3.x",
        "node-swt": "0.x",
        "node-wsfederation": "0.x",
        "oauth": "https://github.com/ciaranj/node-oauth/tarball/master",
        "openid": "0.x",
        "request": "2.x",
        "xml2js": "0.x"
    },
    "description": "Auth solution (password, facebook, & more) for your node.js Connect & Express apps",
    "devDependencies": {
        "expect.js": "0.x",
        "jade": "0.x",
        "mocha": "0.x",
        "satisfy": "0.x",
        "tobi": "0.x"
    },
    "directories": {
        "lib": "lib"
    },
    "dist": {
        "shasum": "b5914b8e540be3ce820b7f6afa41b9ffda59aacd",
        "tarball": "https://registry.npmjs.org/everyauth/-/everyauth-0.4.9.tgz"
    },
    "engines": {
        "node": ">=0.4"
    },
    "gitHead": "54c8dd024f202d6c4f7199b216027d10c720f578",
    "homepage": "https://github.com/bnoguchi/everyauth/",
    "keywords": [
        "auth",
        "oauth",
        "password",
        "facebook",
        "openid",
        "twitter",
        "dropbox",
        "authorization",
        "authentication",
        "connect",
        "express"
    ],
    "main": "./index.js",
    "maintainers": [
        {
            "name": "bnoguchi",
            "email": "brian.noguchi@gmail.com"
        }
    ],
    "name": "everyauth",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/bnoguchi/everyauth.git"
    },
    "scripts": {},
    "version": "0.4.9"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module everyauth](#apidoc.module.everyauth)
1.  boolean <span class="apidocSignatureSpan">everyauth.</span>debug
1.  [function <span class="apidocSignatureSpan">everyauth.</span>addRequestGetter (name, fn, isAsync)](#apidoc.element.everyauth.addRequestGetter)
1.  [function <span class="apidocSignatureSpan">everyauth.</span>addRequestMethod (name, fn)](#apidoc.element.everyauth.addRequestMethod)
1.  [function <span class="apidocSignatureSpan">everyauth.</span>helpExpress ()](#apidoc.element.everyauth.helpExpress)
1.  [function <span class="apidocSignatureSpan">everyauth.</span>middleware (opts)](#apidoc.element.everyauth.middleware)
1.  [function <span class="apidocSignatureSpan">everyauth.</span>promise (_module, values)](#apidoc.element.everyauth.promise)
1.  [function <span class="apidocSignatureSpan">everyauth.</span>routeTriggeredSequence (name, _module)](#apidoc.element.everyauth.routeTriggeredSequence)
1.  [function <span class="apidocSignatureSpan">everyauth.</span>step (name, _module)](#apidoc.element.everyauth.step)
1.  [function <span class="apidocSignatureSpan">everyauth.</span>stepSequence (name, module)](#apidoc.element.everyauth.stepSequence)
1.  object <span class="apidocSignatureSpan">everyauth.</span>_req
1.  object <span class="apidocSignatureSpan">everyauth.</span>enabled
1.  object <span class="apidocSignatureSpan">everyauth.</span>modules
1.  object <span class="apidocSignatureSpan">everyauth.</span>promise.prototype
1.  object <span class="apidocSignatureSpan">everyauth.</span>routeTriggeredSequence.prototype
1.  object <span class="apidocSignatureSpan">everyauth.</span>step.prototype
1.  object <span class="apidocSignatureSpan">everyauth.</span>stepSequence.prototype
1.  object <span class="apidocSignatureSpan">everyauth.</span>utils

#### [module everyauth.promise](#apidoc.module.everyauth.promise)
1.  [function <span class="apidocSignatureSpan">everyauth.</span>promise (_module, values)](#apidoc.element.everyauth.promise.promise)

#### [module everyauth.promise.prototype](#apidoc.module.everyauth.promise.prototype)
1.  [function <span class="apidocSignatureSpan">everyauth.promise.prototype.</span>breakTo (seqName)](#apidoc.element.everyauth.promise.prototype.breakTo)

#### [module everyauth.routeTriggeredSequence](#apidoc.module.everyauth.routeTriggeredSequence)
1.  [function <span class="apidocSignatureSpan">everyauth.</span>routeTriggeredSequence (name, _module)](#apidoc.element.everyauth.routeTriggeredSequence.routeTriggeredSequence)
1.  [function <span class="apidocSignatureSpan">everyauth.routeTriggeredSequence.</span>super_ (name, module)](#apidoc.element.everyauth.routeTriggeredSequence.super_)

#### [module everyauth.routeTriggeredSequence.prototype](#apidoc.module.everyauth.routeTriggeredSequence.prototype)
1.  [function <span class="apidocSignatureSpan">everyauth.routeTriggeredSequence.prototype.</span>routeHandler (req, res, next)](#apidoc.element.everyauth.routeTriggeredSequence.prototype.routeHandler)

#### [module everyauth.step](#apidoc.module.everyauth.step)
1.  [function <span class="apidocSignatureSpan">everyauth.</span>step (name, _module)](#apidoc.element.everyauth.step.step)

#### [module everyauth.step.prototype](#apidoc.module.everyauth.step.prototype)
1.  [function <span class="apidocSignatureSpan">everyauth.step.prototype.</span>_unwrapArgs (seq)](#apidoc.element.everyauth.step.prototype._unwrapArgs)
1.  [function <span class="apidocSignatureSpan">everyauth.step.prototype.</span>clone (name, _module)](#apidoc.element.everyauth.step.prototype.clone)
1.  [function <span class="apidocSignatureSpan">everyauth.step.prototype.</span>exec (seq)](#apidoc.element.everyauth.step.prototype.exec)

#### [module everyauth.stepSequence](#apidoc.module.everyauth.stepSequence)
1.  [function <span class="apidocSignatureSpan">everyauth.</span>stepSequence (name, module)](#apidoc.element.everyauth.stepSequence.stepSequence)

#### [module everyauth.stepSequence.prototype](#apidoc.module.everyauth.stepSequence.prototype)
1.  boolean <span class="apidocSignatureSpan">everyauth.stepSequence.prototype.</span>isSeq
1.  [function <span class="apidocSignatureSpan">everyauth.stepSequence.prototype.</span>_bind (priorPromise, nextStep)](#apidoc.element.everyauth.stepSequence.prototype._bind)
1.  [function <span class="apidocSignatureSpan">everyauth.stepSequence.prototype.</span>_transposeArgs (args)](#apidoc.element.everyauth.stepSequence.prototype._transposeArgs)
1.  [function <span class="apidocSignatureSpan">everyauth.stepSequence.prototype.</span>clone (submodule)](#apidoc.element.everyauth.stepSequence.prototype.clone)
1.  [function <span class="apidocSignatureSpan">everyauth.stepSequence.prototype.</span>materialize ()](#apidoc.element.everyauth.stepSequence.prototype.materialize)
1.  [function <span class="apidocSignatureSpan">everyauth.stepSequence.prototype.</span>start ()](#apidoc.element.everyauth.stepSequence.prototype.start)
1.  [function <span class="apidocSignatureSpan">everyauth.stepSequence.prototype.</span>validateSteps ()](#apidoc.element.everyauth.stepSequence.prototype.validateSteps)
1.  object <span class="apidocSignatureSpan">everyauth.stepSequence.prototype.</span>_propertiesToMaterialize

#### [module everyauth.utils](#apidoc.module.everyauth.utils)
1.  [function <span class="apidocSignatureSpan">everyauth.utils.</span>clone (obj)](#apidoc.element.everyauth.utils.clone)
1.  [function <span class="apidocSignatureSpan">everyauth.utils.</span>extractHostname (req)](#apidoc.element.everyauth.utils.extractHostname)
1.  [function <span class="apidocSignatureSpan">everyauth.utils.</span>merge ()](#apidoc.element.everyauth.utils.merge)



# <a name="apidoc.module.everyauth"></a>[module everyauth](#apidoc.module.everyauth)

#### <a name="apidoc.element.everyauth.addRequestGetter"></a>[function <span class="apidocSignatureSpan">everyauth.</span>addRequestGetter (name, fn, isAsync)](#apidoc.element.everyauth.addRequestGetter)
- description and source-code
```javascript
addRequestGetter = function (name, fn, isAsync) {
  this._req._getters[name] = fn;
  return this;
}
```
- example usage
```shell
...
};

everyauth
  .addRequestMethod('logout', function () {
    var req = this;
    delete req.session.auth;
  })
  .addRequestGetter('loggedIn', function () {
    var req = this;
    return !!(req.session && req.session.auth && req.session.auth.loggedIn);
  });

everyauth.modules = {};
everyauth.enabled = {};
...
```

#### <a name="apidoc.element.everyauth.addRequestMethod"></a>[function <span class="apidocSignatureSpan">everyauth.</span>addRequestMethod (name, fn)](#apidoc.element.everyauth.addRequestMethod)
- description and source-code
```javascript
addRequestMethod = function (name, fn) {
  this._req._methods[name] = fn;
  return this;
}
```
- example usage
```shell
...

everyauth.addRequestGetter = function (name, fn, isAsync) {
this._req._getters[name] = fn;
return this;
};

everyauth
.addRequestMethod('logout', function () {
  var req = this;
  delete req.session.auth;
})
.addRequestGetter('loggedIn', function () {
  var req = this;
  return !!(req.session && req.session.auth && req.session.auth.loggedIn);
});
...
```

#### <a name="apidoc.element.everyauth.helpExpress"></a>[function <span class="apidocSignatureSpan">everyauth.</span>helpExpress ()](#apidoc.element.everyauth.helpExpress)
- description and source-code
```javascript
helpExpress = function () {
  console.warn('everyauth.helpExpress is being deprecated. helpExpress is now automatically invoked when it detects express. So
remove everyauth.helpExpress from your code');
  return this;
}
```
- example usage
```shell
...
To enable them:

'''javascript
var express = require('express')
  , everyauth = require('everyauth')
  , app = express.createServer();

everyauth.helpExpress(app);
'''

Then, from within your views, you will have access to the following helpers methods
attached to the helper, 'everyauth':

- 'everyauth.loggedIn'
- 'everyauth.user' - the User document associated with the session
...
```

#### <a name="apidoc.element.everyauth.middleware"></a>[function <span class="apidocSignatureSpan">everyauth.</span>middleware (opts)](#apidoc.element.everyauth.middleware)
- description and source-code
```javascript
middleware = function (opts) {
  opts = merge({
    autoSetupRoutes: true
  }, opts);
  var userAlias = everyauth.expressHelperUserAlias || 'user';
  var router = new ExpressRouter;

  if (opts.autoSetupRoutes) {
    var router = new ExpressRouter();
    var modules = everyauth.enabled;
    for (var _name in modules) {
      var _module = modules[_name];
      _module.validateSequences();
      _module.routeApp(router);
    }
  }

  return function (req, res, next) {
    fetchUserFromSession(req, function (err) {
      addRequestLocals(req, res, userAlias);
      registerReqGettersAndMethods(req);
      if (router) {
        router._dispatch(req, res, next);
      } else {
        next();
      }
    });
  }
}
```
- example usage
```shell
...
    // Step 2 code
    var express = require('express');
    var app = express();
    app
      .use(express.bodyParser())
      .use(express.cookieParser('mr ripley'))
      .use(express.session())
      .use(everyauth.middleware(app));
    '''

## Example Application

There is an example application at [./example](https://github.com/bnoguchi/everyauth/tree/master/example)

To run it:
...
```

#### <a name="apidoc.element.everyauth.promise"></a>[function <span class="apidocSignatureSpan">everyauth.</span>promise (_module, values)](#apidoc.element.everyauth.promise)
- description and source-code
```javascript
promise = function (_module, values) {
  if (values)
    Promise.call(this, values);
  else
    Promise.call(this);
  this.module = _module;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.everyauth.routeTriggeredSequence"></a>[function <span class="apidocSignatureSpan">everyauth.</span>routeTriggeredSequence (name, _module)](#apidoc.element.everyauth.routeTriggeredSequence)
- description and source-code
```javascript
function RouteTriggeredSequence(name, _module) {
  StepSequence.call(this, name, _module);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.everyauth.step"></a>[function <span class="apidocSignatureSpan">everyauth.</span>step (name, _module)](#apidoc.element.everyauth.step)
- description and source-code
```javascript
function Step(name, _module) {
  this.name = name;

  // defineProperty; otherwise,
  // clone will overflow when we clone a module
  Object.defineProperty(this, 'module', { value: _module });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.everyauth.stepSequence"></a>[function <span class="apidocSignatureSpan">everyauth.</span>stepSequence (name, module)](#apidoc.element.everyauth.stepSequence)
- description and source-code
```javascript
function StepSequence(name, module) {
  this.name = name;
  this.module = module;
  this.orderedStepNames = [];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.everyauth.promise"></a>[module everyauth.promise](#apidoc.module.everyauth.promise)

#### <a name="apidoc.element.everyauth.promise.promise"></a>[function <span class="apidocSignatureSpan">everyauth.</span>promise (_module, values)](#apidoc.element.everyauth.promise.promise)
- description and source-code
```javascript
promise = function (_module, values) {
  if (values)
    Promise.call(this, values);
  else
    Promise.call(this);
  this.module = _module;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.everyauth.promise.prototype"></a>[module everyauth.promise.prototype](#apidoc.module.everyauth.promise.prototype)

#### <a name="apidoc.element.everyauth.promise.prototype.breakTo"></a>[function <span class="apidocSignatureSpan">everyauth.promise.prototype.</span>breakTo (seqName)](#apidoc.element.everyauth.promise.prototype.breakTo)
- description and source-code
```javascript
breakTo = function (seqName) {
  if (this._timeout) clearTimeout(this._timeout);

  var args = Array.prototype.slice.call(arguments, 1);
  var _module = this.module
    , seq = _module._stepSequences[seqName];
  if (_module.everyauth.debug)
    console.log('breaking out to ' + seq.name);
  seq = seq.materialize();
  seq.start.apply(seq, args);
  // TODO Garbage collect the abandoned sequence
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.everyauth.routeTriggeredSequence"></a>[module everyauth.routeTriggeredSequence](#apidoc.module.everyauth.routeTriggeredSequence)

#### <a name="apidoc.element.everyauth.routeTriggeredSequence.routeTriggeredSequence"></a>[function <span class="apidocSignatureSpan">everyauth.</span>routeTriggeredSequence (name, _module)](#apidoc.element.everyauth.routeTriggeredSequence.routeTriggeredSequence)
- description and source-code
```javascript
function RouteTriggeredSequence(name, _module) {
  StepSequence.call(this, name, _module);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.everyauth.routeTriggeredSequence.super_"></a>[function <span class="apidocSignatureSpan">everyauth.routeTriggeredSequence.</span>super_ (name, module)](#apidoc.element.everyauth.routeTriggeredSequence.super_)
- description and source-code
```javascript
function StepSequence(name, module) {
  this.name = name;
  this.module = module;
  this.orderedStepNames = [];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.everyauth.routeTriggeredSequence.prototype"></a>[module everyauth.routeTriggeredSequence.prototype](#apidoc.module.everyauth.routeTriggeredSequence.prototype)

#### <a name="apidoc.element.everyauth.routeTriggeredSequence.prototype.routeHandler"></a>[function <span class="apidocSignatureSpan">everyauth.routeTriggeredSequence.prototype.</span>routeHandler (req, res, next)](#apidoc.element.everyauth.routeTriggeredSequence.prototype.routeHandler)
- description and source-code
```javascript
routeHandler = function (req, res, next) {
  // Create a shallow clone, so that seq.values are different per HTTP request
  var seq = this.materialize();
  // Kicks off a sequence of steps based on a route
  seq.start(req, res, next); // BOOM!
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.everyauth.step"></a>[module everyauth.step](#apidoc.module.everyauth.step)

#### <a name="apidoc.element.everyauth.step.step"></a>[function <span class="apidocSignatureSpan">everyauth.</span>step (name, _module)](#apidoc.element.everyauth.step.step)
- description and source-code
```javascript
function Step(name, _module) {
  this.name = name;

  // defineProperty; otherwise,
  // clone will overflow when we clone a module
  Object.defineProperty(this, 'module', { value: _module });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.everyauth.step.prototype"></a>[module everyauth.step.prototype](#apidoc.module.everyauth.step.prototype)

#### <a name="apidoc.element.everyauth.step.prototype._unwrapArgs"></a>[function <span class="apidocSignatureSpan">everyauth.step.prototype.</span>_unwrapArgs (seq)](#apidoc.element.everyauth.step.prototype._unwrapArgs)
- description and source-code
```javascript
_unwrapArgs = function (seq) {
  return this.accepts.reduce( function (args, accept) {
    args.push(seq.values[accept]);
    return args;
  }, []);
}
```
- example usage
```shell
...
}


if (this.debug) {
  console.log('starting step - ' + this.name);
}

var args = this._unwrapArgs(seq);

// There is a hidden last argument to every step function that
// is all the data promised by prior steps up to the step's point
// in time. We cannot anticipate everything a developer may want via
// 'accepts(...)'. Therefore, just in case, we give the developer
// access to all data promised by prior steps via the last argument -- 'seq.values'
args.push(seq.values);
...
```

#### <a name="apidoc.element.everyauth.step.prototype.clone"></a>[function <span class="apidocSignatureSpan">everyauth.step.prototype.</span>clone (name, _module)](#apidoc.element.everyauth.step.prototype.clone)
- description and source-code
```javascript
clone = function (name, _module) {
  var step = new Step(name, _module);
  step.accepts = clone(this.accepts);
  step.promises = clone(this.promises);
  step.description = this.description;
  step.timeout = this.timeout;
  step.errback = this.errback;
  return step;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.everyauth.step.prototype.exec"></a>[function <span class="apidocSignatureSpan">everyauth.step.prototype.</span>exec (seq)](#apidoc.element.everyauth.step.prototype.exec)
- description and source-code
```javascript
exec = function (seq) {
  var accepts = this.accepts;
  var promises = this.promises;
  var block = this.block;
  var _module = this.module;
  var stepName = this.name;
  var step = this;
  function errorCallback (error) {
    // Ensure that seq.values are always passed back to moduleErrback
    if (step.errback) {
      step.errback(error, seq.values);
    } else if (_module._moduleErrback) {
      _module._moduleErrback(error, seq.values);
    } else {
      throw new Error('Missing module or step errback');
    }
  }


  if (this.debug) {
    console.log('starting step - ' + this.name);
  }

  var args = this._unwrapArgs(seq);

  // There is a hidden last argument to every step function that
  // is all the data promised by prior steps up to the step's point
  // in time. We cannot anticipate everything a developer may want via
  // 'accepts(...)'. Therefore, just in case, we give the developer
  // access to all data promised by prior steps via the last argument -- 'seq.values'
  args.push(seq.values);

  var ret;
  try {
    // Apply the step logic

    // Add _super access
    _module._super = function () {
      var step = this.__proto__._steps[stepName];
      if (!step) return;
      var superArgs = arguments.length ? arguments : args;
      step.block.apply(this, superArgs);
    };
    ret = block.apply(_module, args);
    delete _module._super;
  } catch (breakTo) {
    // Catch any sync breakTo's if any
    if (breakTo.isSeq) {
      if (this.module.everyauth.debug)
        console.log("breaking out to " + breakTo.name);
      breakTo.start.apply(breakTo, breakTo.initialArgs);
      // TODO Garbage collect the promise chain
      return;
    } else {
      // Else, we have a regular exception
      errorCallback(breakTo);
    }
  }

  if (promises && promises.length &&
        'undefined' === typeof ret) {
    errorCallback(
      new Error('Step ' + this.name + ' of '' + _module.name +
        '' is promising: ' +  promises.join(', ') +
        ' ; however, the step returns nothing. ' +
        'Fix the step by returning the expected values OR ' +
        'by returning a Promise that promises said values.')
    );
  }
  // Convert return value into a Promise
  // if it's not yet a Promise
  ret = (ret instanceof Promise)
      ? ret
      : Array.isArray(ret)
        ? promises.length === 1
          ? this.module.Promise([ret])
          : this.module.Promise(ret)
        : this.module.Promise([ret]);

  if (seq.debug) {
    ret.callback( function () {
      console.log('...finished step');
    });
  }

  var convertErr = _module._convertErr;
  if (convertErr) {
    var oldErrback = ret.errback;
    ret.errback = function (fn, scope) {
      var oldFn = fn;
      fn = function (err) {
        if (err.constructor === Object) {
          err = convertErr(err);
        } else if ('string' === typeof err) {
          err = new Error(err);
        }
        return oldFn.call(this, err);
      };
      return oldErrback.call(this, fn, scope);
    };
  }

  ret.errback(errorCallback);

  ret.callback( function () {
    // Store the returned values
    // in the sequence's state via seq.values
    var returned = arguments
      , vals = seq.values;
    if (promises !== null) promises.forEach( function (valName, i) {
      vals[valName] = returned[i];
    });
  });

  ret.timeback( function () {
    ret.fail(new Error('Step ' + stepName + ' of '' + _module.name + '' module timed out.'));
  });

  var timeoutMs = this.timeout || _module.moduleTimeout();
  ret.timeout(timeoutMs);

  return ret;
}
```
- example usage
```shell
...
 * @returns {Promise}
 */
StepSequence.prototype._bind = function (priorPromise, nextStep) {
  var nextPromise = new Promise();
  var seq = this;

  priorPromise.callback( function () {
    var resultPromise = nextStep.exec(seq);
    if (!resultPromise) return; // if we have a breakTo
    resultPromise.callback( function () {
      nextPromise.fulfill();
    }); // TODO breakback?
  });
  return nextPromise;
};
...
```



# <a name="apidoc.module.everyauth.stepSequence"></a>[module everyauth.stepSequence](#apidoc.module.everyauth.stepSequence)

#### <a name="apidoc.element.everyauth.stepSequence.stepSequence"></a>[function <span class="apidocSignatureSpan">everyauth.</span>stepSequence (name, module)](#apidoc.element.everyauth.stepSequence.stepSequence)
- description and source-code
```javascript
function StepSequence(name, module) {
  this.name = name;
  this.module = module;
  this.orderedStepNames = [];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.everyauth.stepSequence.prototype"></a>[module everyauth.stepSequence.prototype](#apidoc.module.everyauth.stepSequence.prototype)

#### <a name="apidoc.element.everyauth.stepSequence.prototype._bind"></a>[function <span class="apidocSignatureSpan">everyauth.stepSequence.prototype.</span>_bind (priorPromise, nextStep)](#apidoc.element.everyauth.stepSequence.prototype._bind)
- description and source-code
```javascript
_bind = function (priorPromise, nextStep) {
  var nextPromise = new Promise();
  var seq = this;

  priorPromise.callback( function () {
    var resultPromise = nextStep.exec(seq);
    if (!resultPromise) return; // if we have a breakTo
    resultPromise.callback( function () {
      nextPromise.fulfill();
    }); // TODO breakback?
  });
  return nextPromise;
}
```
- example usage
```shell
...
  // Pipe through the steps
  var priorStepPromise = steps[0].exec(this);

  // If we have a breakTo
  if (!priorStepPromise) return;

  for (var i = 1, l = steps.length; i < l; i++) {
    priorStepPromise = this._bind(priorStepPromise, steps[i]);
  }
  return priorStepPromise;
};

// Used for exposing the leading promise of a step promise chain to the
// incoming args (e.g., [req, res] pair from the route handler)
StepSequence.prototype._transposeArgs = function (args) {
...
```

#### <a name="apidoc.element.everyauth.stepSequence.prototype._transposeArgs"></a>[function <span class="apidocSignatureSpan">everyauth.stepSequence.prototype.</span>_transposeArgs (args)](#apidoc.element.everyauth.stepSequence.prototype._transposeArgs)
- description and source-code
```javascript
_transposeArgs = function (args) {
  var seq = this;
  this.steps[0].accepts.forEach( function (paramName, i) {
    // Map the incoming arguments to the named parameters
    // that the first step is expected to accept.
    seq.values[paramName] = args[i];
  });
}
```
- example usage
```shell
...
 * This kicks off a sequence of steps.
 * Creates a new chain of promises and exposes the leading promise
 * to the incoming (req, res) pair from the route handler
 */
StepSequence.prototype.start = function () {
var steps = this.steps;

this._transposeArgs(arguments);

// Pipe through the steps
var priorStepPromise = steps[0].exec(this);

// If we have a breakTo
if (!priorStepPromise) return;
...
```

#### <a name="apidoc.element.everyauth.stepSequence.prototype.clone"></a>[function <span class="apidocSignatureSpan">everyauth.stepSequence.prototype.</span>clone (submodule)](#apidoc.element.everyauth.stepSequence.prototype.clone)
- description and source-code
```javascript
clone = function (submodule) {
  var sequence = new (this.constructor)(this.name, submodule);
  sequence.orderedStepNames = clone(this.orderedStepNames);
  return sequence;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.everyauth.stepSequence.prototype.materialize"></a>[function <span class="apidocSignatureSpan">everyauth.stepSequence.prototype.</span>materialize ()](#apidoc.element.everyauth.stepSequence.prototype.materialize)
- description and source-code
```javascript
materialize = function () {
  var sequence = Object.create(this)
    , materializedMethods = this._propertiesToMaterialize;
  sequence.values = {};
  for (var i = materializedMethods.length; i--;) {
    var methodName = materializedMethods[i];
    sequence[methodName] = this[methodName];
  }
  return sequence;
}
```
- example usage
```shell
...
  if (this._timeout) clearTimeout(this._timeout);

  var args = Array.prototype.slice.call(arguments, 1);
  var _module = this.module
    , seq = _module._stepSequences[seqName];
  if (_module.everyauth.debug)
    console.log('breaking out to ' + seq.name);
  seq = seq.materialize();
  seq.start.apply(seq, args);
  // TODO Garbage collect the abandoned sequence
};
...
```

#### <a name="apidoc.element.everyauth.stepSequence.prototype.start"></a>[function <span class="apidocSignatureSpan">everyauth.stepSequence.prototype.</span>start ()](#apidoc.element.everyauth.stepSequence.prototype.start)
- description and source-code
```javascript
start = function () {
  var steps = this.steps;

  this._transposeArgs(arguments);

  // Pipe through the steps
  var priorStepPromise = steps[0].exec(this);

  // If we have a breakTo
  if (!priorStepPromise) return;

  for (var i = 1, l = steps.length; i < l; i++) {
    priorStepPromise = this._bind(priorStepPromise, steps[i]);
  }
  return priorStepPromise;
}
```
- example usage
```shell
...

require('util').inherits(RouteTriggeredSequence, StepSequence);

RouteTriggeredSequence.prototype.routeHandler = function (req, res, next) {
  // Create a shallow clone, so that seq.values are different per HTTP request
  var seq = this.materialize();
  // Kicks off a sequence of steps based on a route
  seq.start(req, res, next); // BOOM!
};
...
```

#### <a name="apidoc.element.everyauth.stepSequence.prototype.validateSteps"></a>[function <span class="apidocSignatureSpan">everyauth.stepSequence.prototype.</span>validateSteps ()](#apidoc.element.everyauth.stepSequence.prototype.validateSteps)
- description and source-code
```javascript
validateSteps = function () {
  var steps = this.steps
    , step
    , paramsToDate = []
    , missingParams;
  for (var i = 0, l = steps.length; i < l; i++) {
    step = steps[i];
    if ('undefined' === typeof step.accepts)
      throw new Error('You did not declare accepts for the step: ' + step.name);
    if ('undefined' === typeof step.promises)
      throw new Error('You did not declare promises for the step: ' + step.name);

    if (i === 0)
      paramsToDate = paramsToDate.concat(step.accepts);

    missingParams = step.accepts.filter( function (param) {
      return paramsToDate.indexOf(param) === -1;
    });

    if (i > 0 && missingParams.length)
      throw new Error('At step, ' + step.name + ', you are trying to access the parameters: ' +
        missingParams.join(', ') + ' . However, only the following parameters have been ' +
        'promised from prior steps thus far: ' + paramsToDate.join(', '));

    paramsToDate = paramsToDate.concat(step.promises);

    if ('undefined' === typeof this.module[step.name]())
      // TODO Remove this Error, since invoking the arg to typeof (see line above)
      //      already throws an Error
      throw new Error('No one defined the function for the following step: ' + step.name + ' in the module ' + this.module.name);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.everyauth.utils"></a>[module everyauth.utils](#apidoc.module.everyauth.utils)

#### <a name="apidoc.element.everyauth.utils.clone"></a>[function <span class="apidocSignatureSpan">everyauth.utils.</span>clone (obj)](#apidoc.element.everyauth.utils.clone)
- description and source-code
```javascript
function clone(obj) {
  if (obj === undefined || obj === null)
    return obj
  if (Array.isArray(obj))
    return cloneArray(obj);
  if (obj.constructor == Object)
    return cloneObject(obj);
  return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.everyauth.utils.extractHostname"></a>[function <span class="apidocSignatureSpan">everyauth.utils.</span>extractHostname (req)](#apidoc.element.everyauth.utils.extractHostname)
- description and source-code
```javascript
function extractHostname(req) {
  var headers = req.headers
    , protocol = (req.connection.server instanceof tls.Server ||
                 (req.headers['x-forwarded-proto'] && req.headers['x-forwarded-proto'].slice(0,5) === 'https'))
               ? 'https://'
               : 'http://'
    , host = headers.host;
  return protocol + host;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.everyauth.utils.merge"></a>[function <span class="apidocSignatureSpan">everyauth.utils.</span>merge ()](#apidoc.element.everyauth.utils.merge)
- description and source-code
```javascript
function merge() {
  var mergeInto = {};
  for (var i = 0, l = arguments.length, mergeFrom, k; i < l; i++) {
    mergeFrom = arguments[i];
    for (k in mergeFrom) {
      mergeInto[k] = mergeFrom[k];
    }
  }
  return mergeInto;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
