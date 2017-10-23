Checkbox component
==================

[![build status](https://img.shields.io/travis/spasdk/component-checkbox.svg?style=flat-square)](https://travis-ci.org/spasdk/component-checkbox)
[![npm version](https://img.shields.io/npm/v/spa-component-checkbox.svg?style=flat-square)](https://www.npmjs.com/package/spa-component-checkbox)
[![dependencies status](https://img.shields.io/david/spasdk/component-checkbox.svg?style=flat-square)](https://david-dm.org/spasdk/component-checkbox)
[![devDependencies status](https://img.shields.io/david/dev/spasdk/component-checkbox.svg?style=flat-square)](https://david-dm.org/spasdk/component-checkbox?type=dev)
[![Gitter](https://img.shields.io/badge/gitter-join%20chat-blue.svg?style=flat-square)](https://gitter.im/DarkPark/spasdk)


Checkbox input is a component to build user interface, an instance of [Component](https://github.com/spasdk/component) module.


## Installation ##

```bash
npm install spa-component-checkbox
```


## Usage ##

Add the singleton to the scope:

```js
var CheckBox = require('spa-component-checkbox');
```

Create instance with custom config:

```js
var checkBox = new CheckBox({
        value: true,
        group: 'lang'
    });
```

### Constructor config ###

Name | Type | Default value | Description
----- | ----- | ------------- | -------------
value | Boolean | false | Initial state
group | String | null | Group name to work synchronously with other checkboxes

### Methods ###

#### .set() ####

Set the given state.
Does nothing in case the value is already as necessary.

Name | Type | Default value | Description
----- | ----- | ------------- | -------------
value | Boolean | false | value new value to set
{return} | Boolean | false | operation status



#### Examples ####

```js
var _checked;
_checked = checkBox.set(true); 
console.log('checked = ', _checked) // Output: _checked = true

```

## Development mode ##

> There is a global var `DEVELOP` which activates additional consistency checks and protection logic not available in release mode.


## Contribution ##

If you have any problem or suggestion please open an issue [here](https://github.com/spasdk/component-checkbox/issues).
Pull requests are welcomed with respect to the [JavaScript Code Style](https://github.com/DarkPark/jscs).


## License ##

`spa-component-checkbox` is released under the [MIT License](license.md).
