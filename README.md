<p align="center">
  <img src="https://github.com/PoslinskiNet/ember-pell/raw/master/ember-pell.png" alt="Ember Pell Logo" width="100%">
</p>

[![Build Status](https://api.travis-ci.org/PoslinskiNet/ember-pell.svg?branch=master)](http://travis-ci.org/PoslinskiNet/ember-pell)
[![Greenkeeper badge](https://badges.greenkeeper.io/PoslinskiNet/ember-pell.svg)](https://greenkeeper.io/)
[![Ember Observer Score](https://emberobserver.com/badges/ember-pell.svg)](https://emberobserver.com/addons/ember-pell)
[![NPM package info for ember-pell](https://img.shields.io/npm/dm/ember-pell.svg)](http://npmjs.com/package/ember-pell)
[![License info](https://img.shields.io/npm/l/ember-pell.svg)](http://npmjs.com/package/ember-pell)

# Ember-pell

An Ember Component that uses under the hood the great Pell micro 1KB WYSIWYG editor (https://github.com/jaredreich/pell) that doesn't require jQuery.

# Browser support

![Chrome](https://raw.githubusercontent.com/alrra/browser-logos/master/src/chrome/chrome_48x48.png) | ![Firefox](https://raw.githubusercontent.com/alrra/browser-logos/master/src/firefox/firefox_48x48.png) | ![IE](https://raw.githubusercontent.com/alrra/browser-logos/master/src/edge/edge_48x48.png) | ![Opera](https://raw.githubusercontent.com/alrra/browser-logos/master/src/opera/opera_48x48.png) | ![Safari](https://raw.githubusercontent.com/alrra/browser-logos/master/src/safari/safari_48x48.png)
--- | --- | --- | --- | --- |
5+ ✔ | 4+ ✔ | 9+ ✔ | 11.6+ ✔ | 5+ ✔ |

# Demo

https://ember-twiddle.com/3b21c63730594b39d2b9cbfa8f963803

## Installation

`ember install ember-pell`

## Usage

### 1. Setup value property:
You can declare value variable in your controller or parent component:

```javascript
// app/controllers/task.js
import Ember from 'ember';

export default Ember.Controller.extend({
  value: '<h1>Some html</h1>',
  options: {} // optional param
});
```
#### 2. Use `pell-editor` component

```hbs
{{pell-editor value=value onChange=(action (mut value)) pellOptions=options}}
```

Available options are documented in [Pell repository](https://github.com/jaredreich/pell)

### Linting

* `npm run lint:hbs`
* `npm run lint:js`
* `npm run lint:js -- --fix`

### Running tests

* `ember test` – Runs the test suite on the current Ember version
* `ember test --server` – Runs the test suite in "watch mode"
* `ember try:each` – Runs the test suite against multiple Ember versions

### Running the dummy application

* `ember serve`
* Visit the dummy application at [http://localhost:4200](http://localhost:4200).

For more information on using ember-cli, visit [http://www.ember-cli.com/](http://www.ember-cli.com/).

## LICENSE

See the LICENSE file included in this repository.

<!-- Links -->
[pell]: https://github.com/jaredreich/pell


## Code of Conduct
Please note that this project is released with a Contributor Code of
Conduct. By participating in this project you agree to abide by its
terms, which can be found in the `CODE_OF_CONDUCT.md` file in this
repository.
