# @wemnyelezxnpm/alias-doloremque-saepe <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

Get the `byteLength` out of a DataView, robustly.

This will work in node <= 0.10 and < 0.11.4, where there's no prototype accessor, only a nonconfigurable own property.
It will also work in modern engines where `DataView.prototype.byteLength` has been deleted after this module has loaded.

## Example

```js
const dataViewByteLength = require('@wemnyelezxnpm/alias-doloremque-saepe');
const assert = require('assert');

const ab = new ArrayBuffer(42);
const dv = new DataView(ab);
assert.equal(dataViewByteLength(dv), 42);
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.org/package/@wemnyelezxnpm/alias-doloremque-saepe
[npm-version-svg]: https://versionbadg.es/inspect-js/@wemnyelezxnpm/alias-doloremque-saepe.svg
[deps-svg]: https://david-dm.org/inspect-js/@wemnyelezxnpm/alias-doloremque-saepe.svg
[deps-url]: https://david-dm.org/inspect-js/@wemnyelezxnpm/alias-doloremque-saepe
[dev-deps-svg]: https://david-dm.org/inspect-js/@wemnyelezxnpm/alias-doloremque-saepe/dev-status.svg
[dev-deps-url]: https://david-dm.org/inspect-js/@wemnyelezxnpm/alias-doloremque-saepe#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@wemnyelezxnpm/alias-doloremque-saepe.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@wemnyelezxnpm/alias-doloremque-saepe.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@wemnyelezxnpm/alias-doloremque-saepe.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@wemnyelezxnpm/alias-doloremque-saepe
[codecov-image]: https://codecov.io/gh/inspect-js/@wemnyelezxnpm/alias-doloremque-saepe/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/inspect-js/@wemnyelezxnpm/alias-doloremque-saepe/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/inspect-js/@wemnyelezxnpm/alias-doloremque-saepe
[actions-url]: https://github.com/inspect-js/@wemnyelezxnpm/alias-doloremque-saepe/actions
