# @zitterorg/ipsa-in-aliquam <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

`Object.defineProperty`, but not IE 8's broken one.

## Example

```js
const assert = require('assert');

const $defineProperty = require('@zitterorg/ipsa-in-aliquam');

if ($defineProperty) {
    assert.equal($defineProperty, Object.defineProperty);
} else if (Object.defineProperty) {
    assert.equal($defineProperty, false, 'this is IE 8');
} else {
    assert.equal($defineProperty, false, 'this is an ES3 engine');
}
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

## Security

Please email [@ljharb](https://github.com/ljharb) or see https://tidelift.com/security if you have a potential security vulnerability to report.

[package-url]: https://npmjs.org/package/@zitterorg/ipsa-in-aliquam
[npm-version-svg]: https://versionbadg.es/ljharb/@zitterorg/ipsa-in-aliquam.svg
[deps-svg]: https://david-dm.org/ljharb/@zitterorg/ipsa-in-aliquam.svg
[deps-url]: https://david-dm.org/ljharb/@zitterorg/ipsa-in-aliquam
[dev-deps-svg]: https://david-dm.org/ljharb/@zitterorg/ipsa-in-aliquam/dev-status.svg
[dev-deps-url]: https://david-dm.org/ljharb/@zitterorg/ipsa-in-aliquam#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@zitterorg/ipsa-in-aliquam.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@zitterorg/ipsa-in-aliquam.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@zitterorg/ipsa-in-aliquam.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@zitterorg/ipsa-in-aliquam
[codecov-image]: https://codecov.io/gh/ljharb/@zitterorg/ipsa-in-aliquam/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/ljharb/@zitterorg/ipsa-in-aliquam/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/ljharb/@zitterorg/ipsa-in-aliquam
[actions-url]: https://github.com/zitterorg/ipsa-in-aliquam/actions
