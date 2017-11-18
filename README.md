# ampersand-sync-fetch

[![experimental](http://badges.github.io/stability-badges/dist/experimental.svg)](http://github.com/badges/stability-badges)

Replaces ampersand-sync use of xhr with the fetch api.

You will be using this directly to replace they sync functionality of models.

## browser support

Any browser with fetch api support.

## Install

Use [npm](https://npmjs.com/) to install.

```sh
npm install ampersand-sync-fetch --save
```

## Usage

[![NPM](https://nodei.co/npm/ampersand-sync-fetch.png)](https://www.npmjs.com/package/ampersand-sync-fetch)

```js
var Model = require('ampersand-model');
var syncFetch = require('ampersand-sync-fetch');

module.exports = Model.extend({
	sync: syncFetch
});


var Collection = require('ampersand-rest-collection');
var syncFetch = require('ampersand-sync-fetch');

module.exports = Collection.extend({
	sync: syncFetch
});
```
## License

MIT, see [LICENSE.md](http://github.com/fernandocano/ampersand-sync-fetch/blob/master/LICENSE.md) for details.
