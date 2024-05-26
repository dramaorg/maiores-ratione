# @dramaorg/maiores-ratione <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

For use with React PropTypes. Will error on any prop not explicitly specified.

## Usage

```jsx
import PropTypes from 'prop-types';
import exact from '@dramaorg/maiores-ratione';

function Foo({ foo, bar }) {
  return <div>{foo}{bar}</div>
}
Foo.propTypes = exact({
  foo: PropTypes.string,
  bar: PropTypes.number,
});

<Foo foo="hi" bar={3} /> // no warnings

<Foo foo="hi" bar={3} baz="extra" /> // propTypes warning!
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.org/package/@dramaorg/maiores-ratione
[npm-version-svg]: http://versionbadg.es/ljharb/@dramaorg/maiores-ratione.svg
[deps-svg]: https://david-dm.org/ljharb/@dramaorg/maiores-ratione.svg
[deps-url]: https://david-dm.org/ljharb/@dramaorg/maiores-ratione
[dev-deps-svg]: https://david-dm.org/ljharb/@dramaorg/maiores-ratione/dev-status.svg
[dev-deps-url]: https://david-dm.org/ljharb/@dramaorg/maiores-ratione#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@dramaorg/maiores-ratione.png?downloads=true&stars=true
[license-image]: http://img.shields.io/npm/l/@dramaorg/maiores-ratione.svg
[license-url]: LICENSE
[downloads-image]: http://img.shields.io/npm/dm/@dramaorg/maiores-ratione.svg
[downloads-url]: http://npm-stat.com/charts.html?package=@dramaorg/maiores-ratione
[codecov-image]: https://codecov.io/gh/ljharb/@dramaorg/maiores-ratione/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/ljharb/@dramaorg/maiores-ratione/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/ljharb/@dramaorg/maiores-ratione
[actions-url]: https://github.com/dramaorg/maiores-ratione/actions
